# Movie Search App 🎬

A React-based application that allows users to search for movies using the OMDB API and watch their trailers via YouTube API integration.

## Features

- 🔍 Search for movies by title
- 🎥 View movie posters and details
- ▶️ Watch movie trailers using YouTube API
- 📱 Responsive design for mobile and desktop
- 🎨 Beautiful UI with gradient backgrounds and smooth animations

## Project Structure

```
pro_slo/
├── public/
│   └── index.html
├── src/
│   ├── App.js
│   ├── index.js
│   ├── MovieSearch.js
│   └── MovieSearch.css
├── package.json
├── .env
└── README.md
```

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn

## Installation

1. Navigate to the project directory:
```bash
cd pro_slo
```

2. Install dependencies:
```bash
npm install
```

## Configuration

### Step 1: Get OMDB API Key
1. Visit [OMDB API](http://www.omdbapi.com/apikey.aspx)
2. Request a free API key
3. The key provided: `539035` (already configured in `.env`)

### Step 2: Get YouTube API Key
1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project
3. Enable the YouTube Data API v3
4. Create an API key (OAuth or API key)
5. Add your YouTube API key to the `.env` file:

```
REACT_APP_OMDB_API_KEY=539035
REACT_APP_YOUTUBE_API_KEY=YOUR_YOUTUBE_API_KEY_HERE
```

## Running the Application

Start the development server:
```bash
npm start
```

The application will open in your browser at `http://localhost:3000`

## Usage

1. Enter a movie title in the search box
2. Click "Search" or press Enter
3. View the search results with movie posters and details
4. Click "Watch Trailer" to see the movie's trailer on YouTube
5. Close the trailer modal by clicking the X button

## API Limits

- **OMDB API**: Free tier allows up to 1,000 requests per day
- **YouTube API**: Free tier has a quota of 10,000 units per day

## Important Notes

- Ensure both API keys are valid and have the correct rate limits configured
- Some movies may not have trailers available on YouTube
- Image posters are provided by OMDB when available
- The app uses HTTP for OMDB (ensure your browser allows mixed content if running on HTTPS)

## Technologies Used

- **React** - UI library
- **Axios** - HTTP client for API requests
- **OMDB API** - Movie database
- **YouTube API v3** - Video search and embedding
- **CSS3** - Styling with animations and gradients

## License

This project is open source and available for personal and educational use.

## Support

For issues or questions:
1. Check your API keys are correctly added to `.env`
2. Verify you have internet connection
3. Check browser console for error messages
4. Ensure your API keys have sufficient quota remaining
