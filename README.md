# Oxford-Styled YouTube Analytics Dashboard

A sophisticated YouTube analytics tracking web application with a clean, professional interface inspired by Oxford University's visual identity. The application enables content creators to record, analyze, and export detailed performance metrics for their YouTube videos.

## Features

- **Authentication System**: Secure user registration, login, and password recovery
- **Video Management**: Form-based data entry for comprehensive YouTube video metrics
- **Analytics Dashboard**: Summary view with performance trends, comparative analysis, and visualizations
- **Data Export**: Multiple format options (CSV, JSON, Excel) with batch export capability and AI-ready formatting
- **Responsive Design**: Optimized for all devices with an Oxford-inspired aesthetic

## Technology Stack

- **Frontend**: React with TypeScript, Redux Toolkit for state management
- **Styling**: Tailwind CSS with custom Oxford branding configuration
- **Visualizations**: Recharts and Chart.js for data visualization
- **Backend**: Node.js with Express (separate repository)
- **Database**: PostgreSQL for data storage, Redis for caching
- **Authentication**: JWT-based authentication

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/oxford-youtube-analytics.git
   cd oxford-youtube-analytics
   ```

2. Install dependencies:
   ```bash
   npm install
   ```
   
3. Create a `.env` file in the root directory with the following variables:
   ```
   REACT_APP_API_URL=http://localhost:5000/api
   ```

4. Start the development server:
   ```bash
   npm start
   ```

5. The application will be available at `http://localhost:3000`

### Building for Production

```bash
npm run build
```

### Running with Docker

If you prefer using Docker, you can build and run the application using Docker Compose:

```bash
docker-compose up -d
```

This will start the frontend, backend, PostgreSQL database, and Redis cache in separate containers.

## Project Structure

```
oxford-youtube-analytics/
├── client/                      # Frontend application
│   ├── public/                  # Static assets
│   ├── src/
│   │   ├── api/                 # API integration layer
│   │   ├── assets/              # Frontend assets
│   │   ├── components/          # Reusable UI components
│   │   ├── context/             # React context providers
│   │   ├── hooks/               # Custom React hooks
│   │   ├── pages/               # Page components
│   │   ├── redux/               # Redux state management
│   │   ├── services/            # Service modules
│   │   ├── styles/              # Global styles
│   │   ├── types/               # TypeScript type definitions
│   │   ├── utils/               # Utility functions
│   │   ├── App.tsx              # Main application component
│   │   └── index.tsx            # Application entry point
├── server/                      # Backend application (separate repository)
├── .env.example                 # Example environment variables
├── .gitignore                   # Git ignore file
├── docker-compose.yml           # Docker Compose configuration
├── Dockerfile                   # Docker configuration
└── README.md                    # Project documentation
```

## Development

### Code Style

This project uses ESLint and Prettier for code formatting. You can run the linter with:

```bash
npm run lint
```

Or to automatically fix issues:

```bash
npm run lint:fix
```

## Deployment

The application can be deployed to any hosting service that supports static websites, such as:

- Vercel
- Netlify
- AWS S3 + CloudFront
- GitHub Pages

For the backend, you'll need a Node.js hosting environment such as:

- Heroku
- AWS Elastic Beanstalk
- Digital Ocean
- Google Cloud Run

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- Oxford University for the visual identity inspiration
- [Tailwind CSS](https://tailwindcss.com/) for the utility-first CSS framework
- [Recharts](https://recharts.org/) for the charting library
- [Redux Toolkit](https://redux-toolkit.js.org/) for state management
