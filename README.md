## Usage

### 1. Install dependencies

Hyde(Theme) is built on Jekyll and uses its built-in SCSS compiler to generate our CSS. Before getting started, you'll need to install the Jekyll gem and related dependencies:

```bash
bundle install
```
### 2. Running Locally

Use jekyll

```bash
bundle exec jekyll serve
```

the site should be available at `http://localhost:4000`.

### 3. Creating posts

To create a new post add the markdown file to `_posts` directory, it needs to follow this convention `YYYY-MM-DD-title.md`

Front matter should be included at the top of the file (header)

```md
---
layout: post
title: post title
---
```

### 4. Sidebar menu

Create a list of nav links in the sidebar by assigning each Jekyll page the correct layout in the page's front matter.

```md
---
layout: page
title: About
---
```

### 5. Sticky sidebar content

By default Hyde ships with a sidebar that affixes it's content to the bottom of the sidebar. You can optionally disable this by removing the `.sidebar-sticky` class from the sidebar's `.container`. Sidebar content will then normally flow from top to bottom.