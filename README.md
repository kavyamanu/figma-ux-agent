# Figma UX Agent

A powerful AI-powered design assistant plugin for Figma that helps you create beautiful, professional designs using your component libraries.

## Features

- 🤖 AI-powered design generation
- 📚 Support for multiple component libraries
- 🔄 Real-time design preview
- 🚀 Fast component rendering
- 💾 Component caching for improved performance
- 🛑 Generation control with stop functionality
- 🔍 Detailed design previews

## Prerequisites

- Node.js (v14 or higher)
- Figma Desktop App
- Access to component libraries in Figma
- Gemini API Key
- Figma Access Token

## API Keys Setup

### Generating Gemini API Key
1. Go to [Google AI Studio](https://aistudio.google.com/apikey)
2. Click on "Get API Key" in the top right corner
3. Click "Create API key in new project"
4. Copy the generated API key

### Generating Figma Access Token
1. Open Figma Desktop App
2. Click on your profile icon in the top left corner
3. Select "Help & Account" → "Account Settings"
4. Switch to the "Security" tab
5. Scroll down to "Personal access tokens"
6. Click "Generate new token"
7. Give your token a name (e.g., "Figma UX Agent")
8. Select "Full access" for permissions
9. Click "Generate token"
10. Copy the generated token immediately (you won't be able to see it again)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/figma-ux-agent.git
cd figma-ux-agent
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
Create a `.env` file in the root directory with:
```
OPENAI_API_KEY=your_gemini_api_key
FIGMA_TOKEN=your_figma_access_token
PORT=3000
```

4. Start the server:
```bash
npm run dev
```

5. In Figma:
   - Go to Plugins > Development > Import plugin from manifest
   - Select the `manifest.json` file from the project directory

## Usage

1. Open the plugin in Figma
2. Enter your design requirements in the chat interface
3. The AI will analyze your prompt and generate a preview
4. Review the preview and components to be used
5. Click generate to create the design
6. Use the stop button to halt generation if needed

## Component Libraries

The plugin supports multiple component libraries:
- Core Components
- Web Components
- SLDS Components

Each library is configured with its own file key and can be used independently or together.

## Development

### Project Structure
```
figma-ux-agent/
├── src/
│   ├── plugin.ts        # Figma plugin code
│   ├── server.js        # Local server for AI integration
│   └── index.html       # Plugin UI
├── manifest.json        # Plugin manifest
└── package.json         # Project dependencies
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Support

For support, please open an issue in the GitHub repository or contact the maintainers.
