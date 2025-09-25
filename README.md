# Vehicle Sticker Designer

A responsive and interactive web application for designing custom vehicle stickers. Built with React, Fabric.js, and Tailwind CSS.

## Features

- 🚗 **Vehicle Selection**: Choose from various vehicle types (Cars, Bikes, Trucks) with multiple models
- 🎨 **Sticker Gallery**: Browse categorized stickers (Flames, Quotes, Logos, Tribal, Minimal)
- 📁 **File Upload**: Drag & drop support for custom vehicle images and sticker designs
- 🔧 **Advanced Controls**: Adjust opacity, rotation, scaling, and flip/mirror stickers
- 🌙 **Dark/Light Mode**: Toggle between themes for comfortable designing
- 💾 **Save & Share**: Download designs or generate shareable links
- 📱 **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- ⚡ **Real-time Preview**: High-resolution rendering of your designs

## Technology Stack

- **Frontend**: React 18 with Vite
- **Canvas Engine**: Fabric.js for drag & drop transformations
- **Styling**: Tailwind CSS with custom theme system
- **File Handling**: React Dropzone for uploads
- **Icons**: Lucide React
- **Image Processing**: HTML2Canvas for exports

## Prerequisites

Before running this application, make sure you have:

- Node.js (version 16 or higher)
- npm or yarn package manager

## Installation

1. **Clone or download the project files**
   
2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser** and navigate to `http://localhost:3000`

## Dependencies

### Core Dependencies
- `react` & `react-dom` - React framework
- `fabric` - Canvas manipulation library
- `react-router-dom` - Client-side routing
- `lucide-react` - Icon library
- `react-dropzone` - File upload handling
- `html2canvas` - Canvas to image conversion

### Development Dependencies
- `vite` - Build tool and dev server
- `tailwindcss` - CSS framework
- `autoprefixer` & `postcss` - CSS processing
- `eslint` - Code linting

## Project Structure

```
vehicle-sticker-designer/
├── public/
│   └── vehicles/              # Sample vehicle SVG files
├── src/
│   ├── components/           # React components
│   │   ├── Header.jsx        # Top navigation with controls
│   │   ├── Sidebar.jsx       # Left sidebar with tabs
│   │   ├── CanvasEditor.jsx  # Main canvas component
│   │   ├── VehicleSelector.jsx
│   │   ├── StickerGallery.jsx
│   │   ├── FileUploader.jsx
│   │   └── StickerControls.jsx
│   ├── context/              # React contexts
│   │   ├── DesignerContext.jsx
│   │   └── ThemeContext.jsx
│   ├── App.jsx               # Main app component
│   ├── main.jsx             # App entry point
│   └── index.css            # Global styles
├── package.json
├── vite.config.js
├── tailwind.config.js
└── postcss.config.js
```

## Usage Guide

### 1. Select a Vehicle
- Choose a vehicle type (Car, Bike, Truck) from the sidebar
- Select a specific model from the available options
- Or upload your own vehicle image via the Upload tab

### 2. Add Stickers
- Browse sticker categories in the Stickers tab
- Click any sticker to add it to your vehicle
- Upload custom sticker designs via the Upload tab

### 3. Customize Stickers
- Select any sticker on the canvas to access controls
- Adjust opacity, rotation, and size using the Controls tab
- Use flip horizontal/vertical for mirroring effects
- Drag stickers around to reposition them

### 4. Export Your Design
- Use the download button in the header to save as PNG
- Click the share button to generate a shareable link
- Toggle between dark and light themes for better visibility

## Customization

### Adding New Vehicle Models
1. Add SVG files to `public/vehicles/`
2. Update the `vehicleTypes` object in `src/context/DesignerContext.jsx`

### Adding New Sticker Categories
1. Add sticker files to `public/stickers/[category]/`
2. Update the `stickerCategories` object in `DesignerContext.jsx`

### Styling
- Modify `tailwind.config.js` for theme customization
- Edit `src/index.css` for global styles
- Component-specific styles are handled via Tailwind classes

## Development

### Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Building for Production
```bash
npm run build
```
The built files will be in the `dist/` directory.

## Browser Support

- Chrome/Chromium 88+
- Firefox 85+
- Safari 14+
- Edge 88+

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## Future Enhancements

- User authentication and design history
- Backend integration for cloud storage
- Advanced sticker effects (shadows, borders)
- Vector text editing capabilities
- Template marketplace
- Bulk design operations
- Print service integration

## License

This project is open source and available under the MIT License.

## Support

For issues, feature requests, or questions, please create an issue in the project repository or contact the development team.

---

**Happy Designing! 🎨🚗**