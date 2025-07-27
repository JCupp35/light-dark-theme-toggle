# Light-Dark Theme Switcher

## Overview
The **Light-Dark Theme Switcher** is a simple React application built with JSX as part of the *Advanced React* course on Coursera. The app demonstrates the use of React Context to manage a global theme state, allowing users to toggle between light and dark themes for a pizza-themed page. The app includes a `Switch` component to toggle themes and uses a `ThemeProvider` and `useTheme` hook to propagate theme state across components without prop drilling.

## Functionality
The app displays a page with a header, title, and paragraph about a pizza-loving family. It includes a switch widget in the top right corner to toggle between light and dark themes. Initially, the app is in "light" theme, with:
- **Header**: "Little Lemon 🍕" title and a theme toggle switch.
- **Content**: A title ("When it comes to dough") and a paragraph about pizza dough.
- **Styling**: White background and black text.

When the user toggles the switch:
- The theme switches between "light" (white background, black text) and "dark" (black background, white text).
- The header, title, and paragraph text colors update accordingly.

This behavior is achieved using React Context in `ThemeContext.js`, where the `ThemeProvider` manages a `theme` state ("light" or "dark") and a `toggleTheme` function, accessible via the `useTheme` hook.

## Project Structure
- **App.jsx**: The main application component, rendering the header and page content with theme-based styling.
- **ThemeContext.jsx**: Defines the `ThemeContext`, `ThemeProvider` component, and `useTheme` hook for managing and accessing the theme state.
- **Switch/index.jsx**: Contains the `Switch` component for toggling the theme.
- **index.jsx**: Entry point for the React application, wrapping the app in `ThemeProvider`.

## Screenshot
![Theme Switcher Output](assets/output.png)

## Technologies Used
- **React**: For building the user interface.
- **JSX**: For writing the component's UI structure.
- **React Context**: For managing global theme state.
- **Create React App**: For the development environment.

## Learning Objectives
This project demonstrates:
- Using React Context to manage global state without prop drilling.
- Creating a custom context provider (`ThemeProvider`) and hook (`useTheme`).
- Handling user interactions with event handlers (e.g., toggling the theme switch).
- Dynamically updating component styles based on state changes.