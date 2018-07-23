# note 

A simple CLI perl script to help organize your text based notes. I recommend using [Markdown](http://daringfireball.net/projects/markdown/).

## Usage
Just run the **note** script.

Basically it just creates notes with a consistent naming scheme:

	YYYY-MM-DD-YourTitleHere.md

## Editor

By default **note** opens the file in `$EDITOR`.

If you want to use a dedicated editor for your notes, **note** supports using a custom editor by defining the  `$NOTE_EDITOR` environment variable. 

I recommend using some sort of Markdown editor. I personally like [macdown](http://macdown.uranusjr.com/) on OSX, but any text editor than can be fired from the terminal will work.

## Where do you store the notes?

We look for the following directories (in order) and 
use the first one we find:

* `~/Dropbox/Notes`
* `~/Documents/notes`
* `~/notes`
* `~/Documents`

If we dont find any of these, we attempt to create `~/notes`. If we can't do that we just default to `~/`