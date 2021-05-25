# ageingonthemove

Microsite for the Report:  __A dignity claim: Ageing on the move__

## What's a microsite and when to use it?

A microsite is a single web-page or a small cluster of web pages that exist separate from the organization main website and is used for specific campaigns. A microsite will have its own domain or unique URL and the branding of it may differ from the brand’s usual one. 

It can typically be built to highlight content from joint study and research process.

Using a reproducible analysis approach, the following workflow can be used:

 1. After data collection in [kobotoolbox](https://kobo.unhcr.org) and one data has been deposited and documented on [RIDL](https://ridl.unhcr.org/), an __initial data crunching report__ can be generated. This can be done with [koboloadeR](https://unhcr.github.io/koboloadeR/docs/). Ideally both the data crunching notebook source (i.e Rmd file) and output (i.e. html, docx or pptx) should also be recorded in RIDL. 
 
 2. The Data analysis expert should then select from within the initial crunching report, the specific figures/charts that are more likely to generate interesting joint data interpretation and compile a new refined & smaller notebook to output some __joint data interpretation presentation material__. The content of the notebook should take in consideration the data literacy levels of the participants to the data interpretation sessions.
 
 3. Joint data interpretation sessions are key to establish common understanding, compensate lack of evidence with expert judgment, resolve inconsistencies in the data, agree on priorities and develop likely scenarios/programmatic recommendations. All steps are well explained in this [video from IFRC](https://www.youtube.com/watch?v=0jE-Y7g88K4&feature=youtu.be&t=2305). The output of the session are __data interpretation notes__ that can be included back in the notebook used to create the initial presentation and archived in [UNHCR Internal Analysis repo](http://analysis.unhcr.org). A last round of comments, regional peer review and validation than can be organized directly through the [UNHCR Internal Analysis repo](http://analysis.unhcr.org)
 
 4. The last step is to produce depending on the context, only a short __microsite__ or a short microsite plus a more in-depth report. For in-depth report, UNHCR Analyst can use the paginated template from [unhcRstyle package](https://unhcr-web.github.io/unhcRstyle/docs/)


## A re-usable microsite template 

This repository can be used as a template to __generate microsite__. It uses a customized version of the [distill package](https://rstudio.github.io/distill/website.html). The advantage of this approach is to develop quickly a microsite without coding any html/css/javascript as the content will be only a [mark-down document](https://www.markdownguide.org/cheat-sheet/).  In addition, because it based on R, it becomes very easy to include charts, graphs and other data visualizations.

The aim is to reproduce the look-and-feel from other UNHCR microsite like: 

 * [Desperate journeys](https://www.unhcr.org/desperatejourneys/)
 * [Families on the run](https://familiesontherun.org/)
 * [Her Turn](https://www.unhcr.org/herturn/)
 * [Stepping Up](https://www.unhcr.org/steppingup/)
 * [Home Visit Report](https://unhcr-jordan.github.io/home-visit-report)
 
The report generated through this repository is available here: [A dignity claim: Ageing on the move](https://unhcr-americas.github.io/ageingonthemove)

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

 * Highlight the main __call to action__ in the  microsite subtitle 
 
 * Start with the main __recommendations__ to ensure the readers does not need to wait 10 minutes of reading to find out what the report message is... if not, drop out risk are high.... 
 
 * Aim to be __minimalistic__: The [ideal length of an article](https://torquemag.io/2018/04/optimal-content-length/) should be between 1500 and 2500 characters, taking an average 7 minutes to read. 

 * Have a 2 or 3 main __top level chapters__ max - avoid presenting content in too many chapter to minimize the cognitive cost for reader to absorb the content.  

 * Avoid putting [too many numbers](https://www.unhcr.org/innovation/wp-content/uploads/2018/02/InnovationYearInReview2017_web.pdf#page=21) to avoid psychic numbing
 
 * Do implement [story telling techniques](https://www.unhcr.org/innovation/wp-content/uploads/2019/04/Innovation18-19-WebApril2019.pdf#pag=23) - A good data story is a way to communicate valuable insights and assign meaning and context to data that otherwise lives as numbers in an Excel spreadsheet. The narrative shall have a hook, momentum, or a captivating purpose. Finding such narrative structure is therefore a prerequisite. Such stories can be categorized according to the four main narrative frames below, each of them being linked to programs design or implementation. The presented data shall reflect the operation context to reinforce what readers knows or to reveal what they don’t:
    1.	shed light on a previously unexplored topic (it teaches people something new or they have not heard before), 
    2.	introduce an interesting angle (gives them a new perspective) 
    3.	provide useful suggestions to solve a problem (inspires to act) 
    4.	disprove a hypothesis / debunk a widely held belief in terms of programmatic assumption.
    
 * Be __persuasive__ for instance by shaping your narrative with the [aforsest techniques](https://www.youtube.com/watch?v=jgyKm11PYWw):
    A - Alliteration.
    F - Facts.
    O - Opinions.
    R - Rhetorical questions.
    E - Emotive language.
    S - Statistics.
    T - (Three) rule of.

### Highlight Content to ease "_active reading_"

"__Active reading__" techniques are used by many professionals and consist in , __before reading the article content__, looking at ad scanning any titles, subheadings, charts, graphs, and captions to get the key messages. 

Those techniques allow to get the main messages of any document without reading it line by line... it is used in most medias nowadays

#### 1. Paragraph Titles as statement

Title should be turned into meaningful statement/ summary - rather than referencing the topic explained in the chapter text 

#### 2. Bold Keywords

Use bold with parsimony - only for key words.

In the template, this can be done with the following tags:

`__quoted word__` are defined with double 

#### 3. Outline Key Quotes


In the template, this can be done with the following tags:

`> quoted text`

#### 4. Insert content to be tweeted

__Make the site ready for social media sharing__: Prepare Key messages (less than 144 character) ready to be tweeted and add a "share" button close to the specific quote .  

In the template, this can be done with the following tags:

`<p class="tweetable"> text for tweet </p>`

#### 5. Add boxed messages 

On the top of article text, add side note to highlight some key elements.

In the template, this can be done with the following tags:

`<aside> text for box </aside>` 

#### 6. Insert Human Stories 

It is crucial to always pair quantitative analysis with human stories to increase the persuasiveness of the content. 

In the template, this can be done with the following tags:

`<div class="story">  STORY: Older Colombians and Venezuelans take care of each other under the same roof. text for box </div>` 


## Insert images

### Select the right pictures

UNHCR has its own media library that can be used to search and select pictures: [https://media.unhcr.org/](https://media.unhcr.org/).

When selecting pictures for a report, as pointed in the report: [Aid recipients call for more dignity and diversity in INGO campaigns](https://www.radiaid.com/aid-recipients-call-for-more-dignity-and-diversity): "_Aid communication still needs to move away from presenting the single story: Why not try to create a sense of hope or provide inspiration to the viewer, instead of primarily provoking feelings of despair?_"

Practically speaking this implies;

 * Avoid putting pictures of persons that can be easily recognized
 * If the pictures you have includes persons that can be recognized, do not include those that present the person in a state of despair.  An emotional state of despair can easily be conveyed by pictures that do not include recognizable faces.


#### First resize them


It is important that you optimize their size for the context in which they will be published. Saving your images with appropriate dimensions and optimizing images for the web can help with a few things:

 * Speed – if a web page loads in more than 5 seconds, the probability that a mobile user will leave that page increases by 90%. By resizing and reducing image sizes, you make your website pages faster.
 
 * User experience – good quality, impactful images helps visitors have a more engaging experience while they browse your website. By keeping those images optimized and loading fast – you’re ensuring a seamless and smooth experience for your visitors, which motivates them to spend more time on your site and explore your content.
 
 * SEO ranking – site speed is a ranking factor. The faster is your site, the better you can potentially rank. Web pages with optimized images will load much quicker on both desktop and mobile devices.
 

To ensure that your full width images look good across any device big or small the recommended size is max 2000px width. If inside the page, then a width of 1080px is recommended. Large images or full-screen background images should be no more than 1 MB.

According to this [tutorial](https://www.smashingmagazine.com/2015/06/efficient-image-resizing-with-imagemagick), the following command line will effectively resize all the image from the folder within it is being run into optimal 1080 pixel width images



`mogrify -filter Triangle -define filter:support=2 -unsharp 0.25x0.25+8+0.065 -dither None -posterize 136 -quality 82 -define jpeg:fancy-upsampling=off -define png:compression-filter=5 -define png:compression-level=9 -define png:compression-strategy=1 -define png:exclude-chunk=all -interlace none -colorspace sRGB -strip -units PixelsPerInch -density 92  -resize 1080  *.png`


### background image

For responsive design, the image needs to be crop-able in both portrait (for smartphone) and landscape (for desktop). Changing between those 2 formats is handled in the css file  `theme.css`

#### Above the fold

“Above the fold” refers to web content that is visible above the border when a page first loads.

The background image is called in `theme.css`, with  the correct path to image (or just overwrite the corresponding image in : `images/header.jpg`)

`> d-title {`
`>   background-image: url(images/header.jpg);`
  

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
 

## Adding videos

Individual files in a github repository are strictly limited to a 100 MB maximum size limit.

When inserting a video, best is to upload it first in youtube or other video streaming platform (like vimeo) and use the built-in embedded video viewer

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



