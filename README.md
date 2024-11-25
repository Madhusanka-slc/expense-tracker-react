# Expense Tracker

A simple expense tracker built with ReactJS, Vite, and Tailwind CSS. This app allows users to track their income and expenses, maintain a balance, and view a history of transactions.

## Features

- **Balance**: Displays your current balance, calculated from income and expenses.
- **Income and Expenses**: Shows the total income and total expenses.
- **Transaction History**: Tracks individual transactions with the amount and description (e.g., salary, book purchase).
- **Add Transaction**: Allows the user to add new transactions (income or expense).

## Project Setup

To run the project locally, follow these steps:

### Prerequisites

Make sure you have the following installed:

- **Node.js** (preferably the latest LTS version)
- **npm** (comes with Node.js)
- **Vite** (for quick development environment setup)
- **Tailwind CSS** (for utility-first styling)

### Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>


2. **Navigate to the project folder**:
   ```bash
   cd expense-tracker-react
   ```

3. **Install dependencies**:
   ```bash
   npm install
   ```

4. **Install Tailwind CSS**:
   If not already installed, follow these steps to set up Tailwind CSS:
   ```bash
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init
   ```
   Add the following to your `tailwind.config.js` file:
   ```js
   module.exports = {
     content: [
       "./index.html",
       "./src/**/*.{js,jsx,ts,tsx}",
     ],
     theme: {
       extend: {},
     },
     plugins: [],
   };
   ```

   Create a `src/index.css` file and add the following lines to import Tailwind's default styles:
   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```

   Ensure `index.css` is imported in your `src/main.jsx` file:
   ```js
   import './index.css';
   ```

### Running the Project

1. **Start the development server**:
   ```bash
   npm run dev
   ```

2. Open your browser and go to `http://localhost:5173` to view the app.

## How to Use

- **Add a Transaction**: Enter the text (e.g., "Salary", "Flower", etc.) and the amount (positive for income, negative for expenses).
- **View Balance**: The app automatically updates the balance based on the transactions.
- **Transaction History**: All added transactions will appear in the history with the amount (either positive for income or negative for expense).

## Technologies Used

- **ReactJS**: Front-end JavaScript library for building user interfaces.
- **Vite**: Fast development build tool for ReactJS applications.
- **Tailwind CSS**: A utility-first CSS framework for creating custom designs.
- **CSS**: Styling for the user interface.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
