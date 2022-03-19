# Welcome to my index file!

<p>Actually I don't know what do I need to do here, ermmmm, right back...
</p>
<br>

(seconds)

<p>OK, Here my index.md file needs contain information about the meme I created,
for example, what the motivation was, and how my meme is new/original (e.g. an 
adaption of an existing meme format)</p>

Let's do it!

Dang---Dang----Dang

![my_great_meme lost@ @](huh.png)

**There are two reasons why I create this meme:**

1. I need to complete the assignment
2. I really don't want bad teammates in game
3. (🥦 really tastes bad)
 
<br>
<br>
 
Owner inspired by meme below (stored in repo)

![the source](mqdefault.jpg)

Want to know how to create amazing meme? See this👇

```r
install.packages("magick")
library(magick)
#Import images from web
ideal_team <- image_read("https://static0.cbrimages.com/wordpress/wp-content/uploads/2021/11/Avengers-Age-of-Ultron-Group-Shot.jpg") %>%
  image_scale(500)
#my team pic
your_team <- image_read("http://5b0988e595225.cdn.sohucs.com/images/20190729/4d67b2a19de44fb78f628bc8b157b935.jpeg") %>%
  image_scale(500)

#my team appendent
god_team <- image_blank(width = 500, 
                          height=250, 
                          color = "#000000") %>%
  image_annotate(text = "Team\nYou expected",
                 color = "#FFFFFF",
                 size = 65,
                 font = "Impact",
                 gravity = "center")%?%

# actual team
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
#combine whole works to a meme

(final_one = c(first_row, second_row) %>%
  image_append(stack = TRUE))

#create my pics
(image_write(your_team, "your_team.png"))
(image_write(ideal_team, "ideal_team.png"))
(image_write(c(first_row, second_row) %>%
               image_append(stack = TRUE), "huh.png"))


```

My work is done! **Cheers!**

![Bibi--](https://media0.giphy.com/media/RJEBGVo2mrGxsujtAE/giphy.gif)
