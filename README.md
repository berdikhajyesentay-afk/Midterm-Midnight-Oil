# Midnight Oil - a night study cafe

Midterm project, Web Technologies 1 (Front End).

| Member | Pages | Their CSS file |
|---|---|---|
| Byerdikhajy Yesyentai | `index.html` (Home), `gallery.html`, shared setup (`css/style.css`, navbar, footer) | `home.css`, `gallery.css` |
| Byegarys Kuandyg | `menu.html` (has the **table**) | `menu.css` |
| Nurbergen Asan | `about.html`, `events.html` | `about.css`, `events.css` |
| Yerkebulan Abenov | `reserve.html` (has the **form**) | `reserve.css` |

## How the files fit together

```
Midterm_Cafe/
├── index.html, menu.html, ...   one file per page
├── css/
│   ├── style.css                SHARED: colors, fonts, navbar, footer, .btn-lamp
│   └── menu.css, about.css ...  one file per page, only for that page
└── images/                      all photos (write the credit in the footer)
```

Every page loads, in this order: Bootstrap → Google Fonts → `style.css` → its own CSS file.
Later files win, so your own CSS can change how Bootstrap looks.

## Rules so the site looks like ONE website

1. Do not change the navbar or footer on your page. If they need a change, change them on all pages.
2. Use the shared colors and fonts: `var(--lamp)`, `var(--night-light)`, `var(--font-mono)` ... (list at the top of `style.css`).
3. Write styles for your page only in your own CSS file.
4. Write mobile-first: normal rules for a phone, then `@media (min-width: 768px)` and `@media (min-width: 992px)`.
5. Use the shared button: `class="btn btn-lamp"`.

## How to work on your page

1. Open the `Midterm_Cafe` folder in VS Code.
2. Open your page and its CSS file. The comments above each part explain what it does and why.
3. Make your change, save, and refresh the page in Chrome.
4. Open the page in Chrome. Press `F12`, then `Ctrl+Shift+M`, and check it at **375px**, **768px** and **1280px**.
   No sideways scrolling at any width.
5. When a part works, commit it under **your own name** (see below).

## Committing under your own name (on this laptop)

The teamwork grade checks that every member commits their own pages.
Use the email of **your** GitHub account, so GitHub shows the commit on your profile.

```
git add menu.html css/menu.css
git commit --author="Byegarys Kuandyg <your-github-email>" -m "Add the coffee table to the menu"
```

Only commit work you typed yourself, and only add your own files.

Useful pages: https://www.w3schools.com/html/ · https://www.w3schools.com/css/ · https://getbootstrap.com/docs/5.3/

## The defense (60 of 100 points, individual)

You must be able to:
- explain why the site uses these colors, fonts and layout;
- explain every line of **your own** page, and roughly how a teammate's page works;
- change something on your page live, with no help.

So type your page yourself, and ask about anything you don't understand while you build it.
