# 🌓 React Theme Switcher

A modern, responsive React application that demonstrates a clean and intuitive theme switching functionality. Built with React 19, Vite, and Tailwind CSS, this project showcases how to implement a smooth dark/light theme toggle with context API.

## ✨ Features

- **Smooth Theme Switching**: Toggle between light and dark themes with a beautiful animated switch
- **Context API Integration**: Uses React Context for global theme state management
- **Responsive Design**: Fully responsive layout that works on all device sizes
- **Modern UI**: Clean, modern interface with Tailwind CSS styling
- **Persistent Theme**: Theme preference is maintained across sessions
- **Product Card Demo**: Includes a sample product card to showcase theme changes


## 🛠️ Tech Stack

- **React 19** - Latest React with modern features
- **Vite** - Fast build tool and development server
- **Tailwind CSS 4** - Utility-first CSS framework
- **Context API** - React's built-in state management
- **ESLint** - Code linting and formatting

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/SagnikPratihar/theme-switcher-using-react.git
   cd theme-switcher-using-react
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` to see the application

## 🏗️ Project Structure

```
src/
├── components/
│   ├── Card.jsx          # Product card component
│   └── ThemeBtn.jsx      # Theme toggle button
├── context/
│   └── theme.js          # Theme context and provider
├── App.jsx               # Main application component
└── main.jsx             # Application entry point
```

## 🎯 Usage

### Theme Toggle
The theme switcher is located in the top-right corner of the application. Simply click the toggle switch to switch between light and dark themes.

### Components

#### ThemeBtn Component
```jsx
import ThemeBtn from './components/ThemeBtn';

// The toggle button automatically handles theme switching
<ThemeBtn />
```

#### Card Component
```jsx
import Card from './components/Card';

// Displays a product card that adapts to the current theme
<Card />
```

## 🔧 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## 🎨 Customization

### Adding New Themes
To add additional themes, modify the `theme.js` context file:

```jsx
// In src/context/theme.js
export const ThemeContext = createContext({
  themeMode: "light",
  darkTheme: () => {},
  lightTheme: () => {},
  // Add your custom theme function here
  customTheme: () => {},
});
```

### Styling
The application uses Tailwind CSS classes with dark mode variants. To add custom styling:

```css
/* Light mode styles */
.class-name {
  @apply bg-white text-gray-900;
}

/* Dark mode styles */
.dark .class-name {
  @apply bg-gray-800 text-white;
}
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🙏 Acknowledgments

- React team for the amazing framework
- Tailwind CSS for the utility-first approach
- Vite for the fast build tooling

---

⭐ If you found this project helpful, please give it a star!
