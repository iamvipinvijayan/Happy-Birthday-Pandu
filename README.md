# Happy Birthday Pandu — website

Public website for the **Happy Birthday Pandu** mobile app
(Android package `com.iamvipinvijayan.happybirthdaypandu`), hosted on GitHub Pages.

| Page | URL |
| --- | --- |
| Home | https://iamvipinvijayan.github.io/Happy-Birthday-Pandu/ |
| Privacy policy | https://iamvipinvijayan.github.io/Happy-Birthday-Pandu/privacy/ |
| Account & data deletion | https://iamvipinvijayan.github.io/Happy-Birthday-Pandu/delete-account/ |

In the Google Play Console, use the privacy policy URL under **App content → Privacy
policy**. Both pages are public and need no sign-in to view, which Google checks.

From version 1.0.3 the app has no sign-in and collects no data, so Data safety is
declared as **no data collected** and the **Data deletion** URL is left empty. The
deletion page stays published anyway: its URL may already be cached by Google, and
it is where testers from the earlier signed-in builds are told to write.

## Layout

```
docs/                 <- GitHub Pages source (Settings → Pages → main / docs)
  index.html                 <- landing page
  privacy/index.html         <- privacy policy
  delete-account/index.html  <- account & data deletion
  style.css                  <- shared styles, light + dark
  .nojekyll                  <- serve files as-is
```

The Pages source is the `docs/` folder rather than the repository root, so the
root stays free for app code or other files. Pushing to `main` republishes the
site within a minute.

## Editing the policy

Edit `docs/privacy/index.html`, update the effective date at the top of the page,
and push. The same claims appear on all three pages — the landing page, the privacy
policy and the deletion page — so a change has to land in each of them. If the app
ever gains sign-in, analytics, ads, a database or any new permission, update these
pages in the same change — Play requires the disclosure to match what the app
actually does.
