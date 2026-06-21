# PRODESK-IT-MISSION-10
Movie Explorer is a modern Next.js application that allows users to search, browse, and explore movies using the OMDb API. It features Redux Toolkit state management, advanced filtering, favorites management, responsive UI, movie details modal, and infinite scrolling for a seamless browsing experience.
Movie Explorer
Overview

Movie Explorer is a modern web application built with Next.js that allows users to search, browse, and discover movies using the OMDb API. The application provides an intuitive interface for exploring movie information, managing favorites, and filtering content efficiently.

Features
Search movies by title
View detailed movie information
Infinite scrolling for seamless browsing
Add and remove favorite movies
Responsive user interface
Advanced movie filtering
Global state management using Redux Toolkit
Real-time search functionality
Featured movie section
Favorites dashboard 
Technologies Used
Frontend
Next.js
React
Redux Toolkit
React Redux
Tailwind CSS
API
OMDb API
State Management
Redux Toolkit
React Redux
Project Structure
app/
├── page.jsx
├── layout.jsx
├── globals.css

components/
├── Navbar.jsx
├── MovieCard.jsx
├── MovieModal.jsx
├── SidebarFilters.jsx
├── ActiveFilters.jsx
├── FilteredMovieGrid.jsx

store/
├── store.js
└── slices/
    └── filterSlice.js

lib/
└── omdb.js
Installation
Clone the Repository
git clone <repository-url>
cd movie-explorer
Install Dependencies
npm install
Configure Environment Variables

Create a .env.local file in the project root:

NEXT_PUBLIC_OMDB_API_KEY=your_api_key
Run Development Server
npm run dev

Open:

http://localhost:3000
Build for Production
npm run build
npm start
Application Workflow
The application loads trending movies on startup.
Users can search movies using the search bar.
Search results are fetched from the OMDb API.
Redux Toolkit manages global filter states.
Infinite scrolling loads additional movies automatically.
Users can add movies to favorites.
Favorite movies are stored locally for persistence.
Detailed movie information can be viewed in a modal.
Redux Architecture

The application uses Redux Toolkit for centralized state management.

Store
Global Redux Store
Predictable state updates
Scalable architecture
Filter Slice

Manages:

Search query
Active filters
Filter synchronization
UI filtering state
Performance Optimizations
Infinite scrolling
Debounced search requests
Memoized components
Efficient state updates
Reduced unnecessary re-renders
Lazy data fetching
Future Enhancements
Genre-based filtering
Dark and Light themes
User authentication
Watchlist functionality
Movie recommendations
Pagination controls
Trending and popular movie sections
Movie ratings and reviews
Learning Outcomes

This project demonstrates:

Next.js App Router
Redux Toolkit integration
API consumption
Component-based architecture
State management patterns
Responsive design principles
Infinite scrolling implementation
Performance optimization techniques
Author

Developed as a modern movie discovery platform using Next.js, Redux Toolkit, Tailwind CSS, and the OMDb API.
