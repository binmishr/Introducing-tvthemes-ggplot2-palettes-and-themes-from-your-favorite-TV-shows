# Introducing-tvthemes-ggplot2-palettes-and-themes-from-your-favorite-TV-shows

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same.



The `tvthemes` package is a collection of various `ggplot2` themes and
color/fill palettes based on everybody’s favorite TV shows.  I got a lot of good feedback on the colors I used for the
custom `ggplot2` theme and color palettes so I decided to expand it to
other shows that I love\! Suggestions and Pull Requests for
palettes/themes are welcome\!

 
``` r
library(tvthemes)
library(ggplot2)
library(extrafont)
#> Registering fonts with R
loadfonts(quiet = TRUE)

ggplot(mpg, aes(displ)) +
  geom_histogram(aes(fill = class), 
                 col = "black", size = 0.1,
                 binwidth = 0.1) +
  scale_fill_brooklyn99(palette = "Dark") +
  labs(title = "Do you know what it means to 'clap back', Raymond?",
       subtitle = glue::glue("BE- {emo::ji('clap')} -CAUSE {emo::ji('clap')} I {emo::ji('clap')} DO {emo::ji('clap')} !"),
       x = "Titles of Your Sex Tape",
       caption = "Pizza bagels? Pizza rolls? Pizza poppers? Pizzaritos? Pizza pockets?") +
  theme_brooklyn99(title.font = "Titillium Web",
                   text.font = "Calibri Light",
                   subtitle.size = 14)
```

## Current list of TV shows

  - **Avatar: The Last Airbender**: theme + palettes (Fire Nation, Water
    Tribe, Earth Kingdom, & Air Nomads)
  - **Brooklyn Nine-Nine**: theme + palettes (regular & dark)
  - **Game of Thrones/A Song of Ice & Fire**: ‘The Palettes of Ice &
    Fire’ (currently: Stark, Baratheon (Stannis), Lannister, Tully,
    Targaryen, Martell, Greyjoy, Tyrell, Arryn, Manderly)
  - **Rick & Morty**: theme + palette
  - **Parks & Recreation**: two themes (light & dark) + palette
  - **The Simpsons**: theme + palette
  - **Spongebob Squarepants**: theme + palette + background images
  - **Hilda**: Day, Dusk, Night themes + palettes
  - **Attack on Titan**: palette
  - **Kim Possible**: palette
  - **Big Hero 6**: palette
  - **Gravity Falls**: palette
  - *More in future releases…*
  - *Development branch*: TBD…

## Installation

You can install `tvthemes` by:

``` r
## v1.1.0 is available on CRAN!
install.packages("tvthemes")
```

## tvthemes 1.0.0 Major Changes

## Brooklyn Nine-Nine

![b99d](https://i.imgur.com/SjxWFXd.png)

![b99l](https://i.imgur.com/OHWQn2q.png)

## Spongebob Squarepants

![bobspog](https://i.imgur.com/cVHEADt.png)

![bobspogbkg](https://i.imgur.com/kpwgeRA.png)

## Game of Thrones: House Stark, Tully, Targaryen

![StarkTullyTargaryen](https://i.imgur.com/TRYevg9.png)

## Game of Thrones: House Tyrell, Lannister, Greyjoy

![TyrellLannisterGreyjoy](https://i.imgur.com/NUjriiF.png)

## Game of Thrones: Arryn, Manderly, Martell

![ArrynManderlyMartell](https://i.imgur.com/WfieMDW.png)

## Game of Thrones: Stannis Baratheon, The One True King

![stannis](https://i.imgur.com/GuCuzyr.png)

## The Simpsons

![simpsons](https://i.imgur.com/DFHVlJS.png)

## Rick and Morty

![randm](https://i.imgur.com/YB7xSoe.png)

## Avatar: The Last Airbender (Fire Nation, Air Nomads, Water Tribe, Earth Kingdom)

![tla](https://i.imgur.com/JA4hEbJ.png)

## Parks and Recreation

![pandr](https://i.imgur.com/9641myM.png)

## Attack on Titan

![aot](https://i.imgur.com/BsLsWPX.png)

## Kim Possible

![KimPossible](https://i.imgur.com/2p9Jf8o.png)

## Big Hero 6

![bighero6](https://i.imgur.com/ww197w4.png)

## Hilda

![hilda](https://i.imgur.com/J9uv7hV.png)

## Gravity Falls

![gravityfall](https://i.imgur.com/Gl83AXz.png)

