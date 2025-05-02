<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="Moodflix is a beginner-friendly React.js movie info platform powered by Appwrite and styled with Tailwind CSS. Browse, search, and discover trending movies effortlessly on any device." />
</head>
<body>
  <h1>Movie DB (Moodflix)</h1>
  <p><strong>Movie Info Website</strong></p>

  <h2>Description</h2>
  <p>
    Movie DB (<em>Moodflix</em>) is a dynamic movie information platform designed to help beginners learn React.js through a real-world project. Leveraging React.js for a fast and interactive UI, Appwrite for a robust backend and trending algorithm, and Tailwind CSS for sleek, responsive styling, Moodflix lets users explore detailed movie data, search titles, and view trending picks in a modern interface.
  </p>

  <h2>Tech Stack</h2>
  <ul>
    <li>React.js</li>
    <li>Appwrite</li>
    <li>Tailwind CSS</li>
  </ul>

  <h2>🔋 Features</h2>
  <ul>
    <li><strong>Browse All Movies:</strong> Explore a wide catalog of films with posters, overviews, and ratings.</li>
    <li><strong>Search Movies:</strong> Quickly find movies by title using a built-in search function.</li>
    <li><strong>Trending Movies Algorithm:</strong> Automatically highlights trending titles based on user interactions and view counts.</li>
    <li><strong>Modern UI/UX:</strong> Clean, intuitive design ensuring a seamless browsing experience.</li>
    <li><strong>Fully Responsive:</strong> Enjoy consistent functionality and layout across desktops, tablets, and mobile devices.</li>
  </ul>

  <h2>Installation</h2>
  <pre><code>git clone https://github.com/PathumSandeepa/Movie-DB.git
cd Movie-DB
npm install
</code></pre>

  <h2>Environment Variables</h2>
  <p>Create a <code>.env.local</code> file in the root directory with the following content:</p>
  <pre><code>VITE_TMDB_API_KEY=***********************
VITE_APPWRITE_PROJECT_ID=***********************
VITE_APPWRITE_DATABASE_ID=***********************
VITE_APPWRITE_COLLECTION_ID=***********************</code></pre>

  <h2>How to Create <code>VITE_TMDB_API_KEY</code></h2>
  <ol>
    <li>Visit <a href="https://www.themoviedb.org/" target="_blank" rel="noopener">TMDB website</a> and sign up.</li>
    <li>Log in and navigate to <a href="https://developer.themoviedb.org/reference/intro/getting-started" target="_blank" rel="noopener">API Documentation → API Preference</a>.</li>
    <li>Copy the <strong>Credentials</strong> header and set it as your <code>VITE_TMDB_API_KEY</code>.</li>
  </ol>

  <h2>Appwrite Setup</h2>
  <ol>
    <li>Go to <a href="https://appwrite.io/" target="_blank" rel="noopener">Appwrite</a> and create an account.</li>
    <li>Create a new project—use the Project ID for <code>VITE_APPWRITE_PROJECT_ID</code>.</li>
    <li>Set up a database—use the Database ID for <code>VITE_APPWRITE_DATABASE_ID</code>.</li>
    <li>Create a collection—use the Collection ID for <code>VITE_APPWRITE_COLLECTION_ID</code>.</li>
  </ol>

  <h2>Collection Attributes</h2>
  <p>Add these attributes in your Appwrite collection to support search tracking and poster display:</p>
  <ul>
    <li><strong>searchTerm</strong> (string, max length: 1000, required)</li>
    <li><strong>count</strong> (integer, default: 1, optional)</li>
    <li><strong>poster_url</strong> (string, max length: 1000, required)</li>
    <li><strong>movie_id</strong> (integer, required)</li>
  </ul>

  <h2>Usage</h2>
  <p>After configuration, start the development server:</p>
  <pre><code>npm run dev</code></pre>

  <h2>License</h2>
  <p>This project has no license.</p>
</body>
</html>
