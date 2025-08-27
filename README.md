# Zihan Sun - Personal Portfolio

A clean and minimalist personal portfolio website built with Vue 3, showcasing machine learning and blockchain projects.

## Features

- 🎨 Clean and modern design
- 📱 Fully responsive layout
- ⚡ Built with Vue 3 and Vite
- 🚀 Optimized for GitHub Pages deployment
- 🔗 Integration with GitHub projects

## Tech Stack

- **Frontend**: Vue 3
- **Build Tool**: Vite
- **Styling**: CSS3 with modern features
- **Deployment**: GitHub Pages

## Development

### Prerequisites

- Node.js (version 16 or higher)
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/yueqianhaobo/personweb.git
cd personweb

# Install dependencies
npm install

# Start development server
npm run dev
```

### Build for Production

```bash
# Build the project
npm run build

# Preview the build
npm run preview
```

## Deployment to GitHub Pages

1. Build the project:
   ```bash
   npm run build
   ```

2. The built files will be in the `dist` directory

3. Deploy to GitHub Pages:
   - Push your code to GitHub
   - Go to repository Settings > Pages
   - Select "Deploy from a branch"
   - Choose the branch containing your built files
   - Set the folder to `/dist` (or configure GitHub Actions for automatic deployment)

## Project Structure

```
personweb/
├── public/
├── src/
│   ├── App.vue          # Main application component
│   ├── main.js          # Application entry point
│   └── style.css        # Global styles
├── index.html           # HTML template
├── package.json         # Project dependencies
├── vite.config.js       # Vite configuration
└── README.md           # Project documentation
```

## Customization

To customize the portfolio for your own use:

1. Update personal information in `src/App.vue`
2. Modify the projects array with your own projects
3. Update social links and contact information
4. Customize colors and styling in the CSS sections

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

- GitHub: [@yueqianhaobo](https://github.com/yueqianhaobo)

---

Built with ❤️ using Vue 3