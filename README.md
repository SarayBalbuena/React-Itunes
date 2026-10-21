# React iTunes 🎵

A small React app for searching albums in the iTunes catalog. Type an artist or album name and it fetches matching albums from the public [iTunes Search API](https://performance-partners.apple.com/search-api), showing them with high-resolution cover art.

## Features

- **Album search:** queries `itunes.apple.com/search` and returns up to 20 albums
- **Grid or list view:** switch layouts from the search bar
- **Loading, empty and error states:** spinners and feedback messages for each status
- **Component tests:** Jest, Enzyme and React Testing Library

## Tech stack

- React 16 (class components + PropTypes)
- Create React App
- Font Awesome icons
- react-spinkit for loading indicators

## Project structure

```
src/
├── App.js                  # State, iTunes API call, layout
└── components/
    ├── Searcher/           # Search input + grid/list toggle
    ├── Button/             # Search button with loading spinner
    ├── Card/               # Album cover, artist and title
    └── FeedbackMessage/    # Init / loading / no results / error messages
```

## Getting started

```bash
npm install
npm start      # http://localhost:3000
npm test       # run the test suite
npm run build  # production build in /build
```
