# Next.js Animation Editor

A powerful 3D animation editor built with Next.js, React Three Fiber, and TypeScript. Create, record, and play smooth 3D animations with an intuitive interface.

## ✨ Features

- **3D Scene Rendering**: Built with React Three Fiber for smooth 3D graphics
- **Real-time Animation Recording**: Record object positions and movements in real-time
- **Keyframe Animation**: Create smooth animations between recorded keyframes
- **Interactive Controls**: Intuitive sliders for X/Y positioning and timing
- **Playback Controls**: Play, pause, and stop animations with ease
- **Modern UI**: Clean, responsive interface built with Tailwind CSS
- **TypeScript Support**: Full type safety and better development experience

## 🚀 Tech Stack

- **Frontend**: Next.js 13, React 18, TypeScript
- **3D Graphics**: React Three Fiber, Three.js
- **Styling**: Tailwind CSS
- **State Management**: Zustand
- **UI Components**: Headless UI, React Icons
- **Development**: ESLint, Prettier, Husky

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd Next_Animation-Editor
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🎮 Usage

### Basic Controls

1. **Positioning**: Use the X and Y sliders to position your 3D object
2. **Recording**: Click the "Record" button to capture the current position and time
3. **Playback**: Click "Play" to start the animation, "Pause" to stop
4. **Clear**: Use "Clear" to reset all recorded keyframes

### Animation Workflow

1. **Set Initial Position**: Adjust X/Y sliders to set your starting position
2. **Record Keyframes**: Move the object and record positions at different times
3. **Adjust Timing**: Modify the time slider to control animation speed
4. **Play Animation**: Watch your object smoothly animate between recorded positions

## 🏗️ Project Structure

```
src/
├── app/
│   └── (home)/
│       ├── AnimateModel.tsx    # 3D model and animation logic
│       ├── Scene.tsx           # Three.js canvas setup
│       └── page.tsx            # Main page component
├── components/
│   ├── Control/                # Main control panel
│   ├── Marks/                  # Keyframe markers
│   ├── Slider/                 # Base slider component
│   ├── Time/                   # Time control component
│   ├── XSlider/                # X-axis position slider
│   └── YSlider/                # Y-axis position slider
└── store/
    └── useAdjust.tsx           # Zustand state management
```

## 🔧 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint and Prettier
- `npm run lint:check` - Check code quality without fixing

## 🎨 Customization

### Adding New 3D Models

Modify `AnimateModel.tsx` to load different 3D models:

```tsx
// Example: Load a custom GLTF model
import { useGLTF } from '@react-three/drei'

const AnimateModel = () => {
  const { scene } = useGLTF('/path/to/your/model.gltf')
  // ... animation logic
}
```

### Styling

The project uses Tailwind CSS for styling. Customize the theme in `tailwind.config.ts`:

```ts
module.exports = {
  theme: {
    extend: {
      colors: {
        // Add your custom colors
      }
    }
  }
}
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [React Three Fiber](https://github.com/pmndrs/react-three-fiber) for 3D rendering
- [Three.js](https://threejs.org/) for 3D graphics library
- [Zustand](https://github.com/pmndrs/zustand) for state management
- [Tailwind CSS](https://tailwindcss.com/) for styling

## 📞 Support

If you have any questions or need help, please open an issue on GitHub or contact the development team.

---

**Happy Animating! 🎬✨**
