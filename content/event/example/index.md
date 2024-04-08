---
title: Bridging Data Gaps for Air Quality Monitoring - Daily PM2.5 Estimates for 10 km Grid Cells in India

event: EGU General Assembly 2024
event_url: https://meetingorganizer.copernicus.org/EGU24/EGU24-14441.html

location: Vienna, Austria & Online
address:
  street: Austria Center Vienna (ACV) Bruno-Kreisky-Platz 1
  city: Wien
  region: ''
  postcode: '1220'
  country: Austria

summary: A conference talk on the recent publication.
abstract: "India has experienced elevated levels of Particulate Matter (PM) 2.5 concentrations. Despite increased efforts by the Indian government,  the current monitoring network remains limited, impeding a comprehensive understanding of PM2.5 variations throughout the country. Limited PM2.5 data has led previous health studies to rely on publicly-available monthly PM2.5 estimates. However, these estimates have large uncertainties over the under-monitored regions, including India because PM2.5 observations have been calibrated into their model. The coarse temporal resolution of existing datasets makes it challenging to assess short-term effects of exposure to PM2.5. To bridge these gaps, it is imperative to develop daily PM2.5 datasets with robust spatial and temporal certainty.

This study develops open-source daily PM2.5 datasets at a 10 km resolution for India spanning almost two decades (2005 - 2023). Leveraging two-stage machine learning model with 10-fold spatial cross-validation (CV), we generate PM2.5 estimates for regions without ground measurements. In contrast to random k-fold CV, widely used in previous studies, spatial CV is implemented in this study to control for spatial auto-correction, which could lead to overfitting to the training data and underestimation of spatial prediction errors. The first stage fills missing observations for daily MODIS AOD, Sentinel-5P mission's TROPOPOMI NO2, and TROPOMI CO. The second stage predicts daily ground-measured PM2.5 concentrations. Two models are constructed for the second stage: the AOD model and the Full model, the latter incorporating TROPOMI features in addition to AOD.

The Full model exhibits a spatial out-of-sample performance with an R2 of 0.68, effectively predicting local and temporal PM2.5 variations rather than just average differences between locations, months, or years (within R2 = 0.49). The AOD model performs similarly, with an R2 of 0.64 and within R2 of 0.45. At the monthly level, our model outperforms the existing monthly PM2.5 dataset, with an R2 of 0.74 and within R2 of 0.52. 

Utilizing our PM2.5 predictions, we identified that 31% of 10 km grid cells across the country demonstrated a more than 5% reduction in PM2.5 concentrations in 2018-2022 compared to 2005–2010, and any decrease in PM2.5 was observed in 75% of the locations. Additionally, population-weighted annual average PM2.5 concentrations indicate a decline since 2018, except for a notable increase in 2021. Despite an overall declining trend since 2018, approximately 60% of the population remains exposed to PM2.5 concentrations above the national annual guideline (40 µg/m3), with 10% facing extreme levels of 80 µg/m3 annually.

Our method is useful for resource-constrained countries to understand nationwide air quality trends and identify areas with elevated pollution. To address this, we established the optimal number of air quality monitors using multiple machine learning models with randomly-sampled incremental training data. Our findings show a polynomial increase in within R2 for test data, ranging from 0.24 at 25 monitors to 0.54 at 300 monitors in the training data.

Our predictions offer valuable insights into air quality trends in India from 2005 to 2023. Importantly, our estimates contribute to understanding the number of ground monitors needed to explain variations in PM2.5 concentrations across the country, offering insights for other countries."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2024-04-15T03:20:00Z'
#date_end: '2024-04-01T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2017-01-01T00:00:00Z'

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: false

image:
  caption: ''
  focal_point: Right

links:
  #- icon: twitter
  #  icon_pack: fab
  #  name: Follow
  #  url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
  - example
---

{{% callout note %}}
Click on the **Slides** button above to view the built-in slides feature.
{{% /callout %}}

Slides can be added in a few ways:

- **Create** slides using Hugo Blox Builder's [_Slides_](https://docs.hugoblox.com/reference/content-types/) feature and link using `slides` parameter in the front matter of the talk file
- **Upload** an existing slide deck to `static/` and link using `url_slides` parameter in the front matter of the talk file
- **Embed** your slides (e.g. Google Slides) or presentation video on this page using [shortcodes](https://docs.hugoblox.com/reference/markdown/).

Further event details, including [page elements](https://docs.hugoblox.com/reference/markdown/) such as image galleries, can be added to the body of this page.
