# HTML

## What is HTML?

- HTML(Hyper text markup language) is a markup language used to create web pages

## What is difference b/w HTML4 and HTML5?

- We will cover HTML5 only
- HTML4 --
  htm4 doesn't support latest tags
  - like --> Audio, Video, figure and fig caption
  - It doesn't support semantic tags
- html5
  - html5 has deprecated most of tags
  - like --> <acronym>,<applet>, <basefont>, <big>, <center>, <big>, <frameset>
  - It supports semantic tags like --> <main>, <section>, <em>, <strong>

## What are semantic tags?

- Sematic tags are self explanatory
- like main, area, nav, footer, header, aside, section, article, audio, video
- This is SEO friendly (Search Engine Optimization)

## What are semantic html?

- The html which preferred only semantic tags in known as Semantic HTML

## What is DOCType?

- Syntax --> <!DOCTYPE html>
- This briefed about the file --> Document Type
- This is used by browser to understand what kind of html is being used
- This represents that this file related to HTML5

## Structure of html

```
windows
└── document
    └── html
        ├── head
        │   ├── meta tags
        │   ├── title
        │   ├── favicon
        │   └── links
        └── body
            ├── div
            │   ├── p
            │   └── span
            ├── ol
            ├── ul
            └── h1
```

## Terminologies of HTML?

### What are tags in HTML?

- Anything written inside the angular braces <> is known as Tags
- Examples --> <html>, <p>, <br />

### Type of Tags

1. Opening and closing tags
   - <p> </p>, <h1></h1>, <body></body>
2. Self closing tags
   - <img />, <hr />, <br />, <input />

### What is Content?

- Whatever material or thing is used inside the tags is called content
- <p>Hello Abhi</p> ----> `Hello Abhi` is content

### What is Element?

- Entire tag from opening to closing is called element
- <p>Hello Abhi</p>  --> Element

### What are Attributes?

- The supporting elements of tags are known as attributes
- example
  - id
  - class
  - style
  - type
  - name
  - placeholder
  - src
  - alt

### comments in html

- Comment is used to provide indication or reference on the code
- <!-- any comment -->

### heading tags

- We have 6 types of heading tags
- h1, h2, h3, h4, h5, h6

### What are formatting tags?

- Those tags which are used to format or stylize the texts and fonts

1.  b (html4) -- used to bold
2.  strong (html5) -- used to bold
3.  i (html4) -- used to italic
4.  em (html5) -- used to italic
5.  mark -- use for marking with yellow background
6.  del -- (html5) -- used for strike out any text
7.  ins -- to insert any text on the place of striked out or del text
8.  strike (html4) -- used for strike out any text
9.  small -- used to make small text as compare to others
10. big --(html4) used to make bigger text as compare to others
11. sup -- used for mathematical purpose like to show power of
12. sub -- used for scientifically purpose like to show power of

### anchor tag

- Anchor tag (<a>) is used provide some external link or internal html page to redirect

### hr

- used to add divider or horizontal row or line
- <hr/>

### br

- used to break row or line
- <br/>

### img extension

1. .jpg -- normal images- pixelate
2. .png -- no background image- pixelate
3. .svg -- No background - No pixelate
4. .ico -- mostly used for favicon
5. .webp -- Better than jpeg -- Pictures are in high quality
6. .avif --
7. .hvif -- picture format clicked on iphones
8. .gif -- animated pictures

### img tags

- used to add pictures in web page
- We can use picture in 2 methods

1. online image link
2. local image

<img src='image link (online/local)' alt='alternate text' width='100px' height='100px'>
