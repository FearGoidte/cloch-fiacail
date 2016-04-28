<h1 xml:lang="ga">Cloch fiacail</h1>

![](images/cloch-fiacail.svg?raw=true)

There are numerous ways to start a style sheet and numerous ways to organize them. Unfortunately there is no right way, and yet plenty of wrongs ones.

I have based this general purpose style sheet upon The <abbr title="World Wide Web Consortium" class="initialism">W.3.C.</abbr>’s [10.2 The <abbr title="Cascading Style Sheets" class="initialism">C.S.S.</abbr> user agent style sheet and presentational hints](https://www.w3.org/TR/html5/rendering.html#the-css-user-agent-style-sheet-and-presentational-hints) as at <time datetime="2016-02-17">17<sup>th</sup> February 2016.</time> The intended audience for that stylesheet is *not* web developers but makers of visual agents. Nevertheless the organization of the elements and properties does have a certain logic.

I have reformatted for error-checking and resorted properties alphabetically.
I have only included quotation marks for English.

Gradually I will make additions and changes based on use.

## Organization

I have split the rules into the following partials:

* `_code-highlighting`
* `_print`
* `_screen`
* `_visual`

### <abbr title="Syntactically Awesome Style Sheets" class="initialism">SASS</abbr> variables

To make it easier to share the partials between projects, I have added some variables to the stylesheets. All the following variables must be specified for all of the partials to work correctly:

#### `$baseline`

The line height of the `html` element and used to calculate margins and line heights for other elements.

#### `$body-font-family`

The fonts used for the `html` element.

#### `$code-font-family`

The fonts used for the `code`, `kbd`, and `samp` elements.

#### `$heading-font-family`

The fonts used for the `header`, `h1`–`h6`, and `th` elements as well as elements with the `role` attribute “`banner`”.

#### `$background-colour`

The background colour for the the `html` element when displayed on a screen.

#### `$base-colour`

The main body-text colour for screen displays.

#### `$link-colour`

The colour for unvisited links. Best practise is a variation on theme of ‘blue’.

#### `$link-colour-visited`

The colour for visited links. Best practise is a variation on theme of ‘purple’.

#### `$logo-colour`

Principal colour used in logo or used to create identity.

## Significant deletions

### Obsolete elements

I have removed the items obsolete in <abbr title="Hypertext Mark-up Language" class="initialism">H.T.M.L.</abbr>5:

* `acronym`,
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

I have also removed selectors for the ‘purely’ styling elements deprecated prior to <abbr title="Hypertext Mark-up Language" class="initialism">H.T.M.L.</abbr>5 and then reintroduced by that version and given a semantic garnish ([The <abbr title="Hypertext Mark-up Language" class="initialism">H.T.M.L.</abbr> 4.01 Font style elements](https://www.w3.org/TR/html401/present/graphics.html#h-15.2.1)):

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

### Attributes

I have removed the following deprecated or non-standard attributes:

* `align`,
* `border`,
* `clear`,
* `color`,
* `frame`,
* `noshade`,
* `nowrap`,
* `rules`, and
* `valign`.

### Other deletions

The bi-directional stylings and the bindings stylings. I never make use of those properties so they are best left to the visual agent rather than me.

I removed the [<abbr title="Cascading Style Sheets" class="initialism">C.S.S.</abbr> Selectors Level 4 modifier for ASCII case-insensitive attribute values selection](https://drafts.csswg.org/selectors-4/#attribute-case) since [attributes are case-sensitive in <abbr title="eXtensible Hypertext Mark-up Language" class="initialism">X.H.T.M.L.</abbr>](https://www.w3.org/TR/xhtml1/#h-4.2)

## Changes and additions

Added ‘editor’-style formatting for `mark` elements within a `blockquote`.

Reformatted the `hr` element to display an [asterism](https://en.wikipedia.org/wiki/Asterism_%28typography%29) with a faded line background.

Removed underlines from abbreviations since their title attributes cannot be accessed on many touch devices. Added the help cursor for keyboard and mouse users.

### Headings

Removed the rules for nested `h1` headings for sections since whilst, it is valid use under the <abbr title="Hypertext Mark-up Language" class="initialism">H.T.M.L.</abbr>5 Recommendation, it is poorly supported and I think it better to follow the [User’s Guide to <abbr title="International Organization for Standardization" class="initialism">I.S.O.</abbr>/<abbr title="International Electrotechnical Commission">I.E.C.</abbr> 15445:2000 HyperText Markup Language](https://www.cs.tcd.ie/misc/15445/UG.HTML#H1.NEST).

Also switched `h1`-`h6`, `header`, and `th` from bold to a different typeface.

### Lists

Replaced automatic lists with lists using the `::before` pseudo elements nested up to five levels deep.

Also added `serial-comma` class for inline [Oxford comma](https://en.wikipedia.org/wiki/Serial_comma) style lists.

## Copyright

This work, such as it is, is free to use with or without attribution and under any terms that do not obligate me.
