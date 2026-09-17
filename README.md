# HacKSU Presentation Template

A slide deck template to use for HacKSU workshops.

```
static/
  app.js                  slide navigation and particle background
  style.css               HacKSU deck design
templates/
  slides/                 slide files
  base.html               page shell, nav bar, logo
  index.html              slide order
  notes.html              speaker notes and run of show
app.py                    base app, three routes: deck, notes, logo
README.md                 documentation
requirements.txt          dependencies
```

A Flask app on port 5174.

Install dependencies: 

`pip install -r requirements.txt`

To run the app:

`python app.py` or `flask app`

`/` is the deck, navigated with arrows, space, or the dots.

`/notes` is the speaker notes with a minute-by-minute run of show.

To change the order of slides, navigate to `templates/index.html`, and reorder using `{% include %}`

Design and plumbing lifted from the polyglot programming deck.
