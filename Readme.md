# Project Aether: Meshtastic Blackout Strategy

![Status](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Overview

Project Aether is an interactive educational web application that analyzes and visualizes the viability of **Meshtastic (LoRa)** mesh networks as a decentralized communication solution during catastrophic grid failures and natural disasters.

When traditional infrastructure fails, centralized networks collapse within hours. This application demonstrates how mesh networking provides a resilient, community-driven emergency communication layer.

## 🚀 Features

### 1. **Executive Briefing**
- Clear presentation of the problem: centralized network failure during disasters
- Real-time status dashboard with key metrics (frequency bands, cost, battery life)
- Visual comparison of centralized vs. mesh solutions

### 2. **Comparative Technology Analysis**
- **Radar Chart**: Multi-axis comparison of technologies (Meshtastic, Ham Radio, Cellular, Satellite)
- **Battery Life Visualization**: Bar chart showing runtime comparison across different systems
- **Detailed Comparison Table**: Side-by-side analysis of range, infrastructure needs, skill level, and cost

### 3. **Interactive Mesh Topology Simulator**
- Real-time Canvas-based visualization of mesh networking
- Click to add relay nodes and see how messages "hop" through the network
- Visual connectivity status indicator
- Demonstrates the core concept of decentralized mesh networking without external dependencies

### 4. **Deployment Calculator**
- Interactive range estimation based on:
  - Environment density (urban, suburban, rural, mountain)
  - Antenna quality (stock, upgraded, base station)
  - Elevation/height above terrain
- Real-time mesh hop calculations
- Personalized deployment recommendations

## 🛠️ Technical Stack

- **Frontend**: Pure HTML5, CSS3 (Tailwind CSS via CDN)
- **Visualization**: Chart.js for radar and bar charts
- **Animation**: Native HTML5 Canvas for mesh simulation
- **Typography**: Inter & JetBrains Mono (Google Fonts)
- **No build tools required** - runs directly in browser

## 📊 Data Visualizations

1. **Resilience Radar Chart**: 6-axis comparison across Range, Battery Efficiency, Cost, Ease of Use, Off-Grid Ability, and Privacy
2. **Energy Independence Bar Chart**: Battery runtime comparison on 3000mAh battery
3. **Mesh Network Simulator**: Real-time animated topology with BFS connectivity checking
4. **Range Calculator**: Physics-based estimation using terrain and antenna parameters

## 🎨 Design Philosophy

- **Color Palette**: Warm neutrals (Stone/Orange) for a "field manual" aesthetic
- **Responsive Layout**: Mobile-first design with Tailwind utility classes
- **Accessibility**: High contrast, readable fonts, clear visual hierarchies
- **Performance**: Lightweight, no heavy frameworks, optimized Canvas rendering

## 🚦 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No server required - runs as a static HTML file

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Aether-Projects/Project-One.git
cd Project-One
```

2. Open the application:
```bash
open index.html
# or simply double-click index.html in your file browser
```

### Usage

1. **Navigate** through sections using the sticky navigation bar
2. **Interact** with the Mesh Simulator by clicking to add relay nodes
3. **Adjust** deployment parameters in the calculator to see real-time estimates
4. **Compare** technologies using the visual charts and data table

## 📐 Architecture

```
index.html
├── Navigation (Sticky Top Bar)
├── Section 1: Executive Summary
│   ├── Problem Statement
│   └── Status Dashboard
├── Section 2: Comparative Analysis
│   ├── Radar Chart (Chart.js)
│   ├── Battery Bar Chart (Chart.js)
│   └── Comparison Table
├── Section 3: Mesh Logic Simulator
│   ├── Canvas Animation
│   └── BFS Connectivity Algorithm
└── Section 4: Deployment Calculator
    ├── Environment Selector
    ├── Antenna Quality Radio Buttons
    └── Elevation Slider with Real-time Calculations
```

## 🔬 Key Algorithms

### Range Estimation
```javascript
Range = BaseKm × EnvironmentFactor × AntennaFactor × log(Height + 1) × 0.8
```

### Mesh Coverage Calculation
```javascript
NodesNeeded = CityArea / (π × Range²)
```

### Connectivity Check
- Breadth-First Search (BFS) to determine if source can reach target through relay nodes
- Connection threshold: 150 pixels (representing ~range distance)

## 📱 Responsive Breakpoints

- **Mobile**: < 768px (stacked layout, simplified tables)
- **Tablet**: 768px - 1024px (2-column grids)
- **Desktop**: > 1024px (3-column layouts, full charts)

## 🎯 Use Cases

- **Emergency Preparedness**: Understanding backup communication options
- **Community Planning**: Calculating mesh network coverage for neighborhoods
- **Education**: Teaching mesh networking concepts interactively
- **Disaster Response**: Evaluating technology options for crisis scenarios

## 🔮 Future Enhancements

- [ ] Add real-world terrain data integration
- [ ] Export deployment plans as PDF
- [ ] Multi-language support
- [ ] Cost calculator for bulk purchases
- [ ] Integration with actual Meshtastic API for live data

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- **Meshtastic Project**: Open-source mesh networking firmware
- **LoRa Technology**: Semtech for long-range radio modulation
- **Chart.js**: Beautiful, responsive charts
- **Tailwind CSS**: Utility-first CSS framework

## 📞 Contact

Project Link: [https://github.com/Aether-Projects/Project-One](https://github.com/Aether-Projects/Project-One)

---

**Note**: This is an educational simulation. Actual deployment scenarios require professional RF planning and compliance with local regulations (FCC Part 15 in USA, CE in Europe, etc.).
