# YouTube Pink Remover
A simple css stylesheet to revert youtube's new red-pink gradient back to the original red theme. This stylesheet modifies key elements that you often see and interact with, like - progress bar, youtube icon, hd/4k/vr icon, live ring, etc.

<br>

## Installation
### For Chrome, Firefox, Edge, Opera, etc.
1. Install any browser extension of your choice that allows adding custom css (e.g. `User Javascript and CSS` or `Stylus`).
   *  [Chrome Extensions](https://chromewebstore.google.com/)
   *  [Firefox Extensions](https://addons.mozilla.org/)

### For Safari
1. Go to `Safari` > `Preferences` > `Advanced` > `Style Sheet`
2. Create a `.css` file locally, and select it.

<br>

## CSS Code
Copy and paste the following css code into your custom stylesheet

<br>

```
html {
    --yt-spec-static-brand-red: #FF0000 !important;
    --yt-spec-static-overlay-background-brand: #FF0000 !important;
}

.ytp-play-progress,
.yt-spec-avatar-shape--cairo-refresh .yt-spec-avatar-shape__live-badge,
.yt-spec-avatar-shape--cairo-refresh.yt-spec-avatar-shape--live-ring::after,
.ytp-cairo-refresh .ytp-swatch-background-color,
#progress.yt-page-navigation-progress,
#progress.ytd-thumbnail-overlay-resume-playback-renderer {
    background: #FF0000 !important;
    background-color: #FF0000 !important;
}

.ytp-cairo-refresh .ytp-settings-button::after {
    background-color: #FF0000 !important;
}

.ytd-topbar-logo-renderer .yt-icon-shape.style-scope.yt-icon.yt-spec-icon-shape svg > g:first-child path:first-child,
.ytd-reel-shelf-renderer .yt-icon-shape.style-scope.yt-icon.yt-spec-icon-shape svg path:first-child {
    fill: #FF0000 !important;
}
```

<br>

## Report an Issue / Missing Element
If you encounter any issues or notice any missing elements, please [create an issue](https://github.com/abhishek-junghare/youtube-pink-remover/issues)
