+++
# Project title.
title = "Interactive Dot Density Maps with Shiny and Mapdeck"

# Date this page was created.
date = 2019-02-25T00:00:00

# Project summary to display on homepage.
summary = "Explore electricity and latrine access data from the Indian Census"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["sf", "mapdeck", "shiny", "ggplot2"]

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
url_code = ""
url_custom = [{name = "App", url = "https://shiny.seanangio.com/dots/"},
              {name = "GitHub", url = "https://github.com/seanangio/in_household"}]


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
  focal_point = "Smart"
  
  # Show image only in page previews?
  preview_only = true
+++

The app linked below is an interactive dot density map of 1991-2011 Indian Census data of Household Access to Electricity and Latrines. It is a companion project to an earlier effort to visualize the same data in a choropleth to demonstrate the tradeoffs between the two types of visualization.

**https://seanangio.shinyapps.io/dots/**

It is a companion project to an earlier effort to visualize the same data in a [choropleth](https://shiny.socialcops.com/gisvector/) to demonstrate the tradeoffs between the two types of visualization.

![](dots.gif)
