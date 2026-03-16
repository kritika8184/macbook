# 🍎 MacBook Pro 3D Showcase

A stunning, immersive 3D website showcasing the MacBook Pro with interactive features, smooth animations, and modern web technologies. Experience the MacBook Pro like never before with realistic 3D visualization, dynamic color switching, and scroll-triggered animations.

![MacBook Pro 3D Showcase](https://img.shields.io/badge/React-19.2.0-blue) ![Three.js](https://img.shields.io/badge/Three.js-0.183.2-green) ![GSAP](https://img.shields.io/badge/GSAP-3.14.2-orange) ![Vite](https://img.shields.io/badge/Vite-7.3.1-purple)

## ✨ Features

### 🎮 Interactive 3D Model
- **Realistic MacBook Pro 3D Model**: High-quality 3D representation with accurate proportions
- **Color Variants**: Switch between Space Black and Silver finishes
- **Size Options**: Toggle between 14" and 16" models with dynamic scaling
- **Responsive Design**: Optimized viewing experience across all devices

### 🎬 Immersive Animations
- **Scroll-Triggered Animations**: Smooth GSAP animations activated by scroll position
- **Cinematic Transitions**: Fluid transitions between sections
- **Performance Optimized**: Hardware-accelerated animations for smooth 60fps experience

### 📱 Modern UI/UX
- **Responsive Layout**: Mobile-first design that works on all screen sizes
- **Apple-Inspired Design**: Clean, minimalist interface following Apple's design language
- **Interactive Controls**: Intuitive color and size selection interface
- **Video Integration**: High-quality video content showcasing features

### 🚀 Technical Highlights
- **React 19**: Latest React features with modern hooks and patterns
- **Three.js Integration**: Seamless 3D graphics with React Three Fiber
- **State Management**: Zustand for lightweight, efficient state handling
- **Modern Build Tools**: Vite for lightning-fast development and builds

## 🛠️ Technologies Used

### Core Technologies
- **[React](https://reactjs.org/)** (19.2.0) - UI framework
- **[Three.js](https://threejs.org/)** (0.183.2) - 3D graphics library
- **[GSAP](https://greensock.com/gsap/)** (3.14.2) - Animation library

### React Three.js Ecosystem
- **[@react-three/fiber](https://docs.pmnd.rs/react-three-fiber)** - React renderer for Three.js
- **[@react-three/drei](https://docs.pmnd.rs/drei)** - Useful helpers for React Three Fiber

### Styling & UI
- **[Tailwind CSS](https://tailwindcss.com/)** (4.2.1) - Utility-first CSS framework
- **[clsx](https://github.com/lukeed/clsx)** - Conditional className utility

### State Management & Utilities
- **[Zustand](https://zustand-demo.pmnd.rs/)** (5.0.11) - Lightweight state management
- **[react-responsive](https://github.com/yocontra/react-responsive)** - Media queries in React

### Development Tools
- **[Vite](https://vitejs.dev/)** (7.3.1) - Next-generation frontend tooling
- **[ESLint](https://eslint.org/)** - Code linting and formatting

## 🚀 Getting Started

### Prerequisites
- **Node.js** (version 18 or higher)
- **npm** or **yarn** package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd macbook
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` to view the application

### Build for Production

```bash
npm run build
# or
yarn build
```

### Preview Production Build

```bash
npm run preview
# or
yarn preview
```

## 📁 Project Structure

```
macbook/
├── public/                 # Static assets
│   ├── videos/            # Video files for showcases
│   └── mask-logo.svg      # Logo assets
├── src/
│   ├── components/        # React components
│   │   ├── NavBar.jsx     # Navigation component
│   │   ├── Hero.jsx       # Hero section
│   │   ├── ProductViewer.jsx  # 3D MacBook viewer
│   │   ├── Showcase.jsx   # Feature showcase
│   │   ├── Performance.jsx # Performance metrics
│   │   ├── Features.jsx   # Features section
│   │   ├── Highlights.jsx # Product highlights
│   │   └── Footer.jsx     # Footer component
│   ├── three/             # Three.js related components
│   │   ├── StudioLights.jsx   # 3D lighting setup
│   │   └── ModelSwitcher.jsx  # 3D model management
│   ├── store/             # State management
│   │   └── index.js       # Zustand store configuration
│   ├── constants/         # Application constants
│   │   └── index.js       # Shared constants
│   ├── App.jsx           # Main application component
│   ├── main.jsx          # Application entry point
│   └── index.css         # Global styles
├── package.json          # Dependencies and scripts
├── vite.config.js        # Vite configuration
├── tailwind.config.js    # Tailwind CSS configuration
└── README.md            # Project documentation
```

## 🎯 Key Components

### ProductViewer
The heart of the 3D experience, featuring:
- Interactive 3D MacBook model
- Color and size controls
- Responsive camera positioning
- Real-time model updates

### Showcase
Immersive section highlighting:
- M4 chip performance
- Scroll-triggered animations
- Video integration
- Performance statistics

### Three.js Integration
- **StudioLights**: Professional lighting setup for realistic rendering
- **ModelSwitcher**: Dynamic model loading and switching
- **Camera Controls**: Optimized viewing angles and positions

## 🎨 Customization

### Adding New Colors
Update the color options in `src/components/ProductViewer.jsx`:
```jsx
<div onClick={() => setColor('#your-color')}
     className={clsx('bg-your-color-class', color === '#your-color' && 'active')} />
```

### Modifying Animations
GSAP animations can be customized in individual components:
```jsx
useGSAP(() => {
    gsap.timeline({
        scrollTrigger: {
            trigger: '#your-section',
            // Your animation configuration
        }
    });
});
```

### Adding New 3D Models
Place your 3D models in the `public` directory and update the `ModelSwitcher` component to load them.

## 🔧 Performance Optimization

- **Lazy Loading**: Components and assets are loaded on demand
- **Responsive Images**: Optimized assets for different screen sizes
- **Hardware Acceleration**: GPU-accelerated animations and 3D rendering
- **Code Splitting**: Automatic code splitting with Vite
- **Tree Shaking**: Unused code elimination in production builds

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🙏 Acknowledgments

- **Apple Inc.** for design inspiration
- **Three.js Community** for excellent 3D web graphics
- **GSAP Team** for powerful animation tools
- **React Three Fiber** for seamless React-Three.js integration

## 📞 Support

If you have any questions or need help with the project, please:
- Open an issue on GitHub
- Check the documentation for Three.js and GSAP
- Review the component structure for implementation details

---

**Built with ❤️ using React, Three.js, and GSAP**