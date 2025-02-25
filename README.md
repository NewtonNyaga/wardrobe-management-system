
# Wardrobe Management System

A simple and efficient system to help you manage your wardrobe, track clothing items, and organize your outfits.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Setup and Installation](#setup-and-installation)
  - [Frontend Setup](#frontend-setup)
  - [Backend Setup](#backend-setup)
- [Running the Application](#running-the-application)
  - [Frontend](#frontend)
  - [Backend](#backend)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This system helps users keep track of their wardrobe items, allowing them to add, remove, and categorize clothes. It also offers features for organizing outfits and keeping notes about each item.

## Technologies Used

- **Frontend**: Vue.js 3, Vue Router
- **Backend**: Laravel 11
- **Database**: MySQL (or any other database you prefer)
- **Authentication**: JWT (JSON Web Tokens)
- **Other Libraries**: Axios, Tailwind CSS (for styling)

## Prerequisites

Before running this system, you need to have the following installed on your local machine:

1. **Node.js** (for the frontend)
2. **NPM or Yarn** (for package management)
3. **PHP** (for the backend)
4. **Composer** (for managing PHP dependencies)
5. **MySQL** (or another database of your choice)

## Setup and Installation

### Frontend Setup

1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```

2. Install dependencies using npm or yarn:
   ```bash
   npm install
   # or
   yarn install
   ```

3. After the installation is complete, you can run the development server:
   ```bash
   npm run serve
   # or
   yarn serve
   ```

4. Visit the app in your browser at `http://localhost:8080`.

### Backend Setup

1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```

2. Install PHP dependencies using Composer:
   ```bash
   composer install
   ```

3. Copy the `.env.example` file to `.env`:
   ```bash
   cp .env.example .env
   ```

4. Set up your database connection in the `.env` file by adjusting the following variables:
   ```ini
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=wardrobe_db
   DB_USERNAME=root
   DB_PASSWORD=yourpassword
   ```

5. Generate the application key:
   ```bash
   php artisan key:generate
   ```

6. Run the database migrations to set up the schema:
   ```bash
   php artisan migrate
   ```

7. You can now run the backend server:
   ```bash
   php artisan serve
   ```

8. Your backend should now be running on `http://localhost:8000`.

## Running the Application

### Frontend

Once the frontend is running, visit the following URL in your browser:

- **Frontend URL**: `http://localhost:8080`

### Backend

To access the backend API, use the following URL:

- **Backend URL**: `http://localhost:8000/api`

Make sure to set up any authentication headers required for the API requests, such as JWT tokens.

## Usage

1. **Add a new item**: Go to the "Add Item" page to add a new clothing item, specifying the type, size, and color.
2. **View wardrobe items**: Browse the list of all clothing items in your wardrobe.
3. **Edit or remove items**: Update the details of an item or delete it from your wardrobe.
4. **Organize outfits**: Create and save outfits for future reference.
5. **Search**: Search for items in your wardrobe by category, type, or other attributes.

## Contributing

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Make your changes and commit them: `git commit -m 'Add new feature'`.
4. Push to your branch: `git push origin feature-name`.
5. Create a pull request.

## License

This project is licensed under the MIT License.


