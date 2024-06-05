Book Search and Personal Bookshelf Application
Introduction
This project involves creating a React application that allows users to search for books using the Open Library API and maintain a personal bookshelf in the browser using localStorage. The application consists of two main pages: a Book Search page and a Personal Bookshelf page. This application demonstrates the usage of various React and web development concepts, including API integration, state management, and local storage. Additionally, it showcases best practices in responsive design and deployment.

Project Structure
The project is organized into several key components and files, each serving a specific purpose:

App.js: The main application file that sets up routing using react-router-dom.
components/BookSearch.js: A component that handles searching for books and displaying the search results.
components/Bookshelf.js: A component that displays the user's personal bookshelf.
App.css: The CSS file that contains styling for the application, ensuring responsiveness and a clean layout.
index.js: The entry point of the React application.
README.md: The documentation file that provides setup instructions, usage guidelines, and project details.
Key Features
1. Book Search Functionality
The Book Search page allows users to search for books by typing in a query. As the user types, the application fetches search results in real-time using the Open Library API. The search results are displayed in a list of cards, with each card representing a book result. Users can add books from the search results to their personal bookshelf.

Implementation Details
Input Field: An input field is provided for the user to type in the book's name. The query state is updated as the user types.
API Integration: The Open Library API is used to fetch search results. The API endpoint is https://openlibrary.org/search.json?q=YOUR_QUERY&limit=10&page=1, where YOUR_QUERY is the search term entered by the user.
Real-time Search: The search is performed in real-time using the useEffect hook to fetch data whenever the query state changes. If the query is empty, the search results are cleared.
Display Results: The search results are displayed in a list of cards. Each card includes the book's title, author, and a button to add the book to the personal bookshelf.
