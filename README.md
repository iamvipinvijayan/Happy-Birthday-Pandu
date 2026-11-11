# Happy Birthday Pandu — website

Public website for the **Happy Birthday Pandu** mobile app
(Android package `com.iamvipinvijayan.happybirthdaypandu`), hosted on GitHub Pages.

| Page | URL |
| --- | --- |
| Home | https://iamvipinvijayan.github.io/Happy-Birthday-Pandu/ |
| Privacy policy | https://iamvipinvijayan.github.io/Happy-Birthday-Pandu/privacy/ |

Use the privacy policy URL in the Google Play Console (App content → Privacy policy)
and in App Store Connect.

## Layout

```
docs/                 <- GitHub Pages source (Settings → Pages → main / docs)
  index.html          <- landing page
  privacy/index.html  <- privacy policy
  style.css           <- shared styles, light + dark
  .nojekyll           <- serve files as-is
```

The Pages source is the `docs/` folder rather than the repository root, so the
root stays free for app code or other files. Pushing to `main` republishes the
site within a minute.

## Editing the policy

Edit `docs/privacy/index.html`, update both dates at the top of the page, and
push. If the app ever gains analytics, ads, a database or any new permission,
update this policy in the same change — Play requires the disclosure to match
what the app actually does.
