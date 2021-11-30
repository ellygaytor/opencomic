# opencomic

opencomic is a JSON webcomic syndication format, loosely based on [JSON Feed](https://www.jsonfeed.org).

It boasts the same advantages as JSON Feed; it's lightweight, and easy to handle. However, it's explicitly designed to work well for the specific needs of webcomics.

## Versions

* [v1.0](v1.0.md)

## Examples

Here are a few XKCD comics in opencomic format:

```
{
  "version": "https://opencomic.org/v1.0",
  "title": "XKCD",
  "home_url": "https://xkcd.com",
  "description": "A webcomic of romance, sarcasm, math, and language.",
  "authors": {
    "name": "Randall Munroe"
  },
  "language": "en-US",
  "expired": false,
  "pages": [
    {
      "id": 1,
      "url": "https://xkcd.com/1/",
      "title": "Barrel - Part 1",
      "title_text": "Don't we all.",
      "panels": [
        {
          "image_url": "https://imgs.xkcd.com/comics/barrel_cropped_(1).jpg",
          "alt_text": "[[A boy sits in a barrel which is floating in an ocean.]]\nBoy: I wonder where I'll float next?\n[[The barrel drifts into the distance. Nothing else can be seen.]]\n{{Alt: Don't we all.}}"
        }
      ],
      "date_published": "2006-1-1T00:00:00-00:00"
    },
    {
      "id": 2,
      "url": "https://xkcd.com/2/",
      "title": "Petit Trees (sketch)",
      "title_text": "'Petit' being a reference to Le Petit Prince, which I only thought about halfway through the sketch",
      "panels": [
        {
          "image_url": "https://imgs.xkcd.com/comics/tree_cropped_(1).jpg",
          "alt_text": "[[Two trees are growing on opposite sides of a sphere.]]\n{{Alt-title: 'Petit' being a reference to Le Petit Prince, which I only thought about halfway through the sketch}}"
        }
      ],
      "date_published": "2006-1-1T00:00:00-00:00"
    }
  ]
}
```