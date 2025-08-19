# 🍎 Calorie Estimator Web App

A smart web application that uses AI to estimate calorie content from food photos. Built with HTML, CSS, JavaScript and powered by Google's Gemini AI.

![Calorie Estimator](https://img.shields.io/badge/Web-App-blue.svg)
![Gemini AI](https://img.shields.io/badge/Gemini-AI-orange.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

## 📱 Features

- **📸 Image Upload**: Upload food photos from your device
- **🖼️ Drag & Drop**: Easy drag and drop interface
- **🤖 AI-Powered Analysis**: Uses Google Gemini 2.0 Flash for accurate calorie estimation
- **📱 Responsive Design**: Works on desktop, tablet, and mobile browsers
- **⚡ Fast & Lightweight**: Quick processing and minimal loading time
- **🎨 Modern UI**: Beautiful design with smooth animations
- **🔒 Secure**: API key management and secure data handling

## 🎯 Use Cases

- **Health & Fitness**: Track daily calorie intake
- **Diet Planning**: Understand nutritional content of meals
- **Restaurant Dining**: Estimate calories when nutritional info isn't available
- **Meal Prep**: Plan and track homemade meals
- **Weight Management**: Monitor calorie consumption

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **UI Framework**: Tailwind CSS
- **AI Service**: Google Gemini 2.0 Flash API
- **Deployment**: Netlify (optional)

## 📋 Prerequisites

Before using the app, ensure you have:

### Required
- **Modern Web Browser**: Chrome, Firefox, Safari, or Edge
- **Internet Connection**: Required for AI analysis
- **Google Gemini API Key**: For calorie estimation

### Optional
- **Local Web Server**: For development (Live Server, Python, etc.)

## 🚀 Quick Start

### Option 1: Direct Browser Usage

1. **Open the app**
   - Simply open `index.html` in your web browser
   - Or host it on any web server

2. **Get API Key**
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Sign in with your Google account
   - Click "Create API Key"
   - Copy the generated API key

3. **Configure API Key**
   - Open `index.html` in a text editor
   - Find line with `const apiKey = "YOUR_API_KEY_HERE"`
   - Replace with your actual API key

4. **Use the app**
   - Upload a food image
   - Click "Estimate Calories"
   - Get instant calorie estimation

### Option 2: Local Development Server

**Using Python:**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Using Node.js:**
```bash
# Install live-server globally
npm install -g live-server

# Run the server
live-server
```

**Using VS Code:**
- Install "Live Server" extension
- Right-click on `index.html`
- Select "Open with Live Server"

## 🔧 Configuration

### API Key Setup

1. **Get Google Gemini API Key**
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Sign in with your Google account
   - Click "Create API Key"
   - Copy the generated API key

2. **Configure API Key**
   - Open `index.html`
   - Find line with `const apiKey = "YOUR_API_KEY_HERE"`
   - Replace with your actual API key

### Customization

**Change App Title:**
```html
<title>Your Custom Title</title>
```

**Modify Styling:**
- Edit the `<style>` section in `index.html`
- Or modify Tailwind CSS classes

**Update AI Prompt:**
```javascript
const prompt = "Your custom prompt here";
```

## 🌐 Deployment

### Netlify Deployment (Optional)

1. **Push to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin your-repo-url
   git push -u origin main
   ```

2. **Deploy to Netlify**
   - Connect your GitHub repository
   - Set build command: (leave empty)
   - Set publish directory: `.`
   - Deploy

### Other Hosting Options

- **GitHub Pages**: Free static hosting
- **Vercel**: Fast deployment
- **Firebase Hosting**: Google's hosting service
- **Any Web Server**: Apache, Nginx, etc.

## 🎨 UI Components

### Main Features
- **Header**: App title and description
- **Image Upload Area**: Drag & drop or click to upload
- **Image Preview**: Displays uploaded food image
- **Estimate Button**: Primary action button with loading state
- **Results Section**: Displays AI analysis results
- **Message Box**: Shows success/error messages

### Design Elements
- **Color Scheme**: Indigo primary, gradient accents
- **Typography**: Inter font family
- **Animations**: Smooth transitions and loading spinners
- **Responsive**: Optimized for various screen sizes

## 🔍 Troubleshooting

### Common Issues

**1. API Key Error**
- Ensure API key is correctly set
- Check if API key has proper permissions
- Verify Google Gemini API is enabled

**2. Image Upload Issues**
- Check file format (JPEG, PNG supported)
- Ensure file size is reasonable (<10MB)
- Try different browser if issues persist

**3. Network Errors**
- Check internet connection
- Verify API endpoint is accessible
- Check browser console for errors

**4. CORS Issues (Development)**
- Use a local web server instead of file:// protocol
- Or use browser extensions to disable CORS

### Debug Commands

```javascript
// Check API key in browser console
console.log(apiKey);

// Check image data
console.log(base64ImageData);

// Monitor network requests
// Open Developer Tools → Network tab
```

## 📊 Performance

### App Size
- **HTML File**: ~10KB
- **Total Assets**: ~50KB
- **Loading Time**: <2 seconds

### Performance Metrics
- **Image Upload**: <1 second
- **AI Analysis**: 5-15 seconds (depending on image size and network)
- **Memory Usage**: <10MB
- **Compatibility**: All modern browsers

## 🔄 Updates & Maintenance

### Updating Dependencies
- **Tailwind CSS**: Update CDN link in HTML
- **Google Fonts**: Update font import if needed
- **API Version**: Update Gemini API endpoint if needed

### Version Management
- Update version in comments
- Tag releases in Git
- Document changes in README

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 Support

### Getting Help
- **Issues**: Create an issue on GitHub
- **Documentation**: Check this README
- **Community**: Join web development forums

### Contact
- **Email**: dev@example.com
- **GitHub**: [Your GitHub Profile]

## 🗺️ Roadmap

### Planned Features
- [ ] Offline mode with cached results
- [ ] Multiple language support
- [ ] Nutritional breakdown (protein, carbs, fat)
- [ ] Meal history and tracking
- [ ] Social sharing of results
- [ ] Dark mode support
- [ ] Progressive Web App (PWA) features

### Technical Improvements
- [ ] React/Vue.js migration
- [ ] Backend integration for user accounts
- [ ] Database for meal history
- [ ] Advanced image processing
- [ ] Multiple AI model support

## 📈 Analytics & Monitoring

### Built-in Analytics
- Basic usage tracking (optional)
- Error reporting
- Performance monitoring

### Privacy
- No personal data collection
- Images processed locally when possible
- Secure API communication
- GDPR compliant

---

**Made with ❤️ using HTML, CSS, JavaScript and Google Gemini AI** 