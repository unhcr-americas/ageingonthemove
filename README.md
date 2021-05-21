# ageingonthemove

Microsite for the Report:  __A dignity claim: Ageing on the move__

## A re-usable microsite template 

A microsite is a single web-page or a small cluster of web pages that exist separate from the organization main website and is used for specific campaigns. A microsite will have its own domain or unique URL and the branding of it may differ from the brand’s usual one. 

It can typically be built to highlight content from joint study and research process.


This repository can be used as a template to __generate microsite__. It uses a customized version of the [distill package](https://rstudio.github.io/distill/website.html). The advantage of this approach is to develop quickly a microsite without coding any html/css/javascript as the content will be only a [mark-down document](https://www.markdownguide.org/cheat-sheet/).  In addition, because it based on R, it becomes very easy to include charts, graphs and other data visualizations.

The aim is to reproduce the look-and-feel from other UNHCR microsite like: 

 * [Desperate journeys](https://www.unhcr.org/desperatejourneys/)
 * [Families on the run](https://familiesontherun.org/)
 * [Home Visit Report](https://unhcr-jordan.github.io/home-visit-report)

### Markdown syntax

Markdown is a lightweight and easy-to-use syntax for styling your writing. You can use directly when creating the working version of the microsite content in word.


It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).


### “Content is King” 

### Reduce cognitive load

 * Highlight a call to action as the site subtitle 
 
 * start with the main __recommendations__ to ensure the readers does not need to wait 10 minutes of reading to find out what the report message is... if not, drop out risk are high.... 
 
 * __Be minimalistic__: The [ideal length of an article](https://torquemag.io/2018/04/optimal-content-length/) should be between 1500 and 2500 characters, taking an average 7 minutes to read. 

 * Have a 2 or 3 main __top level chapters__ max - avoid presenting content in too many chapter to minimimze the cognitive cost for reader to absorb the content.  

 * Avoid putting [too many numbers](https://www.unhcr.org/innovation/wp-content/uploads/2018/02/InnovationYearInReview2017_web.pdf#page=21) to avoid psychic numbing
 
 * implement [story telling techniques](https://www.unhcr.org/innovation/wp-content/uploads/2019/04/Innovation18-19-WebApril2019.pdf#pag=23) - A good data story is a way to communicate valuable insights and assign meaning and context to data that otherwise lives as numbers in an Excel spreadsheet. The narrative shall have a hook, momentum, or a captivating purpose. Finding such narrative structure is therefore a prerequisite. Such stories can be categorized according to the four main narrative frames below, each of them being linked to programs design or implementation. The presented data shall reflect the operation context to reinforce what readers knows or to reveal what they don’t:
    1.	shed light on a previously unexplored topic (it teaches people something new or they have not heard before), 
    2.	introduce an interesting angle (gives them a new perspective) 
    3.	provide useful suggestions to solve a problem (inspires to act) 
    4.	disprove a hypothesis / debunk a widely held belief in terms of programmatic assumption.
    


### Highlight Content to ease "_active reading_"

"Active reading" techniques consist in , __before reading the article content__, looking at any titles, subheadings, charts, graphs, and captions to get the key messages. - This allow to get the main content of the report simply by reading the table of content... it is used in most medias nowadays

#### Paragraph Titles as statement

Title should be turned into meaningful statement/ summary - rather than referencing the topic explained in the chapter text 

#### Bold key words

Use bold with parcimony - only for key words

`__quoted word`

#### Outline key quotes

`> quoted text`

#### Insert content to be tweeted

__Make the site ready for social media sharing__: Prepare Key messages (less than 144 character) ready to be tweeted and add a "share" button close to the specific quote .  

`<p class="tweetable"> text for tweet </p>`

#### Add small boxes
On the top of article text, add side note to highlight some key elements
`<aside> text for box </aside>` 



## Insert images

### bacground mage

For responsive design, the image needs to be crop-able in both portait (for smartphone) and landscape (for desktop)

#### Above the fold

“Above the fold” refers to web content that is visible above the border when a page first loads.

The background image is called in `theme.css`, with  the correct path to image (or just overwrite the corresponding image in : `images/header.jpg`)

`>` d-title {`
`>`   background-image: url(images/header.jpg);`
  

#### Parallax effect to separate the chapter

` <div class="parallax parallax1"><div class="parallax-content">`
` ## This my chapter delimiter`
` </div></div>`

in `theme.css`, define the property `parallax1` by adding the correct path to image (or just overwrite the corresponding image in : `images/parallax1.jpg`)

### Inside microsite body
 
`{r, layout="l-screen-inset"}`
`include_graphics("images/infographic1.png")`

 
layout can take the following value:
 * `l-body`  will cause content to span the width of the main article body:
 * `l-body-outset` Wider layouts
 * `l-page` Even wider
 * `l-screen` full screen
 * `l-screen-inset` full screen with a bit space at the edges
 


## User experience



### organise site headers and footers

`_site.yml` is the file where site navigation bar is being configured, while `_footer.html` is used for the footer.

See also customization advice from https://rstudio4edu.github.io/rstudio4edu-book/rmd-dress.html 

### URL and Search Engine Optimisation (SEO)

SEO-related factors to consider are:   
 * meta tags (aka a list of key words - see  here: https://rstudio.github.io/distill/metadata.html and https://themockup.blog/posts/2021-03-21-including-and-meta-tagging-extra-content-in-a-distill-blog/), 
 * inbound and outbound links (links  to other content), 
 * domain name & URL structure (URL has to be carefully selected), 
 * mobile friendliness & responsiveness (the site needs to be read-able on smartphone and large screen), 
 * design elements such as images and videos which can affect load speed (for instance image size needs to be reduced).



