# Movie Explorer

## Description

Movie Explorer is a modern movie discovery web application built with Next.js, Redux Toolkit, and Tailwind CSS. It allows users to search movies, view detailed information, manage favorites, apply filters, and enjoy a smooth browsing experience through infinite scrolling. The application fetches real-time movie data from the OMDb API and provides a responsive and user-friendly interface.

---

## Features

- Search movies using OMDb API
- View detailed movie information
- Infinite scrolling for continuous browsing
- Add and remove favorite movies
- Redux Toolkit state management
- Advanced filtering system
- Responsive design
- Featured movie section
- Real-time search functionality
- Persistent favorites using Local Storage

---

## Tech Stack

### Frontend
- Next.js
- React
- Tailwind CSS

### State Management
- Redux Toolkit
- React Redux

### API
- OMDb API

---

## Project Structure

```bash
movie-explorer/
│
├── app/
│   ├── page.jsx
│   ├── layout.jsx
│   └── globals.css
│
├── components/
│   ├── Navbar.jsx
│   ├── MovieCard.jsx
│   ├── MovieModal.jsx
│   ├── SidebarFilters.jsx
│   ├── ActiveFilters.jsx
│   └── FilteredMovieGrid.jsx
│
├── store/
│   ├── store.js
│   └── slices/
│       └── filterSlice.js
│
├── lib/
│   └── omdb.js
│
├── public/
│
├── .env.local
├── package.json
└── README.md
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/movie-explorer.git
cd movie-explorer
```

### Install Dependencies

```bash
npm install
```

### Environment Variables

Create a `.env.local` file in the root directory:

```env
NEXT_PUBLIC_OMDB_API_KEY=YOUR_OMDB_API_KEY
```

Get your free API key from:

https://www.omdbapi.com/apikey.aspx

### Run Development Server

```bash
npm run dev
```

Open:

```bash
http://localhost:3000
```

---

## Build for Production

```bash
npm run build
npm start
```

---

## Redux Toolkit Implementation

The application uses Redux Toolkit to manage global state efficiently.

### Filter Slice

Stores:

- Search query
- Active filters
- Filter state synchronization

### Benefits

- Predictable state management
- Centralized data flow
- Better scalability
- Improved maintainability

---

## Infinite Scrolling

Infinite scrolling is implemented using the Intersection Observer API.

### Workflow

1. User scrolls down the page
2. Observer detects the bottom loader element
3. Next page of movies is requested
4. New movies are appended to existing results
5. Process continues until no more results are available

---

## Performance Optimizations

- Debounced search input
- Redux state management
- Infinite scrolling
- Memoized callbacks using useCallback
- Reduced unnecessary re-renders
- Efficient API requests

---

## Future Improvements

- Dark and Light Theme Toggle
- Genre-Based Filtering
- Watchlist Functionality
- Movie Recommendations
- User Authentication
- Movie Ratings and Reviews
- Trending and Popular Sections

---

## Learning Outcomes

This project demonstrates:

- Next.js App Router
- React Hooks
- Redux Toolkit
- API Integration
- Infinite Scrolling
- State Management
- Component Architecture
- Responsive UI Design
- Performance Optimization

---

## Author

Swobhagya Sahoo

B.Tech Computer Science and Engineering (Artificial Intelligence)

Institute of Aeronautical Engineering

---

## License

This project is developed for educational and portfolio purposes.
