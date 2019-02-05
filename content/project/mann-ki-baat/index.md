+++
# Project title.
title = "Text Mining: TF-IDF & Sentiment Analysis"

# Date this page was created.
date = 2018-06-07T00:00:00

# Project summary to display on homepage.
summary = "Tidy text analysis of India PM’s radio addresses in a Shiny app"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["tidytext", "shiny", "ggplot2", "rvest"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references 
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides = "example-slides"

# Links (optional).
url_pdf = ""
url_slides = ""
url_video = ""
url_code = ""

url_custom = [{name = "App", url = "https://github.com/seanangio/mkb"},
              {name = "Blog", url = "https://blog.socialcops.com/technology/data-science/introduction-tidytext-mining/"},
              {name = "GitHub", url = "https://github.com/seanangio/mkb"}]


# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
#url_custom = [{icon_pack = "fab", icon="twitter", name="Follow", url = "https://twitter.com/georgecushen"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  #caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Center"
  
  # Show image only in page previews?
  preview_only = true
+++

Every month the Indian Prime Minister Narendra Modi gives a radio address to listeners. I collected those speeches with `rvest` and created a `shiny` app to allow users to explore different aspects of the corpus, such as word frequencies, sentiment, and TF-IDF. Find the app at the button above or link below:

**https://seanangio.shinyapps.io/mann_ki_baat/**

![](mkb.gif)

Related to this project, I also wrote a short post introducing the `tidytext` package found on the [Social Cops blog](https://blog.socialcops.com/technology/data-science/introduction-tidytext-mining/).
