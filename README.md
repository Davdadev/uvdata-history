# UV Data History Tracker

A web application that collects and displays UV index data from ARPANSA (Australian Radiation Protection and Nuclear Safety Agency) for multiple locations across Australia.

## Features

- **Real-time Data Collection**: Fetches UV data from ARPANSA's XML API every minute
- **48-Hour History**: Stores UV readings for each location for up to 48 hours
- **Visual Dashboard**: Displays current UV index with color-coded severity levels
- **Historical Charts**: Shows UV trends over time for each location
- **IndexedDB Storage**: Persistent local storage of all collected data
- **Statistics**: Displays aggregate statistics across all locations
- **Data Export**: Export collected data as JSON for further analysis

## Usage

1. Open `index.html` in a modern web browser
2. Click "Start Collection" to begin fetching UV data
3. Data will be automatically collected every minute
4. View real-time UV levels and historical trends for each location
5. Use "Export Data" to download collected data

## UV Index Levels

- **Low (0-2)**: Green - Minimal sun protection required
- **Moderate (3-5)**: Yellow - Some protection required
- **High (6-7)**: Orange - Protection essential
- **Very High (8-10)**: Red - Extra protection needed
- **Extreme (11+)**: Purple - Take all precautions

## Data Source

Data is fetched from: https://uvdata.arpansa.gov.au/xml/uvvalues.xml

## Technical Details

- Pure HTML/CSS/JavaScript implementation (no dependencies)
- Uses IndexedDB for client-side data persistence
- Automatically cleans data older than 48 hours
- Responsive design for desktop and mobile devices

## Browser Support

Requires a modern browser with support for:
- IndexedDB
- Fetch API
- ES6+ JavaScript features