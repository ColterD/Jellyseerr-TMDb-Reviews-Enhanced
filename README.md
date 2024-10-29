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
  - [Violentmonkey](https://violentmonkey.github.io/) (**Preferred!** Open-Source)
  - [Tampermonkey](https://www.tampermonkey.net/) (Closed Source - Chrome, Firefox, Edge, Safari, etc.)
  - [Greasemonkey](https://www.greasespot.net/) (**Outdated**)

### **One-Click Installation**

1. **Click the Installation Link:**

   [Install Jellyseerr TMDb Reviews Enhanced](https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/raw/main/jellyseerr-tmdb-reviews-enhanced.user.js)

2. **Confirm Installation:**
   
   - Your userscript manager (e.g., Violentmonkey, Tampermonkey) will prompt you with the script details.
   - Click **"Install"** or **"Save"** to add the script to your manager.

3. **Configure the Script:**
   
   - After installation, open your userscript manager dashboard.
   - Locate **"Jellyseerr TMDb Reviews Enhanced"** and click **"Edit"**.
   - Replace `'YOUR_TMDB_API_KEY'` with your actual TMDb API Key.
   - Adjust other settings as desired (e.g., `enableCaching`, `maxReviews`).
   - Save the script.

### **Custom Installation for Other Sites**

If you wish to use **Jellyseerr TMDb Reviews Enhanced** on your own website or a different URL pattern, you need to modify the userscript's match pattern:

1. **Open the Userscript Manager:**
   
   - Go to your userscript manager dashboard (Violentmonkey, Tampermonkey, Greasemonkey).

2. **Edit the Script:**
   
   - Find **"Jellyseerr TMDb Reviews Enhanced"** in your scripts list.
   - Click **"Edit"**.

3. **Modify the `@match` Pattern:**
   
   - Locate line 6 in the metadata block:
     ```javascript
     // @match        https://request.colter.plus/*
     ```
   - Replace `https://request.colter.plus/*` with the URL pattern of your website.
     - **Example for `https://yourwebsite.com/*`:**
       ```javascript
       // @match        https://yourwebsite.com/*
       ```
   - **Note:** Ensure that the match pattern correctly corresponds to the pages where you want the script to run.

4. **Save the Script:**
   
   - After making changes, save the script to apply the new match pattern.

## **Usage**

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
   - Modify other settings as needed:
     - **Enable Caching:**
       ```javascript
       const enableCaching = true; // Set to true to enable caching
       ```
     - **Log Level:**
       ```javascript
       const logLevel = 'info'; // Options: 'off', 'info', 'verbose'
       ```
     - **Language Code:**
       ```javascript
       const languageCode = 'en-US'; // Replace with your preferred language code
       ```
     - **Maximum Reviews to Display:**
       ```javascript
       const maxReviews = 3; // Set the number of reviews to display
       ```
   - Save the script after making changes.

## **Auto-Updating**

The script is configured to auto-update via userscript managers like Violentmonkey and Tampermonkey. Ensure that the `@updateURL` and `@downloadURL` in the script metadata point to the raw GitHub URL.

## **Reporting Issues**

If you encounter any issues or have feature requests, please [open an issue](https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/issues) on GitHub.

## **License**

This project is licensed under the [MIT License](LICENSE).

---
