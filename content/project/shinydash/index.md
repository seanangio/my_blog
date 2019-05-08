+++
# Project title.
title = "Dashboards with shinydashboard & ggiraph"

# Date this page was created.
date = 2019-05-09T00:00:00

# Project summary to display on homepage.
summary = "Explore how access to electricity in India varies with respect to latrine access at state and district levels through a scatterplot, dumbbell plot and a bivariate bubble map"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["shiny", "shinydashboard", "sf", "ggiraph"]

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
url_custom = [{name = "App", url = "https://seanangio.shinyapps.io/shinydash/"},
              {name = "GitHub", url = "https://github.com/seanangio/in_household/tree/master/shinydash"}]


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

The app linked below uses the {shinydashboard} and {ggiraph} packages to create an interactive visualization of Indian electricity and latrine access data. 

**https://seanangio.shinyapps.io/shinydash/**

While two previous iterations using this dataset focused on various geospatial representations, this project seeks to shed light on the question of how access to electricity and latrines vary with respect to each other. To what extent do high performers in electricity access also score well in latrine access? How do these metrics vary over time? Across different societal groups? Among urban vs. rural households? At state and district levels? In particular geographic regions?

The vastly uneven population counts across states and districts led me to choose visualizations that allow a raw count like population to be mapped to a size aesthetic, specifically a scatterplot, a dumbbell plot, and a bivariate choropleth. Of course, each has their own particular strengths and weaknesses.

#### District-level scatterplot across time

The scatterplot below is an example of how districts in India have improved their access to electricity and latrines over three decades, but have done so at significantly different rates. It is also interesting to examine the distribution of points. Generally, electricity rates are greater than latrine rates, but this is not exclusively the case.

![](scatter.gif)

Moreover, the dotted lines showing the All-India averages for the selected data divides the plane into four quadrants, identifying states or districts above or below the country average. We might expect to see the top right and bottom left quadrants: places that either do well or do poorly in both electricity and latrine access. The bottom right quadrant is also fairly easy to understand because electricity access tends to exceed latrine access, as demonstrated most vividly by the dumbbell plot. The top left quadrant however, those cases with above average access to latrines but below average access to electricity, are particularly interesting. I do not have any strong intuition for what is happening in this quadrant.

#### Dumbbell plots

The state dumbbell plot below is well suited to showing the gap between a state's household rate of access to electricity versus its rate of access to latrines. Dotted lines highlight cases where this relationship is reversed, and the rate of latrine access actually exceeds that of electricity.

![](dumbbell_state.png)

This plot above is busy, but readable at the state level. However, we can dive deeper into any particular state using the geographic filter. The plot below shows the same data for districts in the state of West Bengal.

![](dumbbell_district.png)

#### Bivariate Bubble Map

Previous iterations of this project have used choropleths to map the household rate of access to electricity or latrines. However, depending on the underlying data, we would be unable to map both of these metrics simultaneously. 

A bivariate color scheme, however, does enable us to track two variables at the same time. Although we have much less precision in any one category, we can place states or districts into a two-dimensional color bin instead of a typical one-dimensional scale.

![](bubble.png)

At the district level, bubbles can become quite crowded, but if we filter to a particular state or region, we can observe the data more clearly, as done here for districts in the Northeast states.

![](bubble_ne.png)