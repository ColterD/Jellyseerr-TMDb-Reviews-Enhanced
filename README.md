# Jellyseerr TMDb Reviews Enhanced

![License](https://img.shields.io/github/license/ColterD/Jellyseerr-TMDb-Reviews-Enhanced)
![Version](https://img.shields.io/github/v/release/ColterD/Jellyseerr-TMDb-Reviews-Enhanced)
![Downloads](https://img.shields.io/github/downloads/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/total)
![Issues](https://img.shields.io/github/issues/ColterD/Jellyseerr-TMDb-Reviews-Enhanced)

## 📚 Overview

**Jellyseerr TMDb Reviews Enhanced** is a userscript that integrates the latest reviews from [The Movie Database (TMDb)](https://www.themoviedb.org/) directly into your [Jellyseerr](https://github.com/Fallenbagel/jellyseerr) movie and TV show pages. Enhance your content discovery with up-to-date reviews seamlessly embedded in your Jellyseerr interface.

## 🎯 Features

- **Latest TMDb Reviews:** Automatically fetches and displays recent reviews for movies and TV shows on Jellyseerr pages.
- **Customizable Settings:** Configure the number of reviews, language, and caching preferences directly within the script.
- **Cache Management:** Efficient caching mechanism to store fetched reviews for 24 hours, reducing API calls and improving performance.
- **Clear Cache Button:** Convenient "Clear TMDb Cache" button located below the reviews section for easy cache management.
- **Responsive Design:** Adapts to both Jellyseerr's light and dark themes for a consistent look and feel.
- **Auto-Updating:** Automatically checks for and applies updates via userscript managers like Tampermonkey and Violentmonkey.
- **Error Handling:** User-friendly messages and logging for seamless troubleshooting.

## 🚀 Installation

### 🛠 Prerequisites

Ensure you have a userscript manager extension installed in your browser. The following are recommended:

- **[Violentmonkey](https://violentmonkey.github.io/)** (**Recommended!** Open-Source)
- **[Tampermonkey](https://www.tampermonkey.net/)** (Closed Source - Chrome, Firefox, Edge, Safari, etc.)
- **[Greasemonkey](https://www.greasespot.net/)** (**Outdated**)

### 🔗 One-Click Installation

1. **Click the Installation Link:**

   [Install Jellyseerr TMDb Reviews Enhanced](https://raw.githubusercontent.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/main/jellyseerr-tmdb-reviews-enhanced.user.js)

2. **Confirm Installation:**
   
   - Your userscript manager (e.g., Violentmonkey, Tampermonkey) will detect the script and prompt you with installation details.
   - Click **"Install"** or **"Save"** to add the script to your manager.

3. **Configure the Script:**
   
   - After installation, open your userscript manager dashboard.
   - Locate **"Jellyseerr TMDb Reviews Enhanced"** and click **"Edit"**.
   - Replace `'YOUR_TMDB_API_KEY'` with your actual TMDb API Key.
   - Adjust other settings as desired (e.g., `enableCaching`, `maxReviews`).
   - Save the script.

### 🌐 Custom Installation for Other Sites

If you wish to use **Jellyseerr TMDb Reviews Enhanced** on your own website or a different URL pattern, follow these steps:

1. **Open the Userscript Manager:**
   
   - Go to your userscript manager dashboard (Violentmonkey, Tampermonkey, Greasemonkey).

2. **Edit the Script:**
   
   - Find **"Jellyseerr TMDb Reviews Enhanced"** in your scripts list.
   - Click **"Edit"**.

3. **Modify the `@match` Pattern:**
   
   - Locate the `@match` directive in the metadata block:
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

## ⚙️ Configuration

1. **Obtain a TMDb API Key:**
   
   - Sign up on [TMDb](https://www.themoviedb.org/).
   - Navigate to your account settings and generate an API key.

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

## 🛠️ Hosting the Userscript on GitHub for One-Click Installation

To enable users to install your userscript with a single click, ensure that your script is hosted in a way that userscript managers can access it directly. Here's how you can achieve this:

1. **Host the Userscript in the Repository:**
   
   - Ensure that your userscript file (`jellyseerr-tmdb-reviews-enhanced.user.js`) is located in the root directory of your GitHub repository.

2. **Use the Raw GitHub URL for Installation:**
   
   - GitHub serves raw files through `raw.githubusercontent.com`. Use this URL to create a direct link for installation.
   - **Installation Link Format:**
     ```
     https://raw.githubusercontent.com/YourUsername/Jellyseerr-TMDb-Reviews-Enhanced/main/jellyseerr-tmdb-reviews-enhanced.user.js
     ```
   - **Replace `YourUsername`** with your actual GitHub username.

3. **Ensure Correct Metadata for Auto-Updating:**
   
   - In your userscript's metadata block, set the `@updateURL` and `@downloadURL` to point to the raw GitHub URL.
   - **Example:**
     ```javascript
     // @updateURL    https://raw.githubusercontent.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/main/jellyseerr-tmdb-reviews-enhanced.user.js
     // @downloadURL  https://raw.githubusercontent.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/main/jellyseerr-tmdb-reviews-enhanced.user.js
     ```
   - This ensures that userscript managers can check for updates automatically.

4. **Provide the Installation Link in README:**
   
   - As shown in the **One-Click Installation** section above, include a direct link to the raw userscript file.
   - **Example:**
     ```markdown
     [Install Jellyseerr TMDb Reviews Enhanced](https://raw.githubusercontent.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/main/jellyseerr-tmdb-reviews-enhanced.user.js)
     ```

5. **Optional: Create a GitHub Release (Recommended for Versioning):**
   
   - While not mandatory, creating a release helps in managing versions and provides a stable link for userscript managers.
   - **Steps to Create a Release:**
     1. Navigate to your repository on GitHub.
     2. Click on the **"Releases"** tab.
     3. Click **"Draft a new release"**.
     4. Tag the release (e.g., `v1.0.0`), provide a title and description.
     5. Upload the `jellyseerr-tmdb-reviews-enhanced.user.js` file as a binary.
     6. Click **"Publish release"**.
   - **Update Metadata:**
     - After creating a release, update the `@updateURL` and `@downloadURL` in your userscript to point to the release's raw file.
     - **Example:**
       ```javascript
       // @updateURL    https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/releases/latest/download/jellyseerr-tmdb-reviews-enhanced.user.js
       // @downloadURL  https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/releases/latest/download/jellyseerr-tmdb-reviews-enhanced.user.js
       ```
   
   > **Note:** Creating releases is beneficial for version control and ensuring users receive updates smoothly.

## 📣 Recommendations

- **Use Violentmonkey:**  
  Among userscript managers, [Violentmonkey](https://violentmonkey.github.io/) is **Recommended!** for its open-source nature and robust feature set.

## 🛠️ Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## 📞 Contact

For any questions or feedback, feel free to reach out via [GitHub Issues](https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/issues).

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---
