# Fetch - Dog Shelter Adoption App

Welcome to the Fetch Dog Shelter Adoption App! This is a Next.js application that helps dog lovers search through a database of shelter dogs, with the goal of finding a dog a new home. The app allows users to authenticate, browse available dogs, filter search results, favorite dogs, and generate a match based on their favorites.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)

## Features

- **User Authentication**: Users can sign in using their name and email.
- **Dog Search**: Browse and filter shelter dogs by breed, age, and zip code.
- **Dog Favorites**: Add dogs to a favorites list for later.
- **Match Generation**: After browsing, generate a match based on the dogs added to your favorites.
- **Responsive UI**: The UI is responsive and user-friendly, optimized for all screen sizes.

## Tech Stack

- **Next.js**: A React framework for building static and dynamic websites.
- **TypeScript**: A typed superset of JavaScript for better developer experience.
- **Tailwind CSS**: A utility-first CSS framework for rapid UI development.
- **Axios**: Used for making HTTP requests to the backend API.
- **ShadCN**: For including components in the UI.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/codeWithGhufran/fe-app-test.git
    ```

2. Install the dependencies:
    ```bash
    npm install
    ```

## Usage

1. Start the development server:
    ```bash
    npm run dev
    ```

2. Open [http://localhost:3000](http://localhost:3000) in your browser to see the app in action.

3. **Authentication**: On the login page, enter your name and email, and submit the form to authenticate.

4. **Browse Dogs**: Once authenticated, you can start browsing available dogs. You can filter by breed, age, and zip code. Dogs will be listed in alphabetical order by breed by default.

5. **Favorites**: Add dogs to your favorites list by clicking the heart icon on each dog card.

6. **Match Generation**: Once you've added dogs to your favorites, click the "Generate Match" button to get a match based on your selected dogs.

## API Endpoints

The app uses the following API endpoints to fetch data:

### Authentication
- **POST /auth/login**: Authenticate user with name and email.
- **POST /auth/logout**: Log out the user and invalidate the auth cookie.

### Dog Search & Data
- **GET /dogs/breeds**: Fetch a list of available dog breeds.
- **GET /dogs/search**: Fetch search results based on breed, age, and zip code.
- **POST /dogs**: Fetch detailed information of a list of dogs.
- **POST /dogs/match**: Generate a match based on favorited dogs.
