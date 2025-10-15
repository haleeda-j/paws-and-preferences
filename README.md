# 🐱 Paws & Preferences: Find Your Favourite Kitty

A fun, interactive web application that helps users discover their cat preferences through an intuitive swipe-based interface, similar to popular dating apps.

[![Live Demo](https://img.shields.io/badge/demo-live-success)](https://haleeda-j.github.io/paws-and-preferences/)
[![GitHub](https://img.shields.io/badge/github-repository-blue)](https://github.com/haleeda-j/paws-and-preferences)

## 🎯 Overview

Paws & Preferences is a single-page application that presents users with a series of adorable cat pictures from the Cataas API. Users can swipe through cats, indicating their preferences, and receive a personalized summary of their favorite felines.

## ✨ Features

- **Intuitive Swipe Gestures**: Swipe right to like, left to dislike (works on both mobile and desktop)
- **Touch & Mouse Support**: Full support for touch screens and traditional mouse/trackpad input
- **Visual Feedback**: Real-time "LIKE" and "NOPE" indicators as you swipe
- **Button Controls**: Alternative button interface (♥ and ✕) for non-swipe interaction
- **Card Stack Animation**: Beautiful depth effect with stacked cards
- **Results Summary**: View all your liked cats in a grid layout with thumbnails
- **Mobile-First Design**: Optimized for mobile devices with responsive layout
- **Smooth Animations**: Fluid transitions and card movements
- **Loading Animations**: Cute rotating cat emoji during image loading
- **Custom Theme**: Warm orange and beige color palette for a cozy feel
- **Mixed Typography**: Playful Quicksand headings with clean Inter body text

## 🚀 Live Demo

**Website**: [https://haleeda-j.github.io/paws-and-preferences/](https://haleeda-j.github.io/paws-and-preferences/)

## 🎨 Design Theme

The application features a warm, cozy color palette:

- **Primary Orange**: `#FFB347` - Headers, like button, accents
- **Cream**: `#FFF8E7` - Container and card backgrounds
- **Coffee Brown**: `#7A5230` - Dislike button, text accents
- **Dark Brown**: `#3B2F2F` - Main text color
- **Light Beige**: `#FAF3E0` - Page background and swipe area

### Typography
- **Quicksand** (Playful & Rounded) - All headings for a friendly feel
- **Inter** (Clean & Modern) - Body text for excellent readability

## 🛠️ Technology Stack

- **HTML5**: Semantic markup structure
- **CSS3**: Modern styling with animations, flexbox, and grid
- **Vanilla JavaScript**: Pure JavaScript for optimal performance
- **Google Fonts**: Quicksand & Inter font families
- **Cataas API**: Cat image source ([https://cataas.com/](https://cataas.com/))
- **GitHub Pages**: Static site hosting

## 📱 How It Works

1. The app loads 15 random cat images from the Cataas API
2. Images are preloaded to ensure smooth performance
3. Users swipe right (or click ♥) to like a cat
4. Users swipe left (or click ✕) to dislike a cat
5. Visual indicators ("LIKE" or "NOPE") appear during swiping
6. Progress counter shows current position (e.g., "Cat 3 of 15")
7. After all cats are reviewed, a summary page displays:
   - Total number of cats liked
   - Thumbnail gallery of all liked cats with orange borders
   - "Start Over" button to restart with new cats

## 🎮 User Interaction

### Swipe Gestures
- **Swipe Right**: Like the cat (shows orange "LIKE" indicator)
- **Swipe Left**: Dislike the cat (shows brown "NOPE" indicator)
- **Short Swipe**: Card returns to center (no action taken)
- **Drag Rotation**: Card rotates slightly while being dragged

### Button Controls
- **♥ Button** (Orange): Like current cat
- **✕ Button** (Brown): Dislike current cat
- **Start Over Button**: Restart the experience with fresh cats

### Visual Feedback
- Card rotates and moves during drag
- Opacity indicators fade in based on swipe distance
- Smooth animations for all transitions
- Loading spinner with rotating cat emoji (🐱)

## 💻 Local Development

1. Clone the repository:
```bash
git clone https://github.com/haleeda-j/paws-and-preferences.git
```

2. Navigate to the project directory:
```bash
cd paws-and-preferences
```

3. Open `index.html` in your browser or use a local server:
```bash
# Using Python 3
python -m http.server 8000

# Or using Node.js with http-server
npx http-server
```

4. Visit `http://localhost:8000` in your browser

## 📂 Project Structure

```
paws-and-preferences/
│
├── index.html          # Main application file (HTML, CSS, JS)
└── README.md          # Project documentation
```

## 🎨 Design Decisions

### Architecture
- **Single File Structure**: All HTML, CSS, and JavaScript in one file for simplicity and easy deployment to GitHub Pages
- **No Dependencies**: Pure vanilla JavaScript for maximum compatibility, fast loading, and zero build process
- **No External Libraries**: Self-contained application with no CDN dependencies

### User Experience
- **Mobile-First Approach**: Touch gestures prioritized, with desktop support as enhancement
- **Card Stack UI**: Familiar Tinder-like interface for intuitive user experience
- **Preloading Strategy**: All cat images load before starting to ensure smooth, uninterrupted swiping
- **Visual Feedback**: Clear indicators and animations provide immediate response to user actions

### Styling
- **Warm Color Palette**: Orange and beige tones create a friendly, inviting atmosphere
- **Solid Colors**: Clean, flat design without gradients for modern aesthetic
- **Custom Fonts**: Quicksand for personality, Inter for clarity
- **Responsive Design**: Adapts beautifully from mobile to desktop screens

## 🔧 Configuration

You can easily customize the application:

### Number of Cats
Change the `CAT_COUNT` variable in JavaScript:
```javascript
const CAT_COUNT = 15; // Change this number (recommended: 10-20)
```

### Colors
Update CSS variables in the style section:
```css
/* Primary colors */
#FFB347  /* Warm Orange */
#FFF8E7  /* Cream */
#7A5230  /* Coffee Brown */
#3B2F2F  /* Dark Brown */
#FAF3E0  /* Light Beige */
```

### Fonts
Replace in the Google Fonts link:
```html
<link href="https://fonts.googleapis.com/css2?family=YourFont&display=swap">
```

## 🌐 Browser Compatibility

Tested and working on:
- ✅ Chrome/Chromium (recommended)
- ✅ Firefox
- ✅ Safari (desktop & iOS)
- ✅ Edge
- ✅ Mobile browsers (iOS Safari, Chrome Mobile, Samsung Internet)

## 📊 Performance Features

- **Image Preloading**: All images load before interaction begins
- **Efficient Animations**: CSS transforms for smooth 60fps animations
- **Event Delegation**: Optimized event listeners
- **Minimal Reflows**: Smart DOM manipulation to reduce layout thrashing
- **Progressive Enhancement**: Works without JavaScript for basic viewing

## 🤝 Contributing

This is an assessment project, but suggestions and feedback are welcome! Feel free to:
- Report bugs or issues
- Suggest new features or improvements
- Share your experience using the app

## 📄 License

This project is created for educational purposes as part of a technical assessment.

## 👤 Author

**Haleeda**
- GitHub: @haleeda-j(https://github.com/haleeda-j)
- Assessment: Paws & Preferences Technical Challenge

## 🙏 Acknowledgments

- **Cataas API** ([cataas.com](https://cataas.com/)) - Providing adorable cat images
- **Google Fonts** - Quicksand and Inter typography
- **Inspiration** - Modern swipe-based UX patterns from dating apps
- **Purpose** - Built as a technical assessment to demonstrate web development skills

## 📝 Assessment Requirements Met

✅ Single-page web application  
✅ Cat image stack display  
✅ Right swipe for "like"  
✅ Left swipe for "dislike"  
✅ Summary page showing liked cats  
✅ Cataas API integration  
✅ Mobile-optimized interface  
✅ Intuitive and pleasant UX  
✅ Smooth animations and transitions  
✅ Hosted on GitHub Pages  
✅ Public GitHub repository  
