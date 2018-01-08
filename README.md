# html-media-flicker

Was an idea from an Anonymous in 4chan, but I am too dumb to write a proper Android application.

Uses the `no-referrer` policy in order to bypass some websites that do referrer checking to prevent hotlinking. Only [latest browsers are supported](https://caniuse.com/#feat=referrer-policy), of course.

- [Bootstrap v4](https://getbootstrap.com/)
- [jQuery](https://jquery.com/)
- [Bowser](https://github.com/lancedikson/bowser)
- [some super small files](https://github.com/mathiasbynens/small)


## Example file format

**Guess Mode**, where the application attempts to guess the file type based on the URL provided in text file.

```
https://i.imgur.com/AdfU8FT.png
https://s1.webmshare.com/azr96.webm
```

**Descriptive Mode**, where the application gets informed on how to load the URL. (Essentially a JSON file.)

```
[
  { "url": "https://i.imgur.com/AdfU8FT.png", "type": "image" },
  { "url": "https://webmshare.com/play/azr96", "type": "video" }
]
```
