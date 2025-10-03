# X4: Foundations - Nyra Database & Utilities

A comprehensive web application for **X4: Foundations** game data, featuring an advanced station calculator, database browser, and utilities to help players plan and optimize their gameplay.

🌐 **Official Game:** [www.x4-game.com](http://www.x4-game.com)

## 📋 Overview

This Angular-based web application provides an interactive interface for browsing and analyzing X4: Foundations game data, including ships, equipment, modules, wares, factions, and races. The centerpiece is a powerful station calculator that helps players design and optimize their space stations.

## ✨ Features

### 🏭 Station Calculator (Primary Feature)
- **Interactive Station Planning**: Design and configure custom space stations
- **Module Selection**: Browse and add production modules to your station
- **Resource Management**: Calculate resource inputs/outputs and production chains
- **Cost Analysis**: Estimate build costs and material requirements
- **Import/Export Plans**: Save and share station configurations
- **Layout Management**: Save, load, and share station layouts

### 🗃️ Database Browser
- **Ships Database**: Complete catalog of all ships with detailed specifications
- **Equipment Browser**: Comprehensive equipment and component listings
- **Module Database**: All station modules with production capabilities
- **Wares Catalog**: Full inventory of tradeable items and resources
- **Factions**: Information about game factions
- **Races**: Details about different races in the X4 universe

### 🎨 User Interface
- **Modern Design**: Clean, responsive UI built with Bootstrap 5
- **Dark Theme**: DevExtreme dark theme for comfortable extended use
- **Advanced Components**: Professional data grids and interactive elements
- **Mobile Responsive**: Optimized for various screen sizes

## 🛠️ Technology Stack

### Frontend Framework
- **Angular 15.2**: Modern TypeScript-based framework
- **TypeScript 4.9**: Strong typing and modern JavaScript features
- **RxJS 7.8**: Reactive programming for async operations

### UI Libraries
- **Bootstrap 5.3**: Responsive layout and component styling
- **DevExtreme 22.2**: Advanced data grid and UI components
- **ng-bootstrap 14.1**: Bootstrap components for Angular
- **Font Awesome 4.7**: Icon library

### Additional Tools
- **Google Analytics**: Usage tracking and analytics
- **i18n Support**: Internationalization with support for multiple languages (English, Chinese)
- **XML Processing**: `xml-js` for data parsing
- **URLON**: URL encoding for sharing configurations

## 📁 Project Structure

```
x4-Nyra/
├── src/
│   ├── app/
│   │   ├── station/              # Station calculator (main feature)
│   │   │   ├── components/
│   │   │   │   ├── station-calculator/
│   │   │   │   ├── station-modules/
│   │   │   │   ├── station-resources/
│   │   │   │   ├── station-summary/
│   │   │   │   └── import-export/
│   │   │   └── services/
│   │   ├── ship/                 # Ships database module
│   │   ├── equipment/            # Equipment browser
│   │   ├── module/               # Modules catalog
│   │   ├── ware/                 # Wares database
│   │   ├── faction/              # Factions information
│   │   ├── races/                # Races information
│   │   ├── shared/               # Shared services and components
│   │   │   ├── services/
│   │   │   │   ├── data/        # Game data files
│   │   │   │   ├── *.service.ts # Entity services
│   │   │   │   └── model/       # Data models
│   │   │   └── components/
│   │   ├── core/                 # Core module
│   │   └── google-analytics/     # Analytics integration
│   ├── assets/
│   │   ├── icons/               # Race and ware icons
│   │   ├── images/              # X4 logo and graphics
│   │   └── styles/              # Additional styles and fonts
│   ├── environments/            # Environment configurations
│   └── i18n/                    # Internationalization files
├── docs/                        # Production build output
└── angular.json                 # Angular configuration
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher recommended)
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd x4-Nyra/x4-Nyra
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run development server**
   ```bash
   npm start
   ```
   Navigate to `http://localhost:4200/` in your browser.

### Build

**Development build:**
```bash
npm run build
```

**Production build:**
```bash
npm run build -- --configuration production
```

The build artifacts will be stored in the `dist/` directory.

**Watch mode** (auto-rebuild on file changes):
```bash
npm run watch
```

## 🎮 Usage

### Station Calculator
1. Navigate to the **Station Calculator** (default landing page)
2. Add production modules from the module browser
3. Configure module quantities and production settings
4. Review resource requirements in the summary panel
5. Save or share your station design using the export feature

### Database Browser
- Use the navigation menu to browse different categories
- Search and filter items using the data grid controls
- Click on items for detailed information

## 🌍 Internationalization

The application supports multiple languages:
- English (en-US)
- Chinese Simplified (zh-Hans)

Translation files are located in `src/i18n/`.

## 📦 Module Architecture

The application uses Angular's lazy loading feature for optimal performance:
- Each major feature (ships, equipment, modules, etc.) is a separate module
- Modules are loaded on-demand when navigated to
- Shared services and components are centralized in the `shared` module

## 🎨 Styling

- **SCSS**: Used for component-specific styling
- **Bootstrap 5**: Grid system and utility classes
- **DevExtreme Dark Theme**: Primary UI theme
- **Font Awesome**: Icons throughout the application

## 🔧 Configuration

### Angular Configuration (`angular.json`)
- Output path: `dist/x4-new`
- Style preprocessor: SCSS
- Asset handling for icons, images, and fonts
- Production optimizations enabled

### Build Budgets
- Initial bundle: 2MB max
- Component styles: 4KB max

## 🤝 Contributing

This is an open-source project. Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

**GitHub Repository**: [github.com/crissian/x4](https://github.com/crissian/x4)

## 📄 License

This project is open source. Please refer to the repository for license details.

## 🎯 Roadmap & Future Enhancements

Potential areas for improvement:
- [ ] Real-time station profitability calculations
- [ ] Integration with latest X4 DLC data
- [ ] Advanced production chain optimization
- [ ] Fleet calculator
- [ ] Trade route planner
- [ ] Additional language support

## 🐛 Known Issues

Please report issues on the GitHub repository issue tracker.

## 📞 Contact & Support

For questions, suggestions, or support:
- Open an issue on GitHub
- Check existing documentation
- Review the About page in the application

---

**Made for X4: Foundations players by the community** 🚀
