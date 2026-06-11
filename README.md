# AquaVest - Smart Rainwater Harvesting Solution

AquaVest is an intelligent web application that helps users calculate their rainwater harvesting potential, design optimal water storage solutions, and understand the economic benefits of rainwater conservation. Built with Next.js, TypeScript, and Google Genkit AI.

## 🌊 Overview

AquaVest enables users to:
- Calculate rainwater harvesting potential based on roof area, location, and rainfall data
- Get AI-powered recommendations for water storage tank sizing
- Analyze cost-benefit scenarios for water conservation
- Simulate real-time rainfall data using IoT-like sensors
- Generate comprehensive PDF reports with harvesting analysis
- Support for multiple languages (English, Hindi, Tamil)

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ and npm
- A Google AI API key (for Genkit integration)
- Modern web browser

### Installation

```bash
# Clone or navigate to project directory
cd "path/to/rain water harvesting"

# Install dependencies
npm install

# Create .env.local file with your API keys
echo "NEXT_PUBLIC_FIREBASE_API_KEY=your_key_here" > .env.local
echo "GENKIT_API_KEY=your_genkit_key_here" >> .env.local
```

### Development

```bash
# Run the development server
npm run dev

# In another terminal, start Genkit AI with watch mode
npm run genkit:watch
```

The application will be available at `http://localhost:3000`

## 📁 Project Structure

```
src/
├── ai/                          # Genkit AI integration
│   ├── genkit.ts               # Genkit configuration
│   └── dev.ts                  # Development server
├── app/                         # Next.js app directory
│   ├── layout.tsx              # Root layout
│   ├── page.tsx                # Home/main page
│   ├── admin/                  # Admin dashboard
│   ├── login/                  # Authentication pages
│   ├── signup/
│   ├── forgot-password/
│   ├── settings/               # User settings
│   ├── report/                 # Report generation
│   └── iot-connect/            # IoT integration
├── components/
│   ├── aquavest/               # Feature components
│   │   ├── input-form.tsx
│   │   ├── results-dashboard.tsx
│   │   ├── cost-benefit-chart.tsx
│   │   ├── annual-potential-chart.tsx
│   │   ├── water-savings-pie-chart.tsx
│   │   └── iot-simulation-card.tsx
│   ├── ui/                     # Reusable UI components
│   └── layout/                 # Layout components
├── contexts/                   # React contexts
│   ├── language-context.tsx
│   └── theme-builder-context.tsx
├── hooks/                      # Custom React hooks
├── lib/                        # Utilities and config
│   ├── firebase-config.ts
│   ├── types.ts
│   ├── data.ts
│   └── utils.ts
└── locales/                    # Internationalization
    ├── en.json
    ├── hi.json
    └── ta.json
```

## 🎨 Features

### Core Functionality
- **Rainwater Harvesting Calculator**: Computes potential runoff using the formula: Runoff = Rainfall × Area × 0.85
- **Smart Tank Sizing**: AI-powered recommendations for optimal water storage
- **Cost-Benefit Analysis**: Financial projections for water conservation investments
- **IoT Simulation**: Simulates real-time rainfall sensor data for visualization
- **Report Generation**: Export comprehensive PDF reports

### User Experience
- **Multi-language Support**: English, Hindi, Tamil
- **Dark/Light Theme**: Toggle themes for comfortable viewing
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Real-time Visualizations**: Interactive charts and dashboards
- **User Authentication**: Login/signup with password recovery

### Design
- **Primary Color**: Deep Blue (#3F51B5) - represents water and reliability
- **Background**: Light Blue (#E3F2FD) - clean and refreshing
- **Accent**: Green (#4CAF50) - sustainability and calls to action
- **Typography**: PT Sans - modern, humanist sans-serif
- **Icons**: Clean line-art style for intuitive navigation

## 🛠️ Tech Stack

- **Frontend**: Next.js 15, React 18, TypeScript
- **Styling**: Tailwind CSS, Shadcn/ui components
- **AI/ML**: Google Genkit, Google AI models
- **Backend**: Firebase, Next.js API routes
- **Authentication**: Firebase Authentication
- **State Management**: React Contexts
- **UI Library**: Radix UI components
- **Internationalization**: JSON locale files

## 📦 Available Scripts

```bash
# Development
npm run dev                 # Start dev server
npm run genkit:dev        # Start Genkit development server
npm run genkit:watch      # Start Genkit with file watching

# Production
npm run build             # Build for production
npm start                 # Start production server

# Quality & Maintenance
npm run lint              # Run ESLint
npm run typecheck         # Check TypeScript types
npm audit fix             # Fix security vulnerabilities
```

## 🔌 Environment Variables

Create a `.env.local` file in the root directory:

```env
# Firebase Configuration
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id

# Genkit/AI Configuration
GENKIT_API_KEY=your_genkit_api_key
NEXT_PUBLIC_GOOGLE_AI_API_KEY=your_google_ai_key
```

## 🔐 Authentication

- Users can sign up with email and password
- Password recovery via email
- Session management through Firebase Auth
- Protected routes for authenticated features

## 📊 Data Visualization

- Annual rainwater potential charts
- Cost-benefit analysis pie charts
- Water savings projections
- Real-time rainfall simulation graphs

## 🌐 Multi-language Support

The application automatically detects and supports:
- **English** (en)
- **Hindi** (hi)
- **Tamil** (ta)

Switch languages in the settings menu.

## 🚀 Deployment

### Build for Production

```bash
npm run build
npm start
```

### Deploy to Firebase Hosting

```bash
firebase deploy
```

The project includes `apphosting.yaml` and Firebase configuration for cloud deployment.

## 📝 License

This project is part of the AquaVest rainwater harvesting initiative.

## 🤝 Contributing

To contribute:
1. Create a feature branch (`git checkout -b feature/amazing-feature`)
2. Commit your changes (`git commit -m 'Add amazing feature'`)
3. Push to the branch (`git push origin feature/amazing-feature`)
4. Open a Pull Request

## 🐛 Troubleshooting

### "next is not recognized"
```bash
# Install dependencies first
npm install
```

### Port 3000 already in use
```bash
# Use a different port
npm run dev -- -p 3001
```

### API Key errors
- Ensure `.env.local` file exists with correct API keys
- Restart the dev server after updating environment variables

## 📚 Documentation

- See `docs/blueprint.md` for detailed feature specifications
- Check individual component files for implementation details

## 🎯 Roadmap

- [ ] Advanced IoT sensor integration
- [ ] Mobile app (React Native)
- [ ] Government policy recommendations
- [ ] Community data sharing
- [ ] AI-powered maintenance alerts
- [ ] Integration with water utility providers

## 📞 Support

For issues or questions, please open an issue in the repository or contact the development team.
