# AutoAccess Browser Extension

AutoAccess is a powerful browser extension that enhances web accessibility for disabled individuals through AI-powered features. The extension automatically improves websites by adding image descriptions, adjusting color contrast, and enabling voice navigation.

## Features

### AI Image Labeling
- Automatically generates descriptive alt text for images
- Uses Azure Vision API for accurate image recognition
- Supports multiple languages
- Configurable confidence threshold

### Color Contrast Enhancement
- Automatically adjusts color contrast to meet WCAG standards
- Supports both AA (4.5:1) and AAA (7:1) compliance levels
- Real-time color adjustments
- Customizable color schemes

### Voice Navigation
- Hands-free website navigation
- Voice commands for scrolling, zooming, and navigation
- Text-to-speech for reading content
- Multiple language support
- Customizable voice commands

## Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/autoaccess.git
```

2. Open Chrome and navigate to `chrome://extensions/`

3. Enable "Developer mode" in the top right

4. Click "Load unpacked" and select the extension directory

## Configuration

1. Open the extension options by right-clicking the extension icon and selecting "Options"

2. Configure your Azure Vision API credentials:
   - Enter your API Key
   - Enter your API Endpoint

3. Customize feature settings:
   - Enable/disable features
   - Adjust confidence thresholds
   - Select WCAG compliance level
   - Choose voice command language

## Usage

### Basic Usage
1. Click the extension icon to open the popup
2. Toggle features on/off using the switches
3. Access settings through the options menu

### Voice Commands
- "Scroll up/down" - Scroll the page
- "Zoom in/out" - Adjust zoom level
- "Go to [link text]" - Navigate to a link
- "Read this" - Read selected text
- "Focus [element]" - Focus on a specific element

## Premium Features

### Free Plan
- Basic image labeling
- Standard color contrast
- Limited voice commands
- Community support

### Monthly Plan ($9.99/month)
- Advanced image labeling
- Custom color schemes
- Unlimited voice commands
- Priority support
- Ad-free experience

### Yearly Plan ($99.99/year)
- All monthly features
- Early access to new features
- 2 months free
- Dedicated support
- Custom integrations

## Development

### Project Structure
```
autoaccess/
├── manifest.json
├── popup.html
├── popup.js
├── content.js
├── background.js
├── options.html
├── options.js
├── payment.js
├── config.js
├── success.html
├── cancel.html
├── pricing.html
└── styles/
    ├── popup.css
    └── options.css
```

### Building from Source
1. Install dependencies:
```bash
npm install
```

2. Build the extension:
```bash
npm run build
```

3. Load the extension in Chrome as described in the Installation section

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support, please:
1. Check the [documentation](docs/)
2. Open an issue on GitHub
3. Contact support@autoaccess.com

## Acknowledgments

- Azure Vision API for image recognition
- Web Speech API for voice commands
- Chrome Extension APIs
- WCAG guidelines for accessibility standards 