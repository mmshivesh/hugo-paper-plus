# Paper Plus

Paper Plus, a fork of Paper theme that builds on the original [Paper](https://github.com/nanxiaobei/hugo-paper) with lots of new features.


---

## New Features

1. Dark mode is now responsive to the appearance of your computer. It doesn't depend on the time of the day anymore but rather on the `prefers-color-scheme:` flag.
2. Posts can now have a banner header image (place in the same folder as the post/`static` folder and in the front matter of the post's markdown use: 

`header: "imagename.png"`

(1440x250 images preferred)

3. Additional configurable Parameters in `config.toml`:

```
[params]
    email = <Your Email> (Shown in the footer as a "Contact Me" link)
    github = <Link to your github> (Adds a top bar menu item linking to your GitHub)
    darkDefault = <true | false> (Use Dark mode by default if the browser doesn't support Automatic Appearances)
    siteAuthor = <Site Author> (Name to show on the footer without showing anything on posts)
    mainTitle = "Recent Posts" (Title to show on the main root page instead of repeating the website name)
    serifTitles = <true | false> (Setting to true will use serif titles instead of sans-serif titles. Default serif font is Playfair. Place the font under `static/fonts/PlayfairDisplay-Bold.ttf`)
```

4. Proper hover animations on the Navbar.
5. Reading time estimates on each post (Shown along with the date when `showDate` is set to true on the front matter)
6. Optional Serif titles.


## Overview

Demo: `https://mmshivesh.ml/hugo-paper-plus/`

<p>
<kbd>
  <img src="https://raw.githubusercontent.com/mmshivesh/hugo-paper-plus/master/images/screenshot.png" alt="Paper Plus Light">
</kbd>
</p>

<p>
<kbd>
  <img src="https://raw.githubusercontent.com/mmshivesh/hugo-paper-plus/master/images/screenshot_dark.png" alt="Paper Plus Dark Mode">
</kbd>
</p>

<p>
<kbd>
  <img src="https://raw.githubusercontent.com/mmshivesh/hugo-paper-plus/master/images/screenshot_features.png" alt="Paper Plus Sample post">
</kbd>
</p>

## Install

Inside the folder of your Hugo site, run:

```bash
git clone https://github.com/mmshivesh/hugo-paper-plus themes/paper
```

Then change in `config.toml`:

```toml
theme = "paper"
```

For more information read the official [guide](https://gohugo.io/getting-started/quick-start/#step-3-add-a-theme) of Hugo.

## Dark Mode

Dark mode has been updated in Paper Plus to respect `prefers-color-scheme` provided by the browser. It dynamically changes theme when you change from Light mode to Dark and vice-versa.
