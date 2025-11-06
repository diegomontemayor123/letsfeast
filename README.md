# LetsFeast - Social Recipe Sharing Platform

## Overview

LetsFeast is a social platform for sharing and discovering user-generated recipes, built as a mobile app prototype. It enables users to explore a variety of home-cooked meals, share their own recipes, interact with others through likes, comments, and direct messages, and create personalized feeds. With a modern, engaging UI and real-time features, LetsFeast aims to build an organic community of food lovers.

## Features

* **User-Generated Recipes**: Share your own recipes, discover new ones, and save your favorites.
* **Likes and Bookmarks**: Users can like or bookmark recipes to save them for later.
* **Comments and Conversations**: Threaded comments allow users to interact with recipe creators and fellow food enthusiasts.
* **Direct Messaging**: Private messaging between users with recipe previews and images shared.
* **Real-Time Feed Filtering**: Personalized recipe feeds that update in real-time, based on your interactions and preferences.
* **Push Notifications**: Real-time alerts for new messages, recipe updates, and community interactions.
* **Image Uploads**: Share photos of your culinary creations with your recipes.
* **User Avatars**: Personalize your profile with an avatar for a more engaging community experience.

## Tech Stack

* **Frontend**: React Native – A modular, efficient mobile framework for building the app's UI and handling interactive components like likes, comments, and image uploads.
* **Backend**: Node.js & Express – A robust backend built with Express.js for API management, user authentication (JWT), and data validation (Joi).
* **Database**: MongoDB – A NoSQL database to store user profiles, recipes, likes, comments, messages, and other social interactions.
* **Authentication**: JWT (JSON Web Tokens) – For secure, stateless authentication across sessions.
* **Real-time Messaging**: Push notifications for user interactions and messaging.
* **Validation**: Joi – A schema-based validation library to ensure user inputs are correctly formatted and secure.

## Installation

### Prerequisites

* Node.js (v14 or higher)
* MongoDB (local or MongoDB Atlas)
* React Native development environment (with Android Studio or Xcode)

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/diegomontemayor123/letsfeast.git
   cd letsfeast
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Set up your MongoDB instance:

   * If you're using MongoDB Atlas, create a cluster and obtain your connection string.
   * If you're using a local MongoDB instance, make sure it's running.

4. Create a `.env` file in the root directory and add the following variables:

   ```bash
   MONGO_URI=<Your MongoDB Connection String>
   JWT_SECRET=<Your JWT Secret>
   ```

5. Start the backend server:

   ```bash
   npm run dev
   ```

6. For the React Native app, follow the [React Native setup guide](https://reactnative.dev/docs/environment-setup) based on your platform (Android or iOS), then start the app:

   ```bash
   npx react-native run-android  # For Android
   npx react-native run-ios      # For iOS
   ```

## Backend Architecture

* **Node.js/Express**: Handles API requests, user authentication, and routing.
* **MongoDB**: Stores all application data including user accounts, recipes, likes, comments, and messages.
* **JWT Authentication**: Secures API endpoints by issuing and verifying JSON Web Tokens for user sessions.

## Frontend Architecture

* **React Native**: Cross-platform mobile framework used for building the app’s interface. The app is designed to be responsive, with real-time updates for interactions.
* **React Navigation**: Used for navigating between different screens like home, recipe detail, messaging, and profile.
* **Redux**: Manages application state for user preferences, likes, and the real-time feed.

## Features in Development

* **User Profile Customization**: Enhance the user profile with bio, favorite recipes, and social media integrations.
* **Advanced Recipe Search**: Filtering recipes by cuisine, difficulty level, cooking time, and more.
* **Social Features**: Introduce the ability to follow other users and receive updates on their new recipe posts.

## How to Contribute

1. Fork the repository.
2. Create a new branch for your feature (`git checkout -b feature/feature-name`).
3. Make your changes and commit (`git commit -m 'Add feature'`).
4. Push to your branch (`git push origin feature/feature-name`).
5. Open a Pull Request.

Please ensure your changes are well-documented and that the app remains functional with your new features.

## License

All rights reserved. This project is proprietary and may not be used, modified, or distributed without permission from the author.
