# Stop Typing App website

The landing page for [Stop Typing App](https://github.com/kevintraver/stop-typing-app), a macOS menu bar app that nudges you to dictate instead of typing out paragraphs.

It's a single static page with no build step: `index.html` plus its icons. Vercel serves it as is.

To preview locally:

```sh
python3 -m http.server 8000
```

## Privacy

The page loads [Vercel Web Analytics](https://vercel.com/docs/analytics) from `/_vercel/insights/script.js` and [Vercel Speed Insights](https://vercel.com/docs/speed-insights) from `/_vercel/speed-insights/script.js`. Both only work on a Vercel deployment with them enabled, so the requests 404 when previewing locally. The footer and the privacy section disclose them.

There are no third-party font requests. Geist and Geist Mono are served from `fonts/`; their SIL Open Font Licenses are included there. Vercel still serves ordinary HTTP requests and can retain hosting request metadata.

App privacy text describes the next privacy-hardened release. Publish it together with that release; local changes do not update the public download or deployed site.
