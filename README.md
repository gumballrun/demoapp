# Gumball Run

A multiplayer web-based game designed to teach users about the beneficial speed/accuracy tradeoff that comes from assisted estimation. Through gameplay, users experience first-hand the net benefit that comes when the speed of estimation is increased at the expense of a small reduction in accuracy .

## Purpose

Gumball Run is an educational game that demonstrates the practical advantages of estimation over precise calculation in time-sensitive scenarios. Players learn that:

- **Speed matters**: Quick estimates often provide sufficient accuracy for decision-making
- **Accuracy has diminishing returns**: Perfect precision may not be worth the time cost
- **Context is key**: Understanding when "good enough" is actually better than "perfect"

By playing the game, users develop an intuitive understanding of the speed/accuracy tradeoff and learn to make better decisions about when to use estimation versus precise calculation.

## Features

- **Real-time multiplayer gameplay** with Firebase integration
- **Interactive 3D gumball machine** built with Three.js and React Three Fiber
- **Particle physics simulation** for realistic gumball pouring
- **Live leaderboards** and team statistics
- **Responsive design** that works on desktop and mobile
- **Room-based multiplayer** with easy sharing via URLs

## Installation

### Prerequisites

- Node.js (version 16 or higher)
- npm or yarn package manager

### Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd gumball-run
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up Firebase**
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/)
   - Enable Realtime Database
   - Copy your Firebase configuration
   - Create a `.env` file in the root directory:
     ```env
     VITE_FIREBASE_API_KEY=your_api_key
     VITE_FIREBASE_AUTH_DOMAIN=your_auth_domain
     VITE_FIREBASE_DATABASE_URL=your_database_url
     VITE_FIREBASE_PROJECT_ID=your_project_id
     VITE_FIREBASE_STORAGE_BUCKET=your_storage_bucket
     VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
     VITE_FIREBASE_APP_ID=your_app_id
     ```

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:5173` to see the application.

### Building for Production

```bash
npm run build
```

The built files will be in the `dist` directory, ready for deployment.

## How to Use

### Multiplayer Setup

Gumball Run is designed to be played by multiple users simultaneously:

1. **First Player (Game Host)**:
   - Open the application in your browser
   - Click "Start New Game" or "Create Room"
   - Copy the room link/URL that appears
   - Share this URL with other players

2. **Additional Players**:
   - Use the shared room link to join the game
   - Enter your name when prompted
   - Wait for the game to start

### Gameplay

- **Objective**: Estimate the number of gumballs in the machine as quickly and accurately as possible
- **Scoring**: Balance speed and accuracy to achieve the highest score
- **Multiplayer**: Compete against other players in real-time
- **Leaderboards**: Track your performance across multiple games

## Technology Stack

- **Frontend**: React 19 with Vite
- **3D Graphics**: Three.js with React Three Fiber
- **Styling**: Tailwind CSS
- **Backend**: Firebase Realtime Database
- **Routing**: React Router DOM
- **Build Tool**: Vite

## Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Project Structure

```
src/
├── components/          # React components
├── lib/                 # Utility libraries (Firebase, room management)
├── routes/              # Page components
└── assets/              # Static assets
```

## Deployment

The application is configured for deployment on Netlify with the included `netlify.toml` configuration file. Simply connect your repository to Netlify for automatic deployments.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is private and proprietary.

## Support

For questions or issues, please contact the development team.