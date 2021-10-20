## UT Journalism Professor Bio Scraper

Data Scraper: José Martínez, martinez307jose@gmail.com

This project searches through every UT journalism's professor's bio page and looks for a specific keyword.

For example, if one wants to know if a certain professor of ours has worked at ‘CNN’ or has done ‘audio’ work, one would input the keyword and it would return what professors have that in their bio. 

At the beginning, I wanted to know if there were any professors in my journalism school that had done investigative work in their careers.

The following page, https://journalism.utexas.edu/faculty, displays every professor from the journalism school at UT but with only their name, position, and image. To see more info about their careers, you'd have to click on the image and go to an entirely different page.

To find a professor who had done investigative work, it seemed too complicated to click through every page, so I decided to create this scraper.

Important to note, the page does have a search bar that does the exact function I want it to do, but I wanted to try it on my own for fun.

In essence, I used Selenium to first pull the links from all the pages. I noticed that every page with a professor's bio had "faculty/" in their url, so I filtered for that. Then, I just pulled the page source of each page. Searching for a string in the page source would be similar to searching for a keyword in each page. Thus, the final cell iterates through every link with your keyword and returns the last name of the professors that have that keyword.
