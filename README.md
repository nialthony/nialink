# Social Media Links Landing Page

## Project Structure
```
social-media-links/
│
├── public/
│   ├── index.html
│   └── favicon.ico
│
├── src/
│   ├── components/
│   │   └── SocialMediaLinks.js
│   ├── styles/
│   │   └── index.css
│   ├── App.js
│   └── index.js
│
├── package.json
├── tailwind.config.js
├── postcss.config.js
└── README.md
```

## package.json
```json
{
  "name": "social-media-links",
  "version": "1.0.0",
  "private": true,
  "dependencies": {
    "@tailwindcss/forms": "^0.5.7",
    "@tailwindcss/typography": "^0.5.10",
    "lucide-react": "^0.294.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "tailwind-scrollbar-hide": "^1.1.7"
  },
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
  "devDependencies": {
    "tailwindcss": "^3.4.0",
    "postcss": "^8.4.32",
    "react-scripts": "^5.0.1"
  }
}
```

## README.md
```markdown
# Social Media Links Landing Page

## Setup Instructions
1. Clone the repository
2. Run \`npm install\`
3. Run \`npm start\`

## Features
- Responsive design
- Dark mode toggle
- Animated social media links
- Tailwind CSS styling
```

## src/index.js
```jsx
import React from 'react';
import ReactDOM from 'react-dom/client';
import './styles/index.css';
import App from './App';

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
```

## src/App.js
```jsx
import React from 'react';
import SocialMediaLinks from './components/SocialMediaLinks';

function App() {
  return <SocialMediaLinks />;
}

export default App;
```

## src/styles/index.css
```css
@tailwind base;
@tailwind components;
@tailwind utilities;

body {
  @apply transition-colors duration-300;
}

.dark-mode {
  @apply bg-gray-900 text-white;
}
```

## public/index.html
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Social Media Links</title>
  </head>
  <body>
    <div id="root"></div>
  </body>
</html>
```
