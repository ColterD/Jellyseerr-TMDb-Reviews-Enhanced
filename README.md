# Jellyseerr TMDb Reviews Enhanced

![License](https://img.shields.io/github/license/ColterD/Jellyseerr-TMDb-Reviews-Enhanced)
![Version](https://img.shields.io/github/v/release/ColterD/Jellyseerr-TMDb-Reviews-Enhanced)
![Downloads](https://img.shields.io/github/downloads/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/total)

## **Overview**

**Jellyseerr TMDb Reviews Enhanced** is a userscript that integrates the latest reviews from [The Movie Database (TMDb)](https://www.themoviedb.org/) directly into your [Jellyseerr](https://github.com/Fallenbagel/jellyseerr) movie and TV show pages. Enhance your content discovery with up-to-date reviews seamlessly embedded in your Jellyseerr interface.

## **Features**

- **Latest TMDb Reviews:** Displays recent reviews for movies and TV shows on Jellyseerr pages.
- **Customizable Settings:** Configure the number of reviews, language, and caching preferences.
- **Cache Management:** Option to cache fetched reviews with a **"Clear TMDb Cache"** button.
- **Responsive Design:** Styled to match Jellyseerr's dark and light themes.
- **Auto-Updating:** Automatically updates to the latest version via userscript managers.

## **Installation**

### **Prerequisites**

- A userscript manager extension installed in your browser:
  - [Tampermonkey](https://www.tampermonkey.net/) (Chrome, Firefox, Edge, Safari, etc.)
  - [Violentmonkey](https://violentmonkey.github.io/)
  - [Greasemonkey](https://www.greasespot.net/) (Firefox)

### **One-Click Installation**

1. **Click the Installation Link:**

   [Install Jellyseerr TMDb Reviews Enhanced](https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/raw/main/jellyseerr-tmdb-reviews-enhanced.user.js)

2. **Confirm Installation:**
   
   - Your userscript manager (e.g., Tampermonkey) will prompt you with the script details.
   - Click **"Install"** or **"Save"** to add the script to your manager.

3. **Configure the Script:**
   
   - After installation, open your userscript manager dashboard.
   - Locate **"Jellyseerr TMDb Reviews Enhanced"** and click **"Edit"**.
   - Replace `'YOUR_TMDB_API_KEY'` with your actual TMDb API Key.
   - Adjust other settings as desired (e.g., `enableCaching`, `maxReviews`).
   - Save the script.

### **Usage**

- **Navigate to a Media Page:**
  
  Visit a movie or TV show page on your Jellyseerr instance (e.g., `https://request.colter.plus/movie/harry-potter-and-the-goblet-of-fire`).

- **View TMDb Reviews:**
  
  After the page loads, a **"Latest Reviews from TMDb"** section will appear with the latest reviews.

- **Clear TMDb Cache (If Enabled):**
  
  Click the **"Clear TMDb Cache"** button below the reviews to clear cached data.

## **Configuration**

1. **Obtain a TMDb API Key:**
   
   - Sign up on [TMDb](https://www.themoviedb.org/).
   - Navigate to account settings and generate an API key.

2. **Edit the Userscript:**
   
   - Open your userscript manager dashboard.
   - Edit **"Jellyseerr TMDb Reviews Enhanced"**.
   - Replace `'YOUR_TMDB_API_KEY'` with your TMDb API Key.
   - Modify other settings as needed.
   - Save the script.

## **Auto-Updating**

The script is configured to auto-update via userscript managers like Tampermonkey. Ensure that the `@updateURL` and `@downloadURL` in the script metadata point to the raw GitHub URL.

## **Reporting Issues**

If you encounter any issues or have feature requests, please [open an issue](https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/issues) on GitHub.

## **License**

This project is licensed under the [MIT License](LICENSE).

---
