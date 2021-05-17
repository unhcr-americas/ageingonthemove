# ageingonthemove

Microsite for the Report:  __A dignity claim: Ageing on the move__

## A re-uable microsite template 

This repository can be used as a template to __generate microsite__. It uses a customized version of the [distill package](https://rstudio.github.io/distill/website.html). The advantage of this approach is to develop quickly a microsite without coding any html/css/javascript as the content will be only a [mark-down document](https://www.markdownguide.org/cheat-sheet/).  In addition, because it based on R, it becomes very easy to include charts, graphs and other data visualizations.

The aim is to reproduce the look-and-feel from other UNHCR microsite like: 

 * [Desperate journeys](https://www.unhcr.org/desperatejourneys/)
 * [Families on the run](https://familiesontherun.org/)
 * [Home Visit Report](https://unhcr-jordan.github.io/home-visit-report)
 
## Tips for creating microsite

A microsite is a single web-page or a small cluster of web pages that exist separate from the organization main website and is used for specific campaigns. A microsite will have its own domain or unique URL and the branding of it may differ from the brand’s usual one. 

It can typically be built to highlight content from joint study and research process.

### URL and Search Engine Optimisation (SEO)

SEO-related factors to consider are:   
 * meta tags (aka a list of key words - see  here: https://rstudio.github.io/distill/metadata.html and https://themockup.blog/posts/2021-03-21-including-and-meta-tagging-extra-content-in-a-distill-blog/), 
 * inbound and outbound links (links  to other content), 
 * domain name & URL structure (URL has to be carefully selected), 
 * mobile friendliness & responsiveness (the site needs to be read-able on smartphone and large screen), 
 * design elements such as images and videos which can affect load speed (for instance image size needs to be reduced).

### Structure the content: “Content is King” 

 * Highlight a call to action as the site subtitle

 * have a 2 or 3 main top level chapters max - avoid presenting content in too many chapter to minimimze the cognitive cost for reader to absorb the content.  
  
 * start with the main recommendations to ensure the readers does not need to wait 10 minutes of reading to find out what the report message is... if not, drop out risk are high....
 
 * avoid putting [too many numbers](https://www.unhcr.org/innovation/wp-content/uploads/2018/02/InnovationYearInReview2017_web.pdf#page=21) 
 
 * implement [story telling techniques](https://www.unhcr.org/innovation/wp-content/uploads/2019/04/Innovation18-19-WebApril2019.pdf#pag=23) - A good data story is a way to communicate valuable insights and assign meaning and context to data that otherwise lives as numbers in an Excel spreadsheet. The narrative shall have a hook, momentum, or a captivating purpose. Finding such narrative structure is therefore a prerequisite. Such stories can be categorized according to the four main narrative frames below, each of them being linked to programs design or implementation. The presented data shall reflect the operation context to reinforce what readers knows or to reveal what they don’t:
    1.	shed light on a previously unexplored topic (it teaches people something new or they have not heard before), 
    2.	introduce an interesting angle (gives them a new perspective) 
    3.	provide useful suggestions to solve a problem (inspires to act) 
    4.	disprove a hypothesis / debunk a widely held belief in terms of programmatic assumption.
    
### Shape the size of the content
The [ideal length of an article](https://torquemag.io/2018/04/optimal-content-length/) should be between 1500 and 2500 characters, taking an average 7 minutes to read. 

### Easy "active reading"
"Active reading" techniques consist in , __before reading the article content__, looking at any titles, subheadings, charts, graphs, and captions to get the key messages. - This allow to get the main content of the report simply by reading the table of content... it is used in most medias nowadays

To do that content needs to be hierarchized:

  *  Title should be turned into meaningful statement/ summary - rather than referencing the topic explained in the chapter text 
  
  * On the top of article text, add side note to highlight some key elements
  
  * include infographics / visual summary elements

### Make the site ready for social media sharing

Prepare Key message s (less than 144 character) ready to be tweeted and add a "share" button close to the specific quote .  

### organise site headers and footers

`_site.yml` is the file where site navigation bar is being configured, while `_footer.html` is used for the footer.

See also customization advice from https://rstudio4edu.github.io/rstudio4edu-book/rmd-dress.html 