🎬 Movie Application – README

# Project Overview

This project is a Next.js + TypeScript movie application that integrates with the MoviesDatabase API to fetch and display movie data. The application uses Tailwind CSS, ESLint, and a modular component structure to ensure performance, readability, and scalability.

The goals of this project include:

Understanding and consuming an external API

Designing typed request and response structures

Creating reusable UI components

Implementing a global layout with Header, Footer, and a landing page



---

🌐 API Overview

The MoviesDatabase API offers access to extensive movie and TV show data, including:

Movie and show details

Search functionality

Cast information

Ratings and reviews

Genres and classifications

Images and media metadata

Pagination and filtering options


This API is designed for fast and efficient JSON responses tailored for developers.


---

🏷️ API Version

Current API Version: v1
(Replace with the exact version from the documentation if needed.)


---

🔗 Available Endpoints

Below are commonly used endpoints from the MoviesDatabase API:

Endpoint	Description

/titles	Fetch a list of movies or TV shows
/titles/{id}	Get details of a specific movie or show
/titles/search	Search for titles using keywords
/titles/genres	Retrieve a list of genres
/titles/{id}/cast	Get cast information for a title
/titles/{id}/ratings	Get ratings for a movie or show


(Modify according to the official API documentation.)


---

📥 Request & Response Format

Sample Request

GET /titles/search?title=Inception
Headers:
  X-API-KEY: your_api_key_here

Sample Response

{
  "id": "tt1375666",
  "title": "Inception",
  "year": 2010,
  "genres": ["Action", "Sci-Fi"],
  "rating": 8.8,
  "image": "https://example.com/inception.jpg"
}


---

🔐 Authentication

The MoviesDatabase API requires an API key for most requests.

Authentication Method

Header Method (Recommended):

X-API-KEY: your_api_key_here

Other possible methods (depending on API docs):

Bearer Token Authorization

Query parameter (not recommended due to security risks)


Keep your API key private and store it in environment variables (e.g., .env.local).


---

⚠️ Error Handling

Common API error responses include:

Status Code	Meaning	Reason

400	Bad Request	Invalid or missing parameters
401	Unauthorized	Missing or invalid API key
404	Not Found	The requested resource does not exist
429	Too Many Requests	You exceeded the rate limit
500	Internal Server Error	Server-side API failure


Example Error Response

{
  "error": "Invalid API key",
  "status": 401
}


---

🚦 Usage Limits & Best Practices

To use the API effectively and responsibly:

Follow API rate limits (e.g., 100 requests/min depending on your plan)

Cache requests to improve performance

Implement loading and error UI states

Avoid unnecessary repeated API calls

Store API keys in environment variables (.env.local)

Never commit sensitive keys to GitHub

