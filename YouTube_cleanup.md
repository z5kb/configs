CSS selectors which hide most (possibly all) of the many annoying elements on YouTube. Can be pasted in a browser extension like Stylebot.

```css
/* The "1 month trial for YouTube Premium" ad which appears on the home page as a page-wide banner */
div.style-scope.ytd-statement-banner-renderer {
  display: none;
}

/* The shorts section on the home page which can be dismissed for 30 days but reappears again after that */
ytd-rich-section-renderer > div[id="content"]:has(div[id="dismissible"]) {
  display: none;
}

/* Randomly-generated "Mix" playlists */
ytd-rich-item-renderer:has(yt-thumbnail-overlay-badge-view-model) {
  display: none;
}

/* "Membership only" videos */
ytd-rich-item-renderer:has(div[class="yt-content-metadata-view-model__badge"]) {
  display: none;
}

/* The "Shorts" button inthe left sidebar */
ytd-mini-guide-renderer > div > ytd-mini-guide-entry-renderer:has(a[title="Shorts"]) {
  display: none;
}

/* The "Home" & "Shorts" buttons in the left sidebar (the one which opens with the burger menu on the top left) */ 
div[id="sections"] > ytd-guide-section-renderer:has(a[title="Home"]) {
  display: none;
}

/* The "Explore" section of buttons in the left sidebar (the one which opens with the burger menu on the top left), which redirects to the Music, Gaming and Sports video categories */
div[id="sections"] > ytd-guide-section-renderer:has(a[title="Music"]) {
  display: none;
}

/* The "More from YouTube" section of buttons in the left sidebar (the one which opens with the burger menu on the top left), which redirects to YouTube Premium, YouTube Music & YouTube Kids */
div[id="sections"] > ytd-guide-section-renderer:has(a[title="YouTube Premium"]) {
  display: none;
}

/* Shorts displayed in search results */
grid-shelf-view-model {
  display: none;
}

/* "Previously watched" section which interrupts the search results */
ytd-shelf-renderer {
  display: none;
}

/* Right sidebar with additional videos which appears when playing a video */
div[id="secondary"] {
  display: none;
}

/* Links + similar videos in the video description */
ytd-video-description-infocards-section-renderer {
  display: none;
}

/* "Transcript video" section in the video description */
ytd-video-description-transcript-section-renderer {
  display: none;
}
```
