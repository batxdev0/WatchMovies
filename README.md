# Movie Search App 🎬

🚀 **[Live Demo](https://watchmovies-suit.onrender.com)** — See the project in action!

A modern, responsive React application that helps you discover and search through thousands of movies. Built with React 19, Vite, and Tailwind CSS, this app provides an intuitive interface for movie discovery with real-time search capabilities and trending movie tracking.

## ✨ Features

- **🔍 Real-time Movie Search**: Search through thousands of movies with debounced API calls
- **📊 Trending Movies**: View the most searched movies based on user activity
- **🎨 Modern UI**: Beautiful, responsive design with Tailwind CSS
- **⚡ Fast Performance**: Built with Vite for lightning-fast development and builds
- **📱 Mobile Responsive**: Optimized for all device sizes
- **⭐ Movie Details**: View ratings, release dates, and language information
- **🔄 Search Analytics**: Track popular searches using Appwrite backend

## 🛠️ Tech Stack

- **Frontend**: React 19, Vite
- **Styling**: Tailwind CSS 4
- **Backend**: Appwrite (Database & Analytics)
- **API**: The Movie Database (TMDB) API
- **State Management**: React Hooks
- **Utilities**: react-use (for debouncing)

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- Appwrite account
- TMDB API key

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd my-first-react-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   
   Create a `.env` file in the root directory and add your API keys:
   ```env
   VITE_TMDB_API_KEY=your_tmdb_api_key_here
   VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
   VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
   VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
   ```

4. **Get API Keys**
   
   - **TMDB API Key**: Sign up at [The Movie Database](https://www.themoviedb.org/settings/api) and get your API key
   - **Appwrite Setup**: 
     - Create an Appwrite project
     - Create a database with a collection for search analytics
     - Add the required environment variables

5. **Run the development server**
   ```bash
   npm run dev
   ```

6. **Open your browser**
   
   Navigate to `http://localhost:5173` to view the application

## 🌐 Deployment

### Render Deployment (Recommended)

This project is configured for easy deployment on Render.

#### Automatic Deployment on Render

1. **Push your code to GitHub**
   ```bash
   git add .
   git commit -m "Add Render deployment configuration"
   git push origin main
   ```

2. **Connect to Render**
   - Go to [Render Dashboard](https://dashboard.render.com/)
   - Click "New +" and select "Static Site"
   - Connect your GitHub repository
   - Configure the following settings:
     - **Name**: `watchmovies-app` (or your preferred name)
     - **Build Command**: `npm install && npm run build`
     - **Publish Directory**: `dist`
     - **Branch**: `main`

3. **Set Environment Variables**
   In the Render dashboard, add these environment variables:
   - `VITE_TMDB_API_KEY`
   - `VITE_APPWRITE_PROJECT_ID`
   - `VITE_APPWRITE_DATABASE_ID`
   - `VITE_APPWRITE_COLLECTION_ID`

#### Important Notes for Deployment

- **Environment Variables**: All environment variables must be set for the build to work
- **CORS Issues**: If you encounter CORS issues, ensure your API keys are properly configured

## 🎯 How It Works

### Search Functionality
- Users can search for movies using the search bar
- Search is debounced (500ms delay) to prevent excessive API calls
- Results are fetched from TMDB API in real-time
- Search analytics are tracked in Appwrite database

### Movie Display
- Each movie shows:
  - Movie poster
  - Title
  - Rating (with star icon)
  - Original language
  - Release year

## 🔧 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint
- `npm run deploy` - Deploy to GitHub Pages

## 🌟 Key Features Explained

### Debounced Search
The app uses `react-use` library to debounce search input, preventing excessive API calls while users type.

### Responsive Design
Built with Tailwind CSS for a mobile-first, responsive design that works on all devices.

### Error Handling
Comprehensive error handling for API failures and network issues with user-friendly error messages.

### Performance Optimization
- Lazy loading of images
- Debounced API calls
- Efficient state management with React hooks

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- [The Movie Database (TMDB)](https://www.themoviedb.org/) for providing the movie data API
- [Appwrite](https://appwrite.io/) for backend services
- [Vite](https://vitejs.dev/) for the build tool
- [Tailwind CSS](https://tailwindcss.com/) for styling


---

**Happy Movie Searching! 🎬✨**
