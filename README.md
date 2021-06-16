# ageingonthemove

Microsite for the Report:  __A dignity claim: Ageing on the move__

## What's a microsite and when to use it?

A microsite is a single web-page or a small cluster of web pages that exist separate from the organization main website and is used for specific campaign. To this rgard a microsite can have its own domain or unique URL and a different and distinctive branding. Microsite can typically be built to highlight content from joint study and research process, following a data collection exercise.

Using a __reproducible analysis__ approach, the following workflow can be used:

 1. After data collection in [kobotoolbox](https://kobo.unhcr.org) and one data has been deposited and documented on [RIDL](https://ridl.unhcr.org/), an __initial data crunching report__ can be generated. This can be done with [koboloadeR](https://unhcr.github.io/koboloadeR/docs/). Ideally both the data crunching notebook source (i.e Rmd file) and output (i.e. html, docx or pptx) should also be recorded in RIDL. 
 
 2. The Data analysis expert should then select from within the initial crunching report, the specific figures/charts that are more likely to generate interesting joint data interpretation and compile a new refined & smaller notebook to output some __joint data interpretation presentation material__. The content of the notebook should take in consideration the data literacy levels of the participants to the data interpretation sessions.
 
 3. Joint data interpretation sessions are key to establish common understanding, compensate lack of evidence with expert judgment, resolve inconsistencies in the data, agree on priorities and develop likely scenarios/programmatic recommendations. All steps are well explained in this [video from IFRC](https://www.youtube.com/watch?v=0jE-Y7g88K4&feature=youtu.be&t=2305). The output of the session are __data interpretation notes__ that can be included back in the notebook used to create the initial presentation and archived in [UNHCR Internal Analysis repo](http://analysis.unhcr.org). A last round of comments, regional peer review and validation than can be organized directly through the [UNHCR Internal Analysis repo](http://analysis.unhcr.org)
 
 4. The last step is to produce depending on the context, only a short __microsite__ or a short microsite plus a more in-depth report. For in-depth report, UNHCR Analyst can use the paginated template from [unhcRstyle package](https://unhcr-web.github.io/unhcRstyle/docs/).


## Why a re-usable microsite template? 

This repository can be used as a template to __generate microsite__. The aim is to reproduce the look-and-feel from other UNHCR microsites like: 

 * [Desperate journeys](https://www.unhcr.org/desperatejourneys/)
 * [Families on the run](https://familiesontherun.org/)
 * [Her Turn](https://www.unhcr.org/herturn/)
 * [Stepping Up](https://www.unhcr.org/steppingup/)
 * [Home Visit Report](https://unhcr-jordan.github.io/home-visit-report)
 
The report generated through this repository is available here: [A dignity claim: Ageing on the move](https://unhcr-americas.github.io/ageingonthemove).

## Functional requirement for a microsite template

In order to ease the development of microsite, making a re-usable template is the initial requirement. Such template is expected to address the following functional requirements; 

 1. The template should use a basic and easy to learn __[markdown](https://www.markdownguide.org/cheat-sheet/)  syntax__ allowing users to avoid coding any additional  html/css/javascript. 
 
 2. The template should allow to integrate with [Rmd](https://rmarkdown.rstudio.com/) template would facilitate the full integration of reproducible analysis and the generation of charts following UNHCR brand and as implemented in the [unhcRstyle package](https://unhcr-web.github.io/unhcRstyle/docs/).
 
 3. The resulting microsite should be fully responsive (aka works on smartphone, tablet, laptop and desktop with various screen size).
 
 4. The template should include different ways to highlight contents (boxes, side note), include sufficient social sharing capacity (posting on facebook or twitter) and include [parallax scrolling effects](https://www.wix.com/blog/2019/08/what-is-parallax-scrolling-explained-with-examples/) with picture to better separate the content
 
 5. The template should be independent from any Content Management System (CMS) and work with a Website Building script transforming the initial markdown file into static html site. The website building script should be open source in order to allow for the microsite to be developed collaboratively through a [github repository](https://happygitwithr.com/).
 
 6. The template should integrate with standard UNHCR SEO/UX/tracking features


 
 
## Current template prototype  

The template presented in this repository is based customized version of the [distill package](https://rstudio.github.io/distill/website.html) with allows to generate Statis html stie through built-in building capacity in [Rstudio](. A good overview of website creation with distill is here: https://rstudio4edu.github.io/rstudio4edu-book/make-distill.html and here https://themockup.blog/posts/2020-08-01-building-a-blog-with-distill/ - If you are not yet familiar with git, check this intro: https://happygitwithr.com/


At this stage, the template still have issues that remain to be fixed:

 *  Parallax images not working well on certain smartphone models (Iphone) - see [ticket](https://github.com/rstudio/distill/issues/385).
 *  Hamburger menu icon on mobile is very small, toggles out incorrectly and the logos disappear - see [ticket on site navigation](https://github.com/rstudio/distill/issues/210).  
 *  GTM and Google Analytics code snippets do not integrate well in the template. Need to test this [integration](https://rstudio.github.io/distill/website.html#google-analytics)
 *  The social sharing script are not perfectly integrated  [See instruction to test here](https://www.shamindras.com/posts/2019-07-31-shrotriya2019distillpt2/#step-4-add-blog-post-sharing-options).
 *  Images lazyloading is not integrated  see potential with [lazyrmd](https://github.com/hafen/lazyrmd) - see [ticket](https://github.com/rstudio/distill/issues/386)
 *  Some unnecessary font (FontAwesome) and library (AutoComplete) are loaded by default.


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

The term cognitive load refers to the amount of working memory resources used to process a piece of information. The better designed is a message the more chances, people will retain it. In order to do that: 

 * Highlight the main __call to action__ in the  microsite subtitle 
 
 * Start with the main __recommendations__ to ensure the readers does not need to wait 10 minutes of reading to find out what the report message is... if not, drop out risk are high.... 
 
 * Aim to be __minimalistic__: The [ideal length of an article](https://torquemag.io/2018/04/optimal-content-length/) should be between 1500 and 2500 characters, taking an average 7 minutes to read. 

 * Have a 2 or 3 main __top level chapters__ max - avoid presenting content in too many chapter to minimize the cognitive cost for reader to absorb the content.  

 * Minimize __overwhelming effects__ by avoiding putting [too many numbers](https://www.unhcr.org/innovation/wp-content/uploads/2018/02/InnovationYearInReview2017_web.pdf#page=21) to avoid [psychic numbing](https://www.arithmeticofcompassion.org/psychic-numbing)
 
 * Do implement [story telling techniques](https://www.unhcr.org/innovation/wp-content/uploads/2019/04/Innovation18-19-WebApril2019.pdf#pag=23) - A good __data story__ is a way to communicate valuable insights and assign meaning and context to data that otherwise lives as numbers in an Excel spreadsheet. The narrative shall have a hook, momentum, or a captivating purpose. Finding such narrative structure is therefore a prerequisite. Such stories can be categorized according to the four main narrative frames below, each of them being linked to programs design or implementation. The presented data shall reflect the operation context to reinforce what readers knows or to reveal what they don’t:
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

"_Active reading_" techniques are used by many professionals and consist in , __before reading the article content__, looking at ad scanning any titles, subheadings, charts, graphs, and captions to get the key messages. 

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

As advised by the [Global protection cluster](https://www.globalprotectioncluster.org/wp-content/uploads/Protection-Analysis-Update-Template_FINAL.docx), it is key to check appropriateness of images 
 * Avoid individual or close up pictures of people who can be identified.
 * Avoid pictures of protection actors having a conversation with a group.
 * Do select pictures of a whole areas (e.g. a whole camp or settlement, or pictures where people cannot be identified, 
 * Do select pictures of protection actors in action to show the work done – include a caption that explains the work being done, to achieve better protection or reduce risks. 

In addition, If the pictures you have includes persons that can be recognized, do not include those that present the person in a state of despair.  An emotional state of despair can easily be conveyed by pictures that do not include recognizable faces.

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

When inserting a video, best is to upload it first in youtube or other video streaming platform (like vimeo) and use the built-in embedded video viewer.

In Youtube, click on share and use the embedded html snippet

`<iframe width="415" height="415" src="https://www.youtube.com/embed/***Video_ID***?controls=0&autoplay=1&playlist=***Video_ID***&loop=1&modestbranding=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>`

When adding a video, you may append different element to the video URL

 * `&autoplay=1` start automatically the video
 * `&playlist=***Video_ID***&loop=1` loop the video around..



## User experience

### organise site headers and footers

`_site.yml` is the file where site navigation bar is being configured, while `_footer.html` is used for the footer.

See also customization advice from https://rstudio4edu.github.io/rstudio4edu-book/rmd-dress.html 

You can organize [site navigation](https://rstudio.github.io/distill/website.html#site-navigation) also in `_site.yml`

Some interesting hints there: https://www.jhelvy.com/posts/2021-03-25-customizing-distill-with-htmltools-and-css/ 

### URL and Search Engine Optimisation (SEO)

beside the elements already discussed above, (i.e. mobile friendliness & responsiveness which already built-in through the template together with optimized images as explained before),  SEO-related factors to consider are:   
 * meta tags, aka a list of key words that needs to be defined in the initial chunk (see  here: https://rstudio.github.io/distill/metadata.html and https://themockup.blog/posts/2021-03-21-including-and-meta-tagging-extra-content-in-a-distill-blog/), 
 * inbound and outbound links (links  to other content), 
 * domain name & URL structure be carefully selected



## Add multiple language 

You can create a fully translated copy of you site:

 * Keep the original site in English  
 
 * create a new site (including a new `_site.yml` with translated links..) under a subfolder (good to use ISO 2 letters) - for instance `es`.  
 
 * once your build the website, copy the content generated in `/es/doc` within a new folder in doc: `/doc/es`  
 
 * Adjust the navbar content of your respective `_site.yml` to include the language switch...
 
 

