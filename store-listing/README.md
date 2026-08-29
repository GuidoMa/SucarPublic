# Store listing data

Source data for each flavor's Play Console listing, one directory per flavor.

```
<flavor>/
  contact-email.txt
  contact-website.txt          (optional)
  listings/
    <locale>/                  e.g. en-US, de-DE
      title.txt
      short-description.txt     max 80 characters
      full-description.txt      max 4000 characters
      graphics/
        icon/                        exactly one file, 512x512
        feature-graphic/             exactly one file, 1024x500
        phone-screenshots/           mobile only, up to 8 files
        android-auto-screenshots/    mobile only, reference only (see note below)
        head-unit-screenshots/       automotive only, reference only (see note below)
```

This mirrors the directory layout Gradle Play Publisher expects for a Play Console store listing, so the files here can be copied straight over without renaming.

`android-auto-screenshots/` and `head-unit-screenshots/` aren't a Play listing image type — Play has no such category — so they're kept here only as a reference copy of what's shown on Android Auto and the automotive head unit.

Text and graphics files are placeholders until filled in.
