

## Down upper?
**"Down Under"** is a song recorded by Australian rock band Men at Work. 
<br>It was *originally released in 1980*.
1. A new version of the song was produced by Colin Hay in 2021.
2. The song has been on the NZ Top 40 singles chart for 16 weeks.

![](down_under.jpg)







# **stats220** (Assignment purpose!)

## Author: Yanjie Zhou

### Purpose
<!--- numbered list--->
1. The purpose of this website is to show people how to create meme using **R**. 
2. Have a happy life.
3. Sleep well.

### !Notice
* Don't delete any code from this repo
* *No more* ๐ฅฆ.
* I really love cheese burger

<br>
<br>

[This is the link to my repo](https://jizzx6.github.io/stats220/)

<br>

### I gonna show you something!

Want learn some **magic**? Come and visit ๐ [{magick}](https://cran.r-project.org/web/packages/magick/vignettes/intro.html)

[And this is the assignment page.](https://canvas.auckland.ac.nz/courses/75888/assignments/272595) You got to try once this beautiful thing.

<br>

Ermmm, I don't know what else I can put...
 A bit spoil of my r work but I guess this is alright. Dang-dang-dang-----![ui](huh.png)

<br>
At the end, wish you all the best with my cuteness teammates!  ๐ป
 
 ![ababaab](your_team.png) ![gif](https://media0.giphy.com/media/RJEBGVo2mrGxsujtAE/giphy.gif)

<br>

Below is my code fence๐
```r
library(magick)

ideal_team <- image_read("https://static0.cbrimages.com/wordpress/wp-content/uploads/2021/11/Avengers-Age-of-Ultron-Group-Shot.jpg") %>%
  image_scale(500)

your_team <- image_read("http://5b0988e595225.cdn.sohucs.com/images/20190729/4d67b2a19de44fb78f628bc8b157b935.jpeg") %>%
  image_scale(500)


god_team <- image_blank(width = 500, 
                          height=250, 
                          color = "#000000") %>%
  image_annotate(text = "Team\nYou expected",
                 color = "#FFFFFF",
                 size = 65,
                 font = "Impact",
                 gravity = "center")


bad_team <- image_blank(width = 500, 
                         height = 400, 
                         color = "#000000") %>%
  image_annotate(text = "Team\nYou Got",
                 color = "#FFFFFF",
                 size = 65,
                 font = "Impact",
                 gravity = "center")

first_row <- c(ideal_team, god_team) %>%
  image_append()

second_row <- c(your_team, bad_team) %>%
  image_append()


(final_one = c(first_row, second_row) %>%
  image_append(stack = TRUE))

#create my pics
(image_write(your_team, "your_team.png"))
(image_write(ideal_team, "ideal_team.png"))
(image_write(c(first_row, second_row) %>%
               image_append(stack = TRUE), "huh.png"))



```
```{css}
h1 {
  color: #ffffff; 
  background-color: #ff5470; 
  padding: 10px
}
```
