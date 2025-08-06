# Movie Discovery App

This is a simple, single-page web app for discovering movies using The Movie Database (TMDB) API. It helps users filter through popular movies by genres, moods, keywords, actors, and year ranges to find something to watch. Features include favoriting movies, skipping seen ones, viewing trailers in a modal, and getting recommendations via TasteDive.

The app is designed for personal use on desktop or mobile, with infinite scrolling for more results and a dark theme for easy viewing.

## Features
- **Movie List**: Shows popular movies sorted by popularity, with posters, overviews, ratings, and options to favorite or skip.
- **Filters**: Modal for selecting genres, moods (predefined or custom keywords), movie/actor search, and year range.
- **Trailer Modal**: Click a poster to play the official trailer (if available) in a responsive modal.
- **Recommendations**: Click a movie title for similar suggestions.
- **TMDB Integration**: Syncs favorites and skipped movies to your TMDB account (requires login via TMDB's secure redirect).
- **Undo Skip**: Reverse the last skip action.
- **Clear Filters**: Reset all filters and reload.

## Setup
1. **Get API Keys**:
   - Sign up for a free TMDB account at [themoviedb.org](https://www.themoviedb.org/signup) and get an API key from [settings/api](https://www.themoviedb.org/settings/api).
   - Sign up for a free TasteDive API key at [tastedive.com/api](https://tastedive.com/api).

2. **Edit the Code**:
   - Open `index.html` in a text editor.
   - Replace `YOUR_TMDB_API_KEY_HERE` with your TMDB key: `const apiKey = 'YOUR_TMDB_API_KEY_HERE';`
   - Replace `YOUR_TASTEDIVE_API_KEY_HERE` with your TasteDive key: `const tasteDiveKey = 'YOUR_TASTEDIVE_API_KEY_HERE';`
   - Save the file.

3. **Run Locally**:
   - Open `index.html` in any modern browser (e.g., Chrome, Firefox).
   - If prompted, log in to TMDB for full features (favorites/skipped sync).
   - Use the "Filters" button to set preferences, then browse movies.

## Hosting on GitHub Pages
1. **Create a Repository**:
   - Go to [github.com](https://github.com) and create a new public repository (e.g., "movie-discovery-app").

2. **Upload Files**:
   - Upload `index.html` (with your API keys inserted) to the repo's root.

3. **Enable GitHub Pages**:
   - In the repo, go to Settings > Pages.
   - Under "Source," select "Deploy from a branch," choose the "main" branch, and set the folder to "/ (root)".
   - Save. GitHub will provide a URL like `https://yourusername.github.io/movie-discovery-app/`.

4. **Access the App**:
   - Visit the URL in a browser.
   - Share the link with others—they'll need to insert their own API keys if forking/editing, but the hosted version uses yours (consider making it a template repo for others to fork).

## Notes
- **Privacy**: The app uses localStorage for filters and TMDB session—clear browser data to reset.
- **Limitations**: Relies on TMDB/TasteDive APIs (free tiers have rate limits). No server-side backend, so all data is client-side.
- **Customization**: Feel free to tweak styles or add features; it's pure HTML/JS.
- **Issues**: If trailers don't load or APIs fail, check console errors (e.g., invalid keys). Report bugs via GitHub issues.

Enjoy discovering movies!
