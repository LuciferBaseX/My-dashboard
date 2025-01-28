Doqfy Dashboard

A modern, responsive dashboard built with Next.js 14, TypeScript, and Tailwind CSS. This dashboard provides a clean interface for managing contracts, e-stamps, and e-signs with real-time statistics and progress tracking.

Dashboard Preview
🚀 Features

    📱 Fully responsive design
    💳 Wallet balance tracking
    📊 Real-time order statistics
    📈 Progress tracking with circular charts
    🎨 Modern UI with purple accent theme
    🔔 Notification system
    📱 Mobile-friendly navigation

🛠️ Tech Stack

    Next.js 14 - React Framework
    TypeScript - Type Safety
    Tailwind CSS - Styling
    Lucide Icons - Icons
    Radix UI - UI Components

📦 Installation

    Clone the repository:

git clone https://github.com/yourusername/doqfy-dashboard.git

    Navigate to the project directory:

cd doqfy-dashboard

    Install dependencies:

npm install

    Run the development server:

npm run dev

    Open http://localhost:3000 in your browser.

📁 Project Structure

doqfy-dashboard/
├── app/
│   ├── components/
│   │   ├── header.tsx
│   │   ├── welcome-card.tsx
│   │   ├── service-card.tsx
│   │   ├── order-stats.tsx
│   │   ├── progress-charts.tsx
│   │   └── ui/
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── public/
├── tailwind.config.js
└── package.json

🧩 Components
Header

The main navigation component containing:

    Logo
    Navigation links
    Notification bell
    User avatar

WelcomeCard

Displays:

    Welcome message
    Current date
    Wallet balance
    Low balance notification

ServiceCard

Reusable component for service displays:

    Title
    Description
    "Get started" action button

OrderStats

Shows order statistics including:

    Total Orders
    In Progress
    Completed Orders
    Cancelled Orders

ProgressCharts

Circular progress indicators for:

    E-sign Count
    E-stamp Count

🎨 Styling

The application uses Tailwind CSS with a custom configuration:

// tailwind.config.js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "app/**/*.{ts,tsx}",
    "components/**/*.{ts,tsx}",
  ],
  theme: {
    extend: {
      colors: {
        'purple-primary': 'var(--purple-primary)',
        'purple-light': 'var(--purple-light)',
      }
    }
  }
}

📱 Responsive Design

The dashboard is fully responsive with breakpoints:

    Mobile: < 768px
    Tablet: 768px - 1024px
    Desktop: > 1024px

🔧 Configuration
Environment Variables

No environment variables are required for basic setup.
Custom Styling

Global styles are defined in app/globals.css:

:root {
  --purple-primary: #7C3AED;
  --purple-light: #9461FF;
}

🚀 Deployment
Deploy to Vercel

    Push your code to GitHub
    Import your repository to Vercel
    Deploy

Manual Deployment

Build the application:

npm run build

🤝 Contributing

    Fork the repository
    Create your feature branch:

git checkout -b feature/AmazingFeature

    Commit your changes:

git commit -m 'Add some AmazingFeature'

    Push to the branch:

git push origin feature/AmazingFeature

    Open a Pull Request

📝 Component API
ServiceCard

interface ServiceCardProps {
  title: string;
  description: string;
}

ProgressChart

interface ProgressChartProps {
  title: string;
  percentage: number;
  subtitle?: string;
}

📈 Performance Optimization

The dashboard implements several performance optimizations:

    Component-level code splitting
    Optimized images
    Minimal CSS with Tailwind
    Server-side rendering with Next.js

🔒 Security

    All external links use rel="noopener noreferrer"
    No sensitive data exposed in client-side code
    Type-safe props with TypeScript

📱 Mobile Features

    Responsive navigation
    Touch-friendly interface
    Optimized for various screen sizes
    Mobile-first design approach

🌐 Browser Support

    Chrome (latest)
    Firefox (latest)
    Safari (latest)
    Edge (latest)

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.
👥 Authors

    Your Name - Initial work

🙏 Acknowledgments

    Design inspiration from modern dashboard interfaces
    Icons from Lucide React
    UI components from Radix UI

🐛 Known Issues

Currently, there are no known issues. If you find any, please create an issue in the repository.
🔜 Future Enhancements

    Dark mode support
    More interactive charts
    Additional dashboard widgets
    User settings panel
    Enhanced mobile features
