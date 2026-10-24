<!-- GitHub topics: blogger-theme, blogger-template, blog-theme, responsive-theme, dark-mode, mortgage-calculator, seo-theme, xml-template -->

# 🎨 Navy Gold Blogger Theme

A clean, responsive Blogger theme in navy `#0b2a47` and gold `#f0a500`,
built for content blogs. No frameworks, no build step — one XML file.

## Features

- **Homepage hero + mortgage calculator** — an interactive payment calculator
  (price, down payment, rate, term, tax, insurance) with a monthly breakdown
- **Card grid** with real post thumbnails, plus a sidebar (promo box, latest
  posts, categories)
- **Article pages** — share buttons, author box, label-based related posts,
  reading progress bar, read time, comments
- **Auto "On this page" table of contents** — built from the post's H2s
  (JavaScript, 3+ headings)
- **"Keep exploring" band** under post grids on listing pages (home, archive,
  search, label)
- **Dark mode** (toggle in the header), scroll-reveal animations
- **SEO built in** — BlogPosting + Organization schema, FAQPage JSON-LD
  support, `.key-box` takeaway boxes, styled quiz `<details>` blocks

## Install

1. In Blogger: **Theme → ⋮ → Restore** (back up your current theme first:
   Theme → ⋮ → Backup).
2. Upload `blogger-theme.xml`.
3. **Important Blogger quirk:** a theme Restore resets PageList widgets to
   the lists baked into this file. Check your top navigation and footer
   links after installing and re-add any pages you need.
4. The theme requires the standard Blogger chassis, which this file already
   has: `b:templateVersion='1.0.0'` and `<b:skin version='1.0.0'>`.

## Setup — replace every placeholder

Search the file for `YOUR-` and replace each one. Nothing will break if you
miss one, but your site will show placeholder text.

| Placeholder | What to put there |
| ----------- | ----------------- |
| `YOUR-DOMAIN` | Your blog's domain, e.g. `https://www.example.com` (used in schema, page lists, favicon) |
| `YOUR-SITE-NAME` | Your blog's name (headings, schema, footer) |
| `YOUR-TAGLINE` | Your tagline (top bar, logo tag, footer) |
| `YOUR-AUDIENCE` | Who you write for (footer description) |
| `YOUR-GA4-MEASUREMENT-ID` | Your Google Analytics 4 ID (`G-XXXXXXXXXX`), or delete the gtag block |
| `YOUR-PINTEREST-VERIFY-CODE` | Your Pinterest domain-verify code, or delete the meta tag |
| `YOUR-YOUTUBE-CHANNEL-URL` | Your YouTube channel URL (top bar, Shorts strip) |
| `YOUR-YOUTUBE-VIDEO-ID` | The video ID for the Shorts strip embed |
| `YOUR-VIDEO-TITLE` | That video's title |
| `YOUR-CHANNEL-NAME` | Your channel name (Shorts strip text) |
| `YOUR-INSTAGRAM-URL` | Your Instagram profile URL (top bar) |
| `YOUR-FACEBOOK-URL` | Your Facebook profile/page URL (top bar) |
| `YOUR-GUMROAD-LINK` | Your product link for the sidebar promo box |
| `YOUR-FREE-SAMPLE-LINK` | Your free sample link for the promo box |
| `YOUR-PROMO-TEXT`, `YOUR-PROMO-NOTE`, `YOUR-CALL-TO-ACTION` | Promo box copy |
| `YOUR-SIDEBAR-WIDGET-TITLE` | Sidebar promo widget title |
| `YOUR-FEATURED-POST-1/2/3-URL` | The three "Keep exploring" / hero featured links |
| `YOUR-FEATURED-POST-1/2-TITLE`, `YOUR-FEATURED-POST-1/2-DESCRIPTION` | Those cards' titles and descriptions |
| `YOUR-BUYING-GUIDE-URL` | The guide linked from the calculator note |
| `YOUR-HEADLINE`, `YOUR-INTRO-TEXT`, `YOUR-TOPIC` | Hero badge, headline, and intro paragraph |
| `YOUR-LABEL-1` … `YOUR-LABEL-4` | Hero "Popular" topic chips (label names + links) |
| `YOUR-EXAMPLE-QUERY`, `YOUR-EXAMPLE-TOPIC` | Hero search-box example text |
| `YOUR-NUMBER`, `YOUR-STAT-LABEL` | The three hero stat blocks (use your real numbers) |

### Calculator defaults

The calculator ships with example defaults (price 415,000, 20% down, 6.95%,
30 years, 0.85% tax, 8,471 insurance). They are just defaults — change them
to your market's figures in the `mc-price`, `mc-rate`, `mc-ins` inputs in
the file, and update the note under the calculator.

## Customizing

- **Colors:** change `--navy` / `--gold` CSS variables near the top of the
  `<b:skin>` block.
- **Fonts:** the theme uses Inter; swap the font import to change it.
- **Sidebar promo:** the promo box is widget `HTML10` — edit it in
  Layout, or delete it if you don't sell anything.

## Notes & limits

- This is a genericized version of a theme built for a real blog. The
  structure, styling, and scripts are intact; all site-specific content
  (domains, IDs, social links, product links, demo copy) was replaced with
  the placeholders above.
- Labels must use Blogger's Label widget display setting `LIST` for the
  sidebar categories to render as expected.
- Tested for XML well-formedness (parses cleanly); install it on a test
  blog first if you have heavy custom widgets.

## License

MIT — see [LICENSE](LICENSE).
