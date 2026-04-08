# is-it-friday-in-istanbul

> The most important question of the week, answered live from Istanbul time.

**Live →** [muratzrl.github.io/is-it-friday-in-istanbul](https://muratzrl.github.io/is-it-friday-in-istanbul/)

## What

A tiny website that answers one question: **is it currently Friday in Istanbul?**

If yes → big green **YES**.
If no → big red **NO**.

That's the entire feature set. There are no plans to add more.

## Why

Because the world is loud and most websites lie to you. This one tells the truth, in one word, in two seconds. You either close the tab relieved, or you close it disappointed. No newsletter signup. No cookie banner. No "we use cookies to enhance your experience."

## How it works

One HTML file. No backend. No API. No build step. Just:

1. Get the current time in `Europe/Istanbul` (UTC+3).
2. Check if `getDay() === 5`.
3. Render YES or NO accordingly.
4. Update every second so the clock stays honest.

The time zone is hardcoded to Istanbul, so it works the same whether you open it from Kadıköy, Berlin, or Tokyo. The answer is about Istanbul, not about you.

## Stack

- HTML
- CSS (with one hand-drawn SVG skyline)
- JavaScript (`new Date()` and a `switch` statement, basically)
- Zero dependencies
- Zero excuses

## Features

- ⏱ Live Istanbul clock
- 📅 Day of the week
- ⏳ Countdown to next Friday
- 💬 A different message for every day of the week
- 🌃 A tiny Istanbul skyline at the bottom, because vibes matter
- 🏷 Browser tab title that updates with the answer

## Updating the messages

Open `index.html`, find the `subtexts` object near the bottom of the script tag, and change the lines for whichever day you want. Commit. Done.

## License

Do whatever you want. Just don't add tracking.
