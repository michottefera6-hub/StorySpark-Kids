# StorySpark Kids

StorySpark Kids is a small browser-based prototype that turns a short
children's story into colorful cartoon scenes and a simple animated WebM
video.

## What this version does

-   Runs directly in the browser.
-   Does **not** ask for a Pollinations API key.
-   Does **not** require an OpenAI API key.
-   Does **not** require a Hugging Face API key.
-   Splits a short story into 1--3 scenes.
-   Creates simple cartoon-style scene artwork locally in the browser.
-   Creates a simple zoom/motion WebM animation from the scenes.
-   Works as a static GitHub Pages website.

## Files

-   `index.html` --- the complete StorySpark Kids web app.
-   `.nojekyll` --- optional GitHub Pages helper file. It can be left
    empty.
-   `README.md` --- setup and usage notes.

## GitHub Pages setup

1.  Put `index.html` in the **root** of your repository.
2.  Put `.nojekyll` in the same root folder.
3.  Put `README.md` in the root as well.
4.  Commit the changes.
5.  In **Settings → Pages**, use **Deploy from a branch**.
6.  Select the `main` branch and `/(root)`.
7.  Save if GitHub shows an enabled Save button.
8.  Wait for the Pages deployment to finish.
9.  Open your GitHub Pages address.

Your repository should look like:

``` text
index.html
README.md
.nojekyll
```

The important file for the website is `index.html`.

## Important limitation

This is intentionally a no-API prototype. The cartoon images are
generated locally with browser SVG/canvas graphics. The animation is a
real WebM video made in the browser, but it is not full AI text-to-video
character animation.

## Next upgrades

A future version can add:

-   AI-generated cartoon images
-   character consistency
-   automatic storyboarding
-   narration
-   subtitles
-   background music
-   sound effects
-   image-to-video animation
-   16:9 YouTube export
-   downloadable MP4 conversion

## Troubleshooting

### GitHub Pages shows 404

Make sure the file is named exactly `index.html` and is in the
repository root, not inside another folder.

### The site opens but looks old

Refresh the page after the latest GitHub Pages deployment finishes.

### The video does not save

Keep the page open while the animation is being created. Browser support
for `MediaRecorder` can vary between browsers.
