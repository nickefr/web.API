# web.API
# FRONT-END DEVELOPMENT

## Film Finder

You’ve caught up on your list of TV shows and movies and want to get recommendations for what to watch next, but aren’t sure where to look. In this project, you’ll use your knowledge of HTTP requests and asynchronous JavaScript to create a movie discovery app that will recommend random movies by genre. You’ll be able to choose from several genres, and like or dislike a movie to get another suggestion.

Before you begin, you’ll need to create an account on The Movie Database website. After you create your account and verify your email address, click on your user icon at the top right corner and navigate to the Settings page.



On the Settings page, navigate to the API section and click on the link to Request an API Key to register as a Developer.

You’ll be asked to enter some personal information like your address and phone number. This is pretty common. Many APIs use this information to keep track of how their data is being used. As a part of your registration, you will also be asked to provide a URL for the site where you will be using this API. Here, you can list "https://codecademy.com". Check out these instructions if you need further assistance with registering for an API key.

After you finish this project, feel free to challenge yourself to continue building it out. For example, you might recommend TV shows instead of movies, or change the information you present about the recommended movies. The possibilities are endless. Next time you find yourself needing new content recommendations, you’ll know where to turn!

If you get stuck during this project or would like to see an experienced developer work through it, click “Get Unstuck“ to see a project walkthrough video.

### Tasks
- [ ] Populate Drop-down Menu with Genres
- [ ] Get a Random Movie
- [ ] Get Movie Info
- [ ] Display Movie

---

### Populate Drop-down Menu with Genres


## 1. Save the TMDB API Key
- Obtain an API key from the TMDB API and store it in the `tmdbKey` variable for authentication.

## 2. Define TMDB Base URL
- Set the TMDB API base URL and save it to the `tmdbBaseUrl` variable.

## 3. Fetch Genres from TMDB API
- Inside `getGenres()`, set `genreRequestEndpoint` to the "Genres" API endpoint.

## 4. Add Query Parameters for Genre Request
- Create `requestParams` in `getGenres()` with `api_key` parameter set to `tmdbKey`.

## 5. Construct URL for Genres Request
- Combine base URL, genre endpoint, and parameters to form `urlToFetch` in `getGenres()`.

## 6. Make getGenres() Asynchronous
- Convert `getGenres()` to an asynchronous function for better promise handling.

## 7. Handle Errors in getGenres()
- Implement try/catch block in `getGenres()` to catch and log errors during fetch.

## 8. Send GET Request for Genres
- Use `fetch()` in `getGenres()` to send a GET request to `urlToFetch`.

## 9. Check Response Status
- Verify response status in `getGenres()` try block using `.ok` property.

## 10. Convert Response to JSON
- If response is okay, convert to JSON object and store in `jsonResponse`.

## 11. Retrieve Genres Data
- Log `jsonResponse` and save `genres` property to a variable.

## 12. Return Genres Data
- Return `genres` variable from `getGenres()`.

## 13. Discover Movies Based on Genre
- Save "Movie Discover" API endpoint to `discoverMovieEndpoint`.

## 14. Set Query Parameters for Movie Request
- Create `requestParams` with `api_key` and `with_genres` parameters.

## 15. Convert getMovies() to Asynchronous
- Make `getMovies()` asynchronous for promise handling.

## 16. Handle Errors in getMovies()
- Add try/catch block in `getMovies()` to catch and log fetch errors.

## 17. Process Response for Movies
- Check response status, convert to JSON, and log `jsonResponse`.

## 18. Fetch Movie Details
- Modify `getMovieInfo()` to accept a movie parameter for details fetching.

## 19. Define Movie Details Endpoint
- Save "Details" endpoint to `movieEndpoint` and replace `{movie_id}` with `movieId`.

## 20. Set Query Parameters for Movie Info Request
- Create `requestParams` with `api_key`.

## 21. Convert getMovieInfo() to Asynchronous
- Make `getMovieInfo()` asynchronous for promise handling.

## 22. Process Response for Movie Info
- Check response status, convert to JSON, and store in `movieInfo`.

## 23. Return Movie Info
- Return `movieInfo` from `getMovieInfo()`.

## 24. Display Random Movie
- Convert `showRandomMovie()` to an asynchronous function and call `getMovies()`.

## 25. Get Random Movie and Movie Info
- Call `getRandomMovie()` and `getMovieInfo()` within `showRandomMovie()` and await their results.

## 26. Call displayMovie()
- Call `displayMovie()` with retrieved movie info as argument.

## 28. Additional Challenges
- Explore more features like rearranging information, storing user preferences, and randomizing results.
- https://nickefr.github.io/web.API/index.html
![API KEY-API TOKEN](https://github.com/nickefr/web.API/assets/73330890/882a441e-6476-4836-99fe-8cc98b14f0f1)
![film finder1](https://github.com/nickefr/web.API/assets/73330890/5a60c384-ed04-45a1-bc5f-10fe3e8a7338)




  
