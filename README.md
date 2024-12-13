## General Overview

This project is a Django-based web application for a movie website. It features a range of functionalities typical of modern web platforms.

### 1. Site Architecture and Navigation

The website comprises several pages:
- **Most Watched Movies Page**: Showcasing the most popular movies.
- **Home Page**: The central hub of the site.
- **Category Pages**: Dedicated to different genres.
- **Individual Movie Detail Pages**: For detailed information about each movie.
- **User Profile Pages**: For user-specific information and settings.

Navigation through the website is facilitated by a navbar and sidebars on various pages.

### 2. Authentication

- **Signup**: Users can sign up via the 'Become a Member' section in the navbar, which redirects them to the signup page. Post-registration, users are directed to the login screen.
- **Viewing Movies**: Movies can be viewed by any visitor without the need for registration.
- **Commenting**: To comment on movies, users must sign up and log in.
- **Visibility of Comments**: Unregistered users can view comments but cannot see the comment section on movie detail pages.
- **Profile Access**: All users, regardless of login status, can view individual user profiles.
- **Profile Editing**: Logged-in users can edit their profiles, including avatars, information, and social links.

### 3. Database

- The project utilizes the movie API provided by [The Movie Database (TMDB)](https://www.themoviedb.org/).
- A custom database can be created and utilized following the structure defined in the `models.py` file under `movie_app`.

**If you want to use TheMovieDB Database for the project, you need to get the api key from their original site in the above**

### 4. Search Functionality

The site's search functionality operates based on movie titles. It performs a case-insensitive search across the database and returns results, implementing pagination for queries yielding more than 20 results.

### 5. Homepage

The homepage features the six most popular movies and a paginated list of the latest 20 movies. The movies are sorted from newest to oldest in the database and displayed accordingly on the homepage.

### 6. Categories

Each category page displays only the movies belonging to that specific genre, showing the latest 20 movies in a paginated format.

### 7. Most Popular Movies

This page ranks movies based on the 'popularity' metric from TMDB, showing them from most to least popular. Pagination is active, displaying 20 movies per page.

### 8. Profile (Account)

After signing up and logging in, each user has a personal profile page based on their username. Users can update their information, change their password, or delete their account. Profile customization options include changing the avatar, adding a biography, and including social media links.

In profile detail pages people can see user's latest comments (paginated), their social links and bio + avatar.# moviesite
