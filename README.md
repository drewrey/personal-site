# 🚀 Drewrey's Personal Site

### Configuration

Basic configuration file: `./src/config.mjs`

```javascript
const CONFIG = {
  name: 'Example',

  origin: 'https://example.com',
  basePathname: '/', // Change this if you need to deploy to Github Pages, for example
  trailingSlash: false, // Generate permalinks with or without "/" at the end

  title: 'Example - This is the homepage title of Example', // Default seo title
  description: 'This is the homepage description of Example', // Default seo description
  defaultImage: 'image.jpg', // Default seo image

  defaultTheme: 'system', // Values: "system" | "light" | "dark" | "light:only" | "dark:only"

  language: 'en', // Default language
  textDirection: 'ltr', // Default html text direction

  dateFormatter: new Intl.DateTimeFormat('en', {
    // Date format
    year: 'numeric',
    month: 'short',
    day: 'numeric',
    timeZone: 'UTC',
  }),

  blog: {
    disabled: false,
    postsPerPage: 4,

    list: {
      pathname: 'blog', // Blog main path, you can change this to "articles" (/articles)
      noindex: false,
      disabled: false,
    },

    post: {
      pathname: '', // Empty for /some-post, value for /pathname/some-post
      noindex: false,
      disabled: false,
    },

    category: {
      pathname: 'category', // Set empty to change from /category/some-category to /some-category
      noindex: true,
      disabled: false,
    },

    tag: {
      pathname: 'tag', // Set empty to change from /tag/some-tag to /some-tag
      noindex: true,
      disabled: false,
    },
  },
};
```

## Roadmap

### Base

- [ ] Improve blog design (More generic design that adapts to more needs).
- [ ] Create component or utilities for related posts.
- [ ] Add more _shortcodes_ or _embed_ functions to posts in Markdown: (eg Video, Tweet...).
- [ ] Add more Tailwind components useful for most scenarios (Features, Contact, Call to Actions, Content, FAQs...)
- [ ] Add commonly used example pages (Ex: About, Terms, Profile, Services...).
- [ ] Create detailed documentation with best practices and redesign tips.
