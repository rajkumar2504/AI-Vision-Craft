# AI Vision Craft

A modern, responsive web application that generates AI-powered images using Hugging Face's state-of-the-art models. Transform your imagination into stunning visuals with an intuitive interface and powerful AI models.

![AI Vision Craft Demo]<img width="1795" height="899" alt="Screenshot 2025-09-20 155034" src="https://github.com/user-attachments/assets/c098e94b-149f-4039-94e5-0ced4e74d870" />


## ✨ Features

- **Multiple AI Models**: Choose from various state-of-the-art models including FLUX, Stable Diffusion XL, and Stable Diffusion 3
- **Flexible Image Generation**: Generate 1-5 images simultaneously with customizable aspect ratios
- **Smart Prompt System**: Random prompt generator with typing animation effects
- **Responsive Design**: Beautiful interface that works seamlessly on desktop and mobile devices
- **Dark/Light Theme**: Toggle between themes with system preference detection
- **Image Management**: Built-in download functionality for generated images
- **Real-time Generation**: Live loading indicators and error handling
- **Modern UI/UX**: Glassmorphism effects, smooth animations, and contemporary design

## 🚀 Quick Start

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Hugging Face API key ([Get one here](https://huggingface.co/settings/tokens))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ai-vision-craft.git
   cd ai-vision-craft
   ```

2. **Configure API Key**
   
   Open `script.js` and replace the API key:
   ```javascript
   const API_KEY = "YOUR_HUGGING_FACE_API_KEY_HERE";
   ```

3. **Launch the Application**
   
   Simply open `index.html` in your web browser or serve it using a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (with http-server)
   npx http-server
   
   # Using PHP
   php -S localhost:8000
   ```

4. **Start Creating!**
   
   Navigate to `http://localhost:8000` and start generating amazing images!

## 🎯 How to Use

1. **Enter Your Prompt**: Describe the image you want to generate in the text area
2. **Select Model**: Choose from available AI models (FLUX, Stable Diffusion variants)
3. **Set Parameters**: 
   - Choose number of images (1-5)
   - Select aspect ratio (Square, Landscape, Portrait)
4. **Generate**: Click the "Generate" button and watch your ideas come to life!
5. **Download**: Hover over generated images to reveal the download button

### Quick Prompt Ideas

Use the dice button (🎲) to get random prompt suggestions, or try these categories:

- **Nature**: "A serene mountain lake at sunrise with mist"
- **Fantasy**: "A magical forest with glowing mushrooms and fairy lights"
- **Sci-Fi**: "A futuristic city with flying cars and neon lights"
- **Abstract**: "Colorful geometric patterns in a cosmic setting"

## 🛠 Technical Details

### Supported AI Models

| Model | Description | Best For |
|-------|-------------|----------|
| **FLUX.1-dev** | Latest FLUX development model | High-quality, detailed images |
| **FLUX.1-schnell** | Fast FLUX variant | Quick generation, good quality |
| **Stable Diffusion XL** | Enhanced SD model | Versatile, reliable results |
| **Stable Diffusion 3** | Latest SD iteration | Advanced prompt understanding |

### File Structure

```
ai-vision-craft/
├── index.html          # Main HTML structure
├── style.css           # Styling and themes
├── script.js           # JavaScript functionality
└── README.md           # This file
```

### Key Technologies

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Styling**: Custom CSS with CSS Variables for theming
- **Icons**: Font Awesome 6.4.0
- **Fonts**: Google Fonts (Inter)
- **API**: Hugging Face Inference API

## 🎨 Customization

### Adding New Models

To add new Hugging Face models, update the select options in `index.html`:

```html
<option value="model-organization/model-name">Display Name</option>
```

### Modifying Themes

Customize colors by editing CSS variables in `style.css`:

```css
:root {
  --color-primary: #4CAF50;
  --color-gradient: linear-gradient(135deg, #5C56E1, #8B5CF6);
  /* Add your custom colors */
}
```

### Adding Prompt Categories

Extend the example prompts array in `script.js`:

```javascript
const examplePrompts = [
  "Your custom prompt here",
  // Add more prompts...
];
```

## 🔧 Configuration

### API Settings

The application uses Hugging Face's Inference API. Key configuration options:

- **Model Selection**: Choose from available models in the dropdown
- **Image Dimensions**: Automatically calculated based on aspect ratio
- **Cache Control**: Disabled for fresh results (`"x-use-cache": "false"`)

### Browser Compatibility

- ✅ Chrome 88+
- ✅ Firefox 85+
- ✅ Safari 14+
- ✅ Edge 88+

## 📱 Responsive Design

The application is fully responsive with breakpoints:

- **Desktop**: Full grid layout with all features
- **Tablet**: Adapted grid and navigation
- **Mobile**: Stacked layout with touch-optimized controls

## 🐛 Troubleshooting

### Common Issues

**Images not generating**
- Check your API key is valid and has sufficient quota
- Ensure you have an active internet connection
- Try a different model if one isn't working

**Slow generation**
- Some models are slower than others (try FLUX.1-schnell for speed)
- Hugging Face models may need "warm-up" time
- Consider reducing image count for faster results

**Layout issues**
- Clear browser cache and refresh
- Ensure you're using a supported browser
- Check console for JavaScript errors

### Error Messages

- **"Generation failed!"**: Usually indicates API quota exceeded or model unavailable
- **Network errors**: Check internet connection and API endpoint status

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for:

- Bug fixes
- New features
- UI/UX improvements
- Documentation updates
- Additional AI model integrations

### Development Setup

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and test thoroughly
4. Commit with clear messages: `git commit -m "Add feature description"`
5. Push and create a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Hugging Face** for providing excellent AI models and APIs
- **Font Awesome** for beautiful icons
- **Google Fonts** for the Inter typography
- **Stable Diffusion** and **FLUX** teams for creating amazing AI models

## 🔗 Links

- [Hugging Face Models](https://huggingface.co/models)
- [Font Awesome Icons](https://fontawesome.com/)
- [Google Fonts](https://fonts.google.com/)

---

**Made with ❤️ and AI magic**

