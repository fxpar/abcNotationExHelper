# abcNotationExHelper
Javascript tool to help hardcode html pages of music exercises written in abc notation

## Purpose
This is a simple javascript tool to turn every textarea of the page into an ABC editor and player. It is intended to help hardcode html pages of music exercises.

The abc code can be modified at runtime but the changes are not saved in a browser session.

## Usage
Add a textarea in the page with an id starting by "abc_ex_". Put the ABC code of your song or exercise inside the textarea. For example
```html
<textarea id="abc_ex_001">YOUR ABC CODE HERE </textarea>
```
## Result
For each textarea with an id starting with "abc_ex_":

* [x] The music sheet is created
* [x] The audio player is added
* [x] The warnings are provided
* [x] The abc code is placed into an standard collapsible (Details/Summary)

## Personal application
I needed an easy way to write html pages to play offline on my mobile. 

It is meant to work with a simple http server. The orginal abc-basic.js has been modified to check local audio sounds before trying to download them. (the page needs to be served by http server to avoid CORS error)

Otherwise the exercises are on my wordpress pages.

## Credits
* It refers to the ABC Notation format proposed by Chris Walshaw.
* It is based on the abcjs open source project written by Paul Rosen and Gregory Dyke.
* It is an adaptation of Hieu-Thi Long's online tool.
* Soundfonts for acoustic piano has been added for local server

## Demo 
https://fxpar.github.io/abcNotationExHelper/

🎶Cheers
