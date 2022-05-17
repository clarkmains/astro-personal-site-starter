# Astro 'Slinky' personal starter page

An Astro + Tailwind CSS personal one-page starter.

> Why 'Slinky'?

The design of the page is slim, long and made of horizontal sections - a bit like a coiled [Slinky](https://en.wikipedia.org/wiki/Slinky).

## Features

- 📓 Markdown driven content
- 💨 Tailwind CSS for styling
- 💯 Perfect Lighthouse score
- 🌙 Dark mode
- 📱 Responsive
- ♿ Accessible
- 🔎 SEO-enabled

## Updating content

Understanding Astro's use of [Frontmatter and Markdown](https://docs.astro.build/en/guides/markdown-content/) is helpful here.

The content of the page is driven entirely by the following file:

    /src/pages/index.md

What follows is a breakdown of how the different sections of the page are populated from this file.

### Header section

Headshot image is stored in `/public` and configured as follows:

    image: "/headshot.jpeg"

Page heading e.g. your name:

    name: Daphne Blake

Page sub-heading:

    description: Hey! I'm Daphne, a Web Developer & UX Designer based in Glasgow, Scotland.

### About section

The content of this section is populated by the Markdown slot, so is flexible and can contain rich content such as images etc.

Tailwind's [Typography plugin](https://tailwindcss.com/docs/typography-plugin) is used to format the Markdown.

### Experience section

This section is populated by the `experience` field.

The `experience` field expects a list. The list is not ordered programatically - define the items in the order you want them to appear.

Each item in the list should have the following fields:

Time period:

    period: Jun 2019 - Now

The `period` is treated as one string so you can include terms like "Now" or "Current".

Place of work:

    place: Tyrell Corporation

Description of what you did there:

    description: User Experience Designer

### Education section

This section is populated by the `education` field.

The `education` field expects a list. The list is not ordered programatically - define the items in the order you want them to appear.

Each item in the list should have the following fields:

Time period:

    period: 2014 - 2015

The `period` is treated as one string so you can include terms like "Now" or "Current".

Place of education:

    place: Strathclyde University

Description of what you did there:

    description: MSc Mobile Web Development

### Contact section

The link icons in this section are populated by the `contacts` field.

The `contacts` field expects a list. The list is not ordered programatically - define the items in the order you want them to appear.

Each item in the list should have the following fields:

Name of contact type, used for accessibility:

    name: GitHub

Icon to display:

    icon: fa:github

Must be an icon supported by [astro-icon](https://www.npmjs.com/package/astro-icon).

Link:

    link: https://www.github.com/your-name

## Credits

Example headshot image by [Pexels](https://pixabay.com/users/pexels-2286921/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=1867618) from [Pixabay](https://pixabay.com//?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=1867618).