# Project Architecture

This project follows a modern full-stack architecture with a clear separation between frontend and backend services.

## Project Structure

```
├── Frountend-vite/          # Frontend application
│   ├── src/                # Source code
│   ├── public/             # Static assets
│   └── ...config files     # Configuration files
│
└── Backend-node-mongo/      # Backend application
    ├── src/                # Source code
    ├── Public/             # Static files
    └── ...config files     # Configuration files
```

## Frontend Architecture (Vite + TypeScript)

The frontend is built using:
- **Vite**: A modern build tool for faster development
- **TypeScript**: For type-safe code
- **Tailwind CSS**: For styling
- **ESLint & Prettier**: For code quality and formatting

### Key Features
- Modern development environment with hot module replacement
- Type-safe development with TypeScript
- Utility-first CSS framework with Tailwind
- Code quality tools (ESLint, Prettier)

## Backend Architecture (Node.js + MongoDB)

The backend is built using:
- **Node.js**: JavaScript runtime
- **MongoDB**: NoSQL database
- **Express.js**: Web framework (implied by Node.js backend)

### Key Features
- RESTful API architecture
- MongoDB database integration
- Environment configuration support
- Code formatting with Prettier

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

## Development Guidelines

1. **Code Style**
   - Follow the established ESLint and Prettier configurations
   - Maintain consistent code formatting across the project

2. **TypeScript Usage**
   - Use TypeScript for type safety
   - Define interfaces for data structures
   - Avoid using `any` type when possible

3. **API Development**
   - Follow RESTful conventions
   - Document API endpoints
   - Implement proper error handling

4. **Database**
   - Follow MongoDB best practices
   - Implement proper data validation
   - Use indexes for better performance



### 1. Update All Dependencies
You can update all the dependencies in your project using npm-check-updates:

Install npm-check-updates globally:

```bash
 
npm install -g npm-check-updates
```
Check for outdated dependencies: Run this command in your project folder:

```bash
ncu
```
This will display a list of outdated packages and their latest versions.



Upgrade all dependencies: To update the package.json with the latest versions, run:
```bash
ncu -u
````

Install updated dependencies: After updating package.json, install the updated packages:
```bash
npm install
```

### 2: Use --force or --legacy-peer-deps
If you need React 19 and are okay with potential issues:
```bash
npm install --force
```
Or:
```bash
npm install --legacy-peer-deps
```
These options allow npm to bypass the dependency conflict. However, be cautious as this might cause runtime issues.
