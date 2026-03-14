# ChatWeb

A modern web-based chat application with multiple AI integrations.

## Features

- **Multiple AI Providers**: Supports both Groq and OpenRouter APIs
- **Multiple Chat Interfaces**: 
  - `indexx1.html` - Groq-powered chat interface
  - `indexx2.html` - OpenRouter-powered advanced chat interface
  - `index.html` - Main landing page
- **Modern UI**: Beautiful, responsive design with animations
- **Local Storage**: Chat history saved locally
- **Environment Configuration**: Secure API key management

## Setup

### 1. Clone the Repository
```bash
git clone https://github.com/MrKv7/ChatWeb.git
cd ChatWeb
```

### 2. Configure API Keys

#### Option 1: Using Environment Variables (Recommended)
1. Copy the example environment file:
   ```bash
   cp .env.example .env
   ```

2. Edit `.env` with your actual API keys:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   OPENROUTER_API_KEY=your_openrouter_api_key_here
   ```

#### Option 2: Direct Configuration
Edit `config.js` and replace the placeholder values with your actual API keys.

### 3. Get API Keys

#### Groq API Key
1. Go to [Groq Console](https://console.groq.com/)
2. Sign up or log in
3. Navigate to API Keys section
4. Create a new API key
5. Copy the key (starts with `gsk_`)

#### OpenRouter API Key
1. Go to [OpenRouter](https://openrouter.ai/)
2. Sign up or log in
3. Navigate to API Keys section
4. Create a new API key
5. Copy the key (starts with `sk-or-v1-`)

### 4. Run the Application

Simply open any of the HTML files in your web browser:

- **Groq Chat**: Open `indexx1.html`
- **OpenRouter Chat**: Open `indexx2.html`
- **Landing Page**: Open `index.html`

## File Structure

```
ChatWeb/
├── index.html          # Main landing page
├── indexx1.html        # Groq-powered chat interface
├── indexx2.html        # OpenRouter-powered advanced chat
├── config.js           # API configuration file
├── .env                # Environment variables (DO NOT commit)
├── .env.example        # Environment variables template
├── .gitignore          # Git ignore file
└── README.md           # This file
```

## Security

- API keys are stored in environment variables
- `.env` file is included in `.gitignore` to prevent accidental exposure
- Configuration is loaded via `config.js`

## Features Details

### indexx1.html (Groq Chat)
- Clean, modern interface
- Powered by Groq's fast AI models
- Real-time typing indicators
- Message history
- Responsive design

### indexx2.html (OpenRouter Chat)
- Advanced chat interface
- Multiple model selection (GPT-4o, GPT-3.5, etc.)
- Customizable settings (temperature, max tokens)
- Chat export functionality
- Local storage management
- System prompt customization

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

If you encounter any issues:

1. Check that your API keys are correctly configured
2. Ensure you have an active internet connection
3. Verify your API keys have sufficient credits
4. Check the browser console for error messages

## API Usage

Both Groq and OpenRouter APIs are paid services. Please check their respective pricing pages:

- [Groq Pricing](https://groq.com/pricing/)
- [OpenRouter Pricing](https://openrouter.ai/pricing)
