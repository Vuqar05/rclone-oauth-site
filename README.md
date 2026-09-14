# rclone OAuth Site

This repository contains a static website for **rclone vugar**, a personal-use OAuth application client for the rclone command-line tool that connects to Google Drive.

> **Important:** The app name shown on this site (`rclone vugar`) must exactly match the "App name" configured on the [OAuth consent screen](https://console.cloud.google.com/apis/credentials/consent) in Google Cloud Console. If you rename the app in either place, update the other to match.

## Contents

- **index.html** — Home page describing the application
- **privacy.html** — Privacy policy page

## Purpose

These pages are hosted via GitHub Pages to satisfy Google OAuth's app verification requirements, which mandate that OAuth applications provide:
1. A publicly accessible homepage
2. A privacy policy page

## Hosting on GitHub Pages

This site is configured to be hosted on GitHub Pages. The live URLs are:
- **Home**: `https://Vuqar05.github.io/rclone-oauth-site/`
- **Privacy Policy**: `https://Vuqar05.github.io/rclone-oauth-site/privacy.html`
GitHub will build and deploy your site within a few minutes. The live URLs will be available at the addresses listed above.

## Verifying Home Page Ownership (Google OAuth Verification)

Google's OAuth verification checks that the home page URL is "registered to you" via [Google Search Console](https://search.google.com/search-console). To resolve a "not registered to you" finding for a GitHub Pages site:

1. Open Search Console and add a property using the **URL prefix** method with `https://vuqar05.github.io/rclone-oauth-site/`.
2. Choose the **HTML tag** verification method (file-upload verification is awkward on GitHub Pages, and domain-wide verification isn't available for a `github.io` subpath you don't own outright).
3. Copy the `<meta name="google-site-verification" ...>` tag Search Console gives you.
4. Uncomment and replace the placeholder meta tag already present near the top of `index.html` with that exact tag.
5. Commit, push, and wait for GitHub Pages to redeploy, then click "Verify" in Search Console.
6. Use the **same Google account** that owns/manages the OAuth consent screen to do this verification, and make sure that account is listed as a verified owner of the property.

## Privacy

This application is for personal use only. For details, see the privacy policy page.
