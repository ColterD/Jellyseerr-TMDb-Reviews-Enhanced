# Jellyseerr TMDb Reviews Enhanced

![License](https://img.shields.io/github/license/ColterD/Jellyseerr-TMDb-Reviews-Enhanced)
![Version](https://img.shields.io/github/v/release/ColterD/Jellyseerr-TMDb-Reviews-Enhanced)
![Downloads](https://img.shields.io/github/downloads/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/total)
![Issues](https://img.shields.io/github/issues/ColterD/Jellyseerr-TMDb-Reviews-Enhanced)

## 📚 Overview

**Jellyseerr TMDb Reviews Enhanced** is a userscript that seamlessly integrates the latest reviews from [The Movie Database (TMDb)](https://www.themoviedb.org/) directly into your [Jellyseerr](https://github.com/Fallenbagel/jellyseerr) movie and TV show pages. Enhance your content discovery experience with up-to-date reviews embedded right within your Jellyseerr interface.

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

- **[Violentmonkey](https://violentmonkey.github.io/)** (Open-Source)
- **[Tampermonkey](https://www.tampermonkey.net/)** (Closed Source - Chrome, Firefox, Edge, Safari, etc.)
- **[Greasemonkey](https://www.greasespot.net/)** (Outdated)

### 🔗 One-Click Installation

1. **Click the Installation Link:**

   [Install Jellyseerr TMDb Reviews Enhanced](https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/raw/main/jellyseerr-tmdb-reviews-enhanced.user.js)

2. **Confirm Installation:**

   - Your userscript manager (e.g., Violentmonkey, Tampermonkey) will detect the script and prompt you with installation details.
   - Click **"Install"** or **"Save"** to add the script to your manager.

### 📂 Manual Installation

1. **Download the Userscript:**

   - Navigate to the [Releases](https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/releases) section of this repository.
   - Download the latest `jellyseerr-tmdb-reviews-enhanced.user.js` file.

2. **Install via Userscript Manager:**

   - Open your userscript manager dashboard.
   - Add a new script and paste the contents of the downloaded `.user.js` file.
   - Save the script.

### 🌐 Custom Installation for Other Sites

If you wish to use **Jellyseerr TMDb Reviews Enhanced** on your own website or a different URL pattern, follow these steps:

1. **Open the Userscript Manager:**

   - Go to your userscript manager dashboard (Violentmonkey, Tampermonkey, Greasemonkey).

2. **Edit the Script:**

   - Locate **"Jellyseerr TMDb Reviews Enhanced"** in your scripts list.
   - Click **"Edit"**.

3. **Modify the `@match` Pattern:**

   - Find the `@match` directive in the metadata block:
     ```javascript
     // @match        https://request.colter.plus/*
     ```
   - Replace `https://request.colter.plus/*` with the URL pattern of your website.
     - **Example for `https://yourwebsite.com/*`:**
       ```javascript
       // @match        https://yourwebsite.com/*
       ```
   - **Note:** Ensure the match pattern accurately corresponds to the pages where you want the script to run.

4. **Save the Script:**

   - After making changes, save the script to apply the new match pattern.

## ⚙️ Configuration

1. **Obtain a TMDb API Key:**

   - Sign up on [TMDb](https://www.themoviedb.org/).
   - Navigate to account settings and generate an API key.

2. **Edit the Userscript:**

   - Open your userscript manager dashboard.
   - Edit **"Jellyseerr TMDb Reviews Enhanced"**.
   - Upon first run, the script will prompt you to enter your TMDb API Key. Enter your key when prompted.
   - **Adjust Settings as Needed:**
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
   - **Save the Script:**  
     - After making changes, save the script to apply the new settings.

## 🖥️ Usage

1. **Navigate to a Media Page:**

   - Open Jellyseerr and navigate to a movie or TV show page (e.g., `https://request.colter.plus/movie/harry-potter-and-the-prisoner-of-azkaban`).

2. **View TMDb Reviews:**

   - After the page loads, a **"Latest Reviews from TMDb"** section will appear below the existing reviews.
   - Each review includes the author's name, rating, date, and a truncated version of the review content with a "continue reading" link if applicable.

3. **Clear TMDb Cache:**

   - Click the **"Clear TMDb Cache"** button located below the reviews section.
   - Confirm the action in the prompt.
   - The script will clear the cached reviews and refresh the reviews section.

## 🛠️ Development

### 📝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

### 🐛 Reporting Issues

If you encounter any issues or have feature requests, please [open an issue](https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/issues) on GitHub.

## 📈 Auto-Updating

The script is configured to auto-update via userscript managers like Violentmonkey and Tampermonkey. Ensure that the `@updateURL` and `@downloadURL` in the script metadata point to the raw GitHub URL.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 📞 Contact

For any questions or feedback, feel free to reach out via [GitHub Issues](https://github.com/ColterD/Jellyseerr-TMDb-Reviews-Enhanced/issues).

---

*Happy Streaming! 🎬*
