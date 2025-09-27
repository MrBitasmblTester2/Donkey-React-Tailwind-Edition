# Donkey-React-Tailwind-Edition

Description: Build a professional, simple 2D Donkey Kong–style platform game using React for UI and Tailwind CSS for responsive styling. The project features multiple levels, character movement with jumping, collision detection, and animation loops, demonstrating clean code structure, state management with React hooks, and best practices.

## Tech Stack
- React
- Tailwind CSS

## Requirements
- Character movement and jumping controls (Use keyboard event listeners and update position state inside useEffect.)
- Collision detection with platforms and barrels (Compute bounding boxes and detect overlaps.)
- Multiple levels with increasing difficulty (Store level data as an array and increment level state on completion.)
- Use React functional components and hooks (Leverage useState and useEffect for component logic.)
- Responsive styling with Tailwind CSS (Use Tailwind utility classes for layout and design.)
- Add sound effects with Web Audio API (Play sounds on events using the Audio API.)

## Installation
1. Clone the repository:
   bash
   git clone https://github.com/your-username/Donkey-React-Tailwind-Edition.git
   cd Donkey-React-Tailwind-Edition
   
2. Install dependencies:
   bash
   npm install
   
3. (Optional) Create a `.env` file to configure environment variables (e.g., audio asset paths):
   env
   REACT_APP_AUDIO_BASE_URL=/assets/audio
   

## Usage
Start the development server:
bash
npm start

Open `http://localhost:3000` in your browser. Use keyboard arrow keys for movement and spacebar to jump. Progress through levels and enjoy the game.

## Implementation Steps
1. Initialize a new React project and install Tailwind CSS:
   bash
   npx create-react-app .
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init -p
   
2. Configure `tailwind.config.js` and include Tailwind directives in `src/index.css`.
3. Create core components: `GameBoard`, `Player`, `Platform`, and `Barrel`.
4. Manage game state with `useState` for player position, velocity, and current level.
5. Add keyboard event listeners inside `useEffect` to handle movement and jumping controls.
6. Implement collision detection by computing bounding boxes and checking overlaps between player, platforms, and barrels.
7. Store level data (platform positions, barrel spawn points) in an array and update level state on completion.
8. Create a game loop using `requestAnimationFrame` in a custom hook to update positions and render frames.
9. Style the game layout and components using Tailwind CSS utility classes for responsiveness.
10. Load and play sound effects using the Web Audio API upon player actions and collisions.
11. Test across different screen sizes to ensure responsive behavior.

(Optional) ## API Endpoints
This project does not expose external API endpoints.