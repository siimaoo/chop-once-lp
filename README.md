# Chop Once, Cook Faster — Landing Page

Conversion-focused static sales page for the paid ebook *Chop Once, Cook Faster*.

## Local preview

Open the HTML file in a browser:

```bash
# from this directory
xdg-open index.html
# or: python3 -m http.server 8080
```

Then visit `http://localhost:8080` if using the Python server.

## Docker (Coolify-ready)

Serves static files with nginx on port **80**.

```bash
docker build -t chop-once-lp .
docker run --rm -p 8080:80 chop-once-lp
```

Open `http://localhost:8080`.

## Buy URL

Search for `REPLACE_BUY_URL` in `index.html` and replace `https://example.com/buy` with the real checkout link.

## Stack

- Static HTML + CSS
- nginx Alpine image
- No build step, no JS framework
