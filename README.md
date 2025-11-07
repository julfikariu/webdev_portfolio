# Portfolio Website

A modern, responsive portfolio website built with Vue 3, TypeScript, and Tailwind CSS. Features a clean design with dark mode support, smooth animations, and optimal performance.

## 🚀 Tech Stack

- **Framework**: Vue 3 with Composition API
- **Language**: TypeScript
- **Build Tool**: Vite
- **Styling**: Tailwind CSS
- **Icons**: Lucide Vue
- **Deployment**: Vercel/Netlify

## ✨ Features

- 📱 Fully responsive design
- 🌙 Dark/Light mode toggle
- ⚡ Fast performance with Vite
- 🎨 Modern UI with Tailwind CSS
- ♿ Accessible components
- 🔧 TypeScript for type safety
- 📄 SEO optimized
- 🎯 Smooth scrolling navigation
- 📧 Functional contact form

## 🏃‍♂️ Quick Start

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Installation

1. **Clone the repository**

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173`

## 📜 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## 🎨 Customization

### Personal Information
Update your personal details in the respective components:
- `src/components/sections/AboutSection.vue`
- `src/components/sections/ContactSection.vue`
- `src/components/sections/HeroSection.vue`


## 🚀 Deployment

### Vercel
1. Push your code to GitHub
2. Connect your repository to Vercel
3. Deploy automatically

### Netlify
1. Build the project: `npm run build`
2. Drag and drop the `dist` folder to Netlify

### Manual Deployment
```bash
npm run build
# Upload dist/ folder to your hosting service
```

## 📦 Key Dependencies

### Core
- `vue` - Progressive JavaScript framework
- `typescript` - Type safety
- `vite` - Build tool and dev server

### Styling & UI
- `tailwindcss` - Utility-first CSS framework
- `lucide-vue-next` - Beautiful icons

### Development
- `@vitejs/plugin-vue` - Vite plugin for Vue
- `prettier` - Code formatting

## 🛠️ Configuration Files

- `vite.config.ts` - Vite build configuration
- `tsconfig.json` - TypeScript configuration

## ♿ Accessibility

- Semantic HTML structure
- ARIA labels where needed
- Keyboard navigation support
- Focus management
- Color contrast compliance

## 🌙 Dark Mode

The portfolio includes a seamless dark/light mode toggle that:
- Persists user preference
- Uses system preference as default
- Smooth transitions between modes

## 📱 Responsive Design

- Mobile-first approach
- Breakpoints: sm (640px), md (768px), lg (1024px), xl (1280px)
- Touch-friendly interactions
- Optimized images for different screen sizes

## 🔧 Development

### Adding New Sections
1. Create component in `src/components/sections/`
2. Import and register in `App.vue`
3. Add to navigation


### State Management
Use Vue's Composition API with TypeScript:
```typescript
import { ref, computed } from 'vue'

const darkMode = ref(false)
const toggleDarkMode = () => { darkMode.value = !darkMode.value }
```

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/julfikariu/portfolio/issues).

## 📞 Support

If you have any questions or need help with setup, please open an issue or contact me at julfikariucs15@gmail.com.

---

**Built with ❤️ by Julfikar Ali**

<div align="center">

### ⭐ Don't forget to star this repository if you find it helpful!

</div>