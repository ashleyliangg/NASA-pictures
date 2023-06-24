# NASA Picture of the Day Project
### Author: Ashley Liang

## Overview
This NASA APOD (a picture of the day) project allows the user to pick any day between the day that the picture of the day launched (June 16th 1995) and today, and displays the information and media related to that day's picture or video. This project combined two APIs: the NASA picture of the day and flatpickr, a datetime calendar picker. The top portion of the index.html file is the HTML, the bottom portion is the Javascript. 

![screencapture-file-Users-ashleyliang-Documents-Coding-projects-NASA-pictures-index-html-2023-06-23-22_05_38](https://github.com/ashleyliangg/NASA-pictures/assets/102703391/b2f3cb36-e1c1-4471-bf76-643378d771dc)


## How to run locally
Since it is just an HTML file, just open it with Google Chrome. If it is on Visual Studio Code, click run without debugging.

## Features
- Select any date from the first picture of the day (June 16th 1995) up to today to get the picture or video of the day
- Page includes the name of the picture/video, copyright, description, and the picture/video
- If the user clicks on the image (action indicated by the slight shading of the picture when the user's mouse hovers over the image), the user gets redirected to a new tab with a higher resolution image. This ONLY works with images, as the videos are just in YouTube video format.

## My experience
This project was challenging for me in a couple ways. One was that I've never used bootstrap or implemented a Javascript section in an HTML file before, so it took me a while to understand the structure, syntax, and what the classes were referring to (the bootstrap css). Initially, I followed this youtube video: https://www.youtube.com/watch?v=Y1n2a7YxYGY. However, the date picking part of the video was through a bootstrap premium account, which you had to pay for. I wanted to add the date picker option because I thought that feature was really cool and unique compared to the other NASA APOD videos I looked over, so I found my own way to implement a date picker. I googled different free date pickers and settled on flatpickr because it seemed pretty straightforward based on the documentation overview. However, I kept running into this issue where the flatpickr API wasn't showing up in the form and input HTML tags; it was just the basic HTML form without the calendar pop-up. After searching up the error and spending time trying out different ways to initialize the calendar, it worked. Then, I ran into an issue where I couldn't figure out how to grab the date that the user selected. I searched up the issue but all the answers and tutorials used jquery, which I wasn't using in this project. I then found this onChange hook that would change the date to whatever the user picks, but I couldn't find straightforward documentation on how to use this method in the code. After a couple days of searching, I finally found the syntax that was quite similar to how I ended up using  onChange, and it finally worked (since it wouldn't work on the actual page, I was printing the date to the console). Once I was able to get date variable, I was able to add the calendar aspect to my existing program. After rearranging the code structure to get the calendar/date to work within the program, the program worked! Overall, I was quite proud of myself that I was able to persevere with the calendar and date picking feature. I'm also proud that I was able to solve issues on my own by thinking and playing around with my code instead of just following tutorial/debugging videos.

Updates: I changed the look to fit more of a outer space aesthetic by turning the background black and changing up the fonts. I also experimented a bit with css animations, but I'm not too sue if I like the look of it on this particular project.


MDB5
Version: FREE 4.4.0

Documentation:
https://mdbootstrap.com/docs/standard/
