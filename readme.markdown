<h1 xml:lang="la">Ex nihilo</h1>

There are numerous ways to start a style sheet and numerous ways to organize them. Unfortunately there is no right way, and yet plenty of wrongs ones.

I have based this general purpose style sheet upon The <abbr title="World Wide Web Consortium" class="initialism">W.3.C.</abbr>’s [10.2 The <abbr title="Cascading Style Sheets" class="initialism">C.S.S.</abbr> user agent style sheet and presentational hints](https://www.w3.org/TR/html5/rendering.html#the-css-user-agent-style-sheet-and-presentational-hints) as at <time datetime="2016-02-17">17<sup>th</sup> February 2016.</time> The intended audience for that stylesheet is *not* web developers but makers of visual agents. Nevertheless the organization of the elements and properties does have a certain logic.

I have reformatted for error-checking and resorted properties alphabetically.
I have only included quotation marks for English.

Gradually I will make additions and changes based on use.

## Significant deletions

### Obsolete elements

I have removed the items obsolete in <abbr title="Hypertext Mark-up Language" class="initialism">H.T.M.L.</abbr>5:

* `applet`,
* `basefont`,
* `big`,
* `blink`,
* `center`,
* `dir`,
* `listing`,
* `noembed`,
* `noframes`,
* `plaintext`,
* `strike`,
* `tt`, and
* `xmp`.

### Styling elements

I have also removed selectors for the ‘purely’ styling elements deprecated prior to <abbr title="Hypertext Mark-up Language" class="initialism">H.T.M.L.</abbr>5 and then reintroduced by that version an given a semantic garnish ([The <abbr title="Hypertext Mark-up Language" class="initialism">H.T.M.L.</abbr> 4.01 Font style elements](https://www.w3.org/TR/html401/present/graphics.html#h-15.2.1)):

* `b`,
* `i`,
* `s`,
* `small`, and
* `u`.

Whilst they have been given semantic meanings, they seem thin and redundant. <abbr title="Hypertext Mark-up Language" class="initialism">H.T.M.L.</abbr>5 is bloated enough without these elements.

### Ruby annotations

I have removed the Ruby elements:

* `ruby`,
* `rb`,
* `rbc`,
* `rp`,
* `rt`, and
* `rtc`.

### Other deletions

As well as the bi-directional stylings and the bindings stylings. I never make use of those properties so they are best left to the visual agent rather than me.

I removed the [<abbr title="Cascading Style Sheets" class="initialism">C.S.S.</abbr> Selectors Level 4 modifier for ASCII case-insensitive attribute values](selection]https://drafts.csswg.org/selectors-4/#attribute-case) since [attributes are case-sensitive in <abbr title="eXtensible Hypertext Mark-up Language" class="initialism">X.H.T.M.L.</abbr>](https://www.w3.org/TR/xhtml1/#h-4.2)

## Changes and additions

Added ‘editor’-style formatting for `mark` elements within a `blockquote`.

## Copyright

This work, such as it is, is free to use with or without attribution and under any terms that do not obligate me.