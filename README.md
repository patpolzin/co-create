
# Co-Create - Telegram Mini App

A collaborative canvas application built for Telegram Mini Apps. Co-Create allows teams to collaborate in real-time with sticky notes, drawings, text, shapes, arrows, and images on an infinite canvas.

## Features

- 🎨 **Infinite Canvas** - Unlimited space for creativity
- 👥 **Real-time Collaboration** - Work together with your team instantly
- ✨ **AI-Powered Insights** - Smart summaries and idea organization
- 🗳️ **Voting Mode** - Vote on ideas and prioritize
- 📱 **Mobile & Desktop** - Optimized for both mobile and desktop Telegram clients
- 🎯 **Telegram Integration** - Native Telegram Web App SDK integration

## Tech Stack

- **React 18** with TypeScript
- **Vite** for build tooling
- **Tailwind CSS** for styling
- **Radix UI** components
- **Telegram Web App SDK** for Telegram integration

## Development

### Prerequisites

- Node.js 18+ and npm/yarn/pnpm

### Setup

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

The app will be available at `http://localhost:3000`

### Building for Production

```bash
npm run build
```

The production build will be in the `dist/` directory.

### Preview Production Build

```bash
npm run preview
```

## Deployment to Telegram

### 1. Build the Application

```bash
npm run build
```

### 2. Deploy to Hosting

Deploy the `dist/` folder to a static hosting service:
- **Vercel**: `vercel --prod`
- **Netlify**: Drag and drop the `dist` folder
- **GitHub Pages**: Configure GitHub Actions
- **Cloudflare Pages**: Connect your repository
- Any static hosting service

### 3. Configure Telegram Bot

1. Create a bot with [@BotFather](https://t.me/botfather) on Telegram
2. Use `/newapp` command to create a new Mini App
3. Provide the URL where your app is hosted (must be HTTPS)
4. Set the app name, description, and icon
5. Configure additional settings as needed

### 4. Telegram Mini App Requirements

- ✅ HTTPS required (no HTTP)
- ✅ Valid SSL certificate
- ✅ Accessible from Telegram clients
- ✅ Proper viewport meta tags (already configured)
- ✅ Telegram Web App SDK script (already included)

### 5. Testing

- Test in Telegram Desktop, iOS, and Android clients
- Use Telegram's test mode for development
- Verify safe area insets work correctly on mobile devices

## Project Structure

```
├── src/
│   ├── components/      # React components
│   ├── hooks/           # Custom React hooks
│   ├── lib/             # Utilities and Telegram integration
│   ├── styles/          # Global styles
│   └── App.tsx          # Main application component
├── index.html           # HTML entry point
├── vite.config.ts       # Vite configuration
└── package.json         # Dependencies and scripts
```

## Telegram Integration

The app includes full Telegram Web App SDK integration:

- **User Authentication**: Automatically gets Telegram user info
- **Theme Support**: Adapts to Telegram's theme (light/dark)
- **Haptic Feedback**: Native vibration feedback on interactions
- **Share to Chat**: Send canvas data back to Telegram chat
- **Safe Areas**: Proper handling of device safe areas (notches, etc.)

## Environment Variables

No environment variables are required for basic functionality. The app works both in Telegram and standalone mode.

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Telegram Desktop (Windows, macOS, Linux)
- Telegram Mobile (iOS, Android)
- Web browsers (for development/testing)

## License

Private project - All rights reserved

## Support

For issues or questions, please contact the development team.
  