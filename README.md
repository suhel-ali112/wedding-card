# Nikah Invitation

An animated wedding (Nikah) invitation website for the Muslim community. It is a single HTML file with no build step, so it runs on GitHub Pages as it is.

## Features

- Opening screen with two doors that slide apart when the seal is tapped
- Bismillah in Arabic calligraphy, Quran verse (Ar-Rum 30:21) and a closing dua
- Swaying lanterns, a slowly turning geometric star and floating gold sparks
- Event cards for Mehndi, Nikah and Walima with Hijri dates calculated automatically
- Live countdown to the Nikah
- Venue section with Google Maps and Add to Calendar links
- RSVP form inside the page that saves each response to a Google Sheet
- Personal guest links that greet each guest by name
- Optional soft background music, generated in the browser with no audio files
- Works on phones, respects reduced-motion settings, English and Urdu text

## Live demo

Add your link here after publishing: `https://YOUR-USERNAME.github.io/YOUR-REPO/`

## Publish on GitHub Pages

1. Create a public repository and upload `index.html` to the main branch.
2. Open Settings, then Pages.
3. Choose branch `main` and folder `/ (root)`, then save.
4. After a minute or two the site is live at `https://YOUR-USERNAME.github.io/YOUR-REPO/`.

## Change the details

The names, parents, dates, times and venue in the file are sample content. Open `index.html` and replace them:

| What | Where to look |
| --- | --- |
| Couple's names | Search for `Zaid` and `Ayesha` |
| Parents' names | The "The Bride & Groom" section |
| Event dates, times, venue | The `events` section and the venue section |
| Countdown target | `new Date('2026-12-11T16:30:00+05:30')` in the script |
| Add to Calendar link | The `calendar.google.com` link in the venue section |
| Maps link | The `google.com/maps` link in the venue section |
| Footer contact line | The `credit` block at the end of the page |

## RSVP to Google Sheets

The RSVP form posts to a Google Form, and the Form saves answers to a Google Sheet.

1. Create a Google Form with four short-answer questions: Name, Number of Guest, Arrival Date, Arrival Time.
2. In the Responses tab, choose Link to Sheets.
3. In the form menu choose Get pre-filled link, fill every question with test text and copy the link. Each `entry.NUMBER` in that link belongs to one question.
4. In `index.html`, update `FORM_URL` and the `ENTRY` values in the script with your own form address and numbers.

## Personal guest links

Add `#for-` and the guest's name in lowercase with hyphens to the page address:

```
https://YOUR-USERNAME.github.io/YOUR-REPO/#for-imran-siddiqui
```

The page then shows "Dear Imran Siddiqui" and fills the name into the RSVP form. Names must use English letters.

## Built with

HTML, CSS and plain JavaScript. Fonts are loaded from Google Fonts: Amiri, Aref Ruqaa, Noto Nastaliq Urdu, Cormorant Garamond and Jost.

## Contact

Want an invitation like this made for your own event?

Suhail Ali, +91 90275 50415 (call or WhatsApp)
