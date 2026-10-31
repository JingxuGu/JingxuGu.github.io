# Academic Personal site of Jingxu Gu

## Automatically typeset with markdown

## Directory layout

```text
index.html              # Homepage
pages/                  # Section pages, each with its own index.html
  awards/
  news/
  project/
  publications/
md/                     # Markdown content and site configuration
assets/
  hat.ico               # Site icon
  media/                # Videos and other media
  photos/               # Profile and content images
  pdf/                  # CV and publication PDFs
static/
  css/                  # Stylesheets
  js/                   # Scripts and bundled libraries
```

Edit page content in `md/<section>.md`; shared text is in `md/config.yml`.
Use `### YYYY-MM-DD` headings for dates on all section timelines; month-only
dates such as `### 2026.06` are also supported.
Project images and videos show an English loading indicator until ready,
or an error message if the resource cannot be loaded.
Section URLs use `/pages/<section>/`; the homepage stays at `/`.
Use root-relative asset paths such as `/assets/photos/photo.jpeg` and
`/assets/media/yolo26.mp4` so links work from every section page.

To preview locally, run `python3 -m http.server 8000` from the repository root
and open [the homepage](http://localhost:8000/).

## Adding project media

insert photos:

```
- ![proj_name](/assets/photos/example.jpg) **proj_title**\
  project description. 
```

insert vedios:

```
- <video src="/assets/media/example.mp4"></video> **proj_title**\
  project description. 
```
