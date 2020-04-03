# Portfolio Website - Sass, CSS and HTML
### URL: https://adrian-sal-kennedy-dev.netlify.com  
### source: https://github.com/adrian-sal-kennedy/portfolio-project  

## Rationale
A decent personal brand needs a decent personal website. This site may one day become that for me.  

I've included some film industry work mainly for interest - though I'm fairly well quit with freelance film, my interests and aptitude are still very much tied to it and I have a wealth of tools I've developed over the years that I would really love to start doing justice on and releasing to the world (sometimes for a fee, mostly not).  

I'm definitely going to build the blog feature much further as time goes on. I would ideally like to have some server-side stuff that watches a folder for markdown files and injects them into the page. Markdown is much easier to blog in than html. I'll be putting all kinds of geeky explorations up there. Right now it's just got some book quotes.  

## Design
I started with movie posters. For some reason Sergio Leone popped into my head and I welcomed the idea as it presented some interesting-looking challenges for CSS styling.

### Responsive Design
One thing the movie-poster idea afforded was several international versions in different formats in roughly the same theme. One thing that came up was large red skewed rectangles coming in at offsets. This had been used in both portrait (with horizontal red rectangles) and landscape (with vertical red strips), and this seemed to be very compatible with mobile vs desktop experiences.  

One issue I had was that mobiles, browsers, everything do not have their real-world resolutions. especially desktops all just pretend it's 1999 and they're 96dpi, even if they're 166dpi, 192, or the 469dpi that my phone is.  

Pixels in CSS are not real pixels. I decided to scale by root em-size but that still had problems in mobile. I've commented out almost all this CSS logic and will add it back when I figure it out.

### Accessibility
Semantic elements were used everywhere there was actual content to be delivered. The background images were not included in this because I considered them part of the layout, though they could be argued to need annotation as well for screen readers. They are not included in the html itself so I consider them to be styling rather than content.

## Walkthrough video
[![screenshot of a terminal in ubuntu](https://i.vimeocdn.com/video/872645067_640.jpg)](https://vimeo.com/403254239)

- basic walkthrough of function
- design approach
- responsive portrait/landscape demo
- wireframe (balsamiq)
- trello
- mood board (pinterest)

## Future work
I definitely wish to build this into a full-fledged portfolio site. I'm aware that it's more in the informal side of things, but I'm not concerned with that overly; my philosophy is if a prospective employer cannot deal with a bit of personality while still maintaining a functional site, this is an issue that would come up again and again beyond the recruitment stage.  

Some features I'd like to implement:
- scraping markdown files from a "blog" folder that I can push to. Easy, no need for a CMS, and elegant. These markdown files would be parsed and injected into the blog page, with date elements up the top left.
- complete rewrite of CSS to un-hack it and make the behaviour way more predictible. I admit the current code is a mess, and hindsight would have me do this with more modularity.
- contact page that sends emails to me.