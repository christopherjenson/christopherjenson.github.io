# Modern Static Site for GitHub Pages

A clean, modern replacement for Jekyll-Now that runs on GitHub Pages.

## Project Structure

```
your-username.github.io/
├── index.html          # Home page
├── about.html          # About page
├── projects.html       # Projects page
├── blog.html          # Blog listing
├── contact.html       # Contact page
├── css/
│   └── style.css      # Main stylesheet
├── js/
│   └── main.js        # JavaScript functionality
├── posts/
│   └── *.html         # Individual blog posts
└── README.md          # This file
```

## Setup Instructions

### 1. Create Repository
1. Go to GitHub and create a new repository named `your-username.github.io`
2. Clone it locally: `git clone https://github.com/your-username/your-username.github.io.git`

### 2. Add Files
Copy all the HTML, CSS, and JS files I've provided into your repository:
- Main HTML pages in root directory
- CSS file in `css/` folder
- JavaScript in `js/` folder
- Blog posts in `posts/` folder

### 3. Customize Content
Edit the HTML files to add your:
- Name and bio
- Projects
- Blog posts
- Contact information
- Social media links

### 4. Deploy
```bash
git add .
git commit -m "Initial commit - modern static site"
git push origin main
```

Your site will be live at `https://your-username.github.io` within a few minutes!

## Features

✅ **No build process required** - Pure HTML/CSS/JS
✅ **Responsive design** - Works on all devices
✅ **Modern aesthetics** - Clean, minimal design
✅ **Fast loading** - Optimized performance
✅ **Easy to maintain** - Simple file structure
✅ **SEO friendly** - Semantic HTML
✅ **Accessible** - WCAG compliant

## Adding New Blog Posts

Create a new HTML file in the `posts/` folder:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Post Title - Your Name</title>
    <link rel="stylesheet" href="../css/style.css">
</head>
<body>
    <nav class="nav">
        <div class="nav-container">
            <a href="../index.html" class="nav-logo">Your Name</a>
            <ul class="nav-menu">
                <li><a href="../index.html">Home</a></li>
                <li><a href="../about.html">About</a></li>
                <li><a href="../projects.html">Projects</a></li>
                <li><a href="../blog.html">Blog</a></li>
                <li><a href="../contact.html">Contact</a></li>
            </ul>
        </div>
    </nav>

    <main class="container">
        <article class="post-content">
            <h1>Your Post Title</h1>
            <p class="post-meta">January 19, 2026</p>
            
            <!-- Your content here -->
            
            <a href="../blog.html" class="button">← Back to Blog</a>
        </article>
    </main>

    <footer class="footer">
        <p>&copy; 2026 Your Name. All rights reserved.</p>
    </footer>
</body>
</html>
```

Then add a link to it in `blog.html`.

## Customization

### Colors
Edit the CSS variables in `css/style.css`:
```css
:root {
    --primary-color: #2563eb;
    --text-color: #1f2937;
    --bg-color: #ffffff;
    --secondary-bg: #f9fafb;
}
```

### Fonts
The default font is system fonts for fast loading. To use custom fonts, add to `<head>`:
```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
```

### Adding Analytics
Add before closing `</body>` tag:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR-GA-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR-GA-ID');
</script>
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## License

This template is free to use for personal and commercial projects.
