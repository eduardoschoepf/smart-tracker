# Smart Tracker

A real-time vehicle tracking application that demonstrates the Observer design pattern using React, TypeScript, and interactive mapping.

## 🚀 Features

- Real-time vehicle location tracking
- Interactive map visualization using Leaflet
- Checkpoint detection system
- Route visualization with waypoints
- Live notifications for checkpoint crossings
- Responsive design with Tailwind CSS

## 🏗️ Architecture

The project implements the Observer design pattern with the following components:

- **VehicleTracker (Subject)**: Manages the vehicle's location and notifies observers of changes
- **CheckpointObserver**: Monitors vehicle position and detects checkpoint crossings
- **MapComponent**: Provides real-time visualization of the vehicle's movement and route
- **RoutePoint**: Defines the structure for checkpoints and route coordinates

## 🛠️ Technologies

- React 18
- TypeScript
- Tailwind CSS
- Leaflet Maps
- Lucide Icons
- Vite

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/smart-tracker.git
cd smart-tracker
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

## 🎮 Usage

1. Open the application in your browser
2. Click the "Start Simulation" button to begin the vehicle simulation
3. Watch as the vehicle moves through the predefined route
4. Observe checkpoint notifications as the vehicle passes each waypoint
5. Use the interactive map to view details about checkpoints and the vehicle's current position
6. Click the "Reset" button to restart the simulation

## 🏗️ Project Structure

```
src/
├── components/
│   └── MapComponent.tsx    # Map visualization component
├── models/
│   └── RoutePoint.ts       # Type definitions
├── observers/
│   ├── RouteObserver.ts    # Observer interface
│   └── CheckpointObserver.ts # Checkpoint detection implementation
├── subjects/
│   └── VehicleTracker.ts   # Subject implementation
└── App.tsx                 # Main application component
```

## 🎯 Design Pattern Implementation

The Observer pattern is implemented through:

1. **Subject (VehicleTracker)**
   - Maintains list of observers
   - Notifies observers of location updates
   - Manages vehicle state

2. **Observer (CheckpointObserver)**
   - Registers with the VehicleTracker
   - Receives location updates
   - Detects checkpoint crossings
   - Triggers notifications

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- OpenStreetMap for providing map data
- Leaflet for the mapping library
- React community for excellent tools and libraries
