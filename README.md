# Packing List App

A simple and interactive React application for creating, managing, and organizing a packing list. The app allows users to add items, mark items as packed, sort items based on different criteria, and track the packing progress.

## Table of Contents

- [Demo](#demo)
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Components Overview](#components-overview)
- [Styling](#styling)


## Features

- Add items to the packing list with specified quantities.
- Mark items as packed or unpacked.
- Sort items by input order, description, or packed status.
- Clear the entire list with a single click.
- Displays statistics on packing progress.

## Project Structure

```
src/
├── components/
│   ├── App.js           # Main application component
│   ├── Logo.js          # Header logo
│   ├── Form.js          # Form to add new items
│   ├── PackingList.js   # Component for displaying and sorting items
│   ├── Item.js          # Single item component with delete and toggle functions
│   └── Stats.js         # Packing progress statistics
├── index.js             # Entry point for React
├── index.css            # Styling for the app
└── README.md            # Project documentation
```

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd packing-list-app
   ```
3. Install dependencies:
   ```bash
   npm install
   ```

## Usage

Start the application:
```bash
npm start
```

Open [http://localhost:3000](http://localhost:3000) in a web browser to use the app.

## Components Overview

### `App.js`

The main component that renders the app layout. It manages the state for the packing list items and includes functions for adding, deleting, and toggling items.

### `Logo.js`

Displays the app's title with a tropical and travel-themed logo.

### `Form.js`

A form that allows users to add new items to the packing list. Includes a text input for the item description and a dropdown for the quantity. When the form is submitted, a new item object is created and added to the list.

### `PackingList.js`

Displays the list of items. This component allows sorting by input order, description, or packed status. It also includes a "Clear list" button to remove all items.

### `Item.js`

Represents an individual item on the packing list. Allows users to mark the item as packed/unpacked with a checkbox or delete it from the list.

### `Stats.js`

Shows statistics on packing progress, such as the total number of items and the percentage of items packed.

## Styling

The app is styled with a tropical theme, giving it a vibrant and playful look. Font styles are imported from Google Fonts.

### Key CSS Classes

- `.app`: Main app container.
- `.add-form`: Styles the form for adding items.
- `.list`: Styles the packing list area.
- `.stats`: Styles the footer for displaying packing statistics.
