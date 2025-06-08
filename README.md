# Project Architecture

This project follows a modern full-stack architecture with a clear separation between frontend and backend services.

## Project Structure

```
├── Frountend-vite/          # Frontend application
│   ├── src/                # Source code
│   │   ├── app/           # Main application code
│   │   ├── assets/        # Static assets (images, fonts, etc.)
│   │   ├── components/    # Reusable UI components
│   │   ├── hooks/         # Custom React hooks
│   │   ├── services/      # API services and external integrations
│   │   ├── store/         # State management (Redux/Context)
│   │   ├── styles/        # Global styles and CSS modules
│   │   └── utils/         # Utility functions and helpers
│   ├── public/            # Public static files
│   └── ...config files    # Configuration files
│
└── Backend-node-mongo/      # Backend application
    ├── src/                # Source code
    │   ├── controllers/    # Request handlers and business logic
    │   ├── db/            # Database configuration and models
    │   ├── middlewares/   # Express middlewares
    │   ├── models/        # MongoDB schemas and models
    │   ├── routes/        # API route definitions
    │   └── utils/         # Utility functions and helpers
    ├── Public/            # Static files served by the backend
    └── ...config files    # Configuration files
```

## Detailed Folder Structure

### Frontend Structure (`Frountend-vite/src/`)

- **app/**: Contains the main application code, including pages and layouts
- **assets/**: Stores static files like images, fonts, and other media
- **components/**: Reusable UI components that can be shared across the application
- **hooks/**: Custom React hooks for shared logic and state management
- **services/**: API integration and external service connections
- **store/**: State management logic (Redux store, context providers)
- **styles/**: Global styles, CSS modules, and theme configurations
- **utils/**: Helper functions, constants, and utility methods

### Backend Structure (`Backend-node-mongo/src/`)

- **controllers/**: Contains the business logic and request handlers
- **db/**: Database configuration, connection setup, and initialization
- **middlewares/**: Express middleware functions (auth, validation, etc.)
- **models/**: MongoDB schemas and data models
- **routes/**: API route definitions and endpoint configurations
- **utils/**: Helper functions and utility methods
- **Public/**: Static files served directly by the backend server

## Technology Stack

### Frontend (Vite + TypeScript)
- **Vite**: A modern build tool for faster development
- **TypeScript**: For type-safe code
- **Tailwind CSS**: For styling
- **ESLint & Prettier**: For code quality and formatting

### Backend (Node.js + MongoDB)
- **Node.js**: JavaScript runtime
- **MongoDB**: NoSQL database
- **Express.js**: Web framework

## Development Setup

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd Frountend-vite
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start development server:
   ```bash
   npm run dev
   ```

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd Backend-node-mongo
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Configure environment variables:
   - Copy `.env.sample` to `.env`
   - Update the environment variables as needed
4. Start the server:
   ```bash
   npm start
   ```

## Dependency Management

### Updating Dependencies
1. Install npm-check-updates globally:
   ```bash
   npm install -g npm-check-updates
   ```
2. Check for outdated dependencies:
   ```bash
   ncu
   ```
3. Update package.json with latest versions:
   ```bash
   ncu -u
   ```
4. Install updated dependencies:
   ```bash
   npm install
   ```

### Handling Dependency Conflicts
If you encounter dependency conflicts (e.g., with React 19), you can use one of these approaches:

1. Force install (use with caution):
   ```bash
   npm install --force
   ```
2. Use legacy peer dependencies:
   ```bash
   npm install --legacy-peer-deps
   ```

> **Note**: Using `--force` or `--legacy-peer-deps` might cause runtime issues. Use these options only when necessary and test thoroughly.

## Development Guidelines

### Code Style
- Follow the established ESLint and Prettier configurations
- Maintain consistent code formatting across the project

### TypeScript Usage
- Use TypeScript for type safety
- Define interfaces for data structures
- Avoid using `any` type when possible

### API Development
- Follow RESTful conventions
- Document API endpoints
- Implement proper error handling

### Database
- Follow MongoDB best practices
- Implement proper data validation
- Use indexes for better performance

## Contributing

1. Create a new branch for your feature
2. Follow the established code style
3. Write meaningful commit messages
4. Test your changes thoroughly
5. Submit a pull request

## License

[Add your license information here]
