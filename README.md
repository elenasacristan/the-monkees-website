# The Monkees website – First milestone project

This is a website that will be used mainly by current and prospective fans of the Monkees  in order to keep up to date with the latest news, know more about the band and listen to the Monkees songs.
It will also be used by the band to sell tickets for future concerts, showcase the new albums and be contacted by event organisers to play in events.

Click [here](https://elenasacristan.github.io/the-monkees-website/) to see the website.

## UX

This website is targeting current and potential fans of the Monkees band. This website is also used to showcase their music so event organisers can book the band to perform in events.

### mockups:

In the links below you can see the mockups that I drew using the mockup tool “Pencil”:

- [index.html](https://github.com/elenasacristan/the-monkees-website/tree/master/mockups/index.png)
- [the band-part1.html](https://github.com/elenasacristan/the-monkees-website/tree/master/mockups/ttheband1.png)
- [the band-part2.html](https://github.com/elenasacristan/the-monkees-website/tree/master/mockups/tthebandp2.png)
- [the band-part3.html](https://github.com/elenasacristan/the-monkees-website/tree/master/mockups/thebandp3.png)
- [news.html](https://github.com/elenasacristan/the-monkees-website/tree/master/mockups/news.png)
- [listen.html](https://github.com/elenasacristan/the-monkees-website/tree/master/mockups/listen.png)
- [contact.html](https://github.com/elenasacristan/the-monkees-website/tree/master/mockups/contact.png)

**Note that the final design has changed from the original design in the mockups. The reason why it has changed is because I was trying different layouts while I was writting the code and sometimes the new designs looked better than the original ones. I also was advised by my mentor to remove the two scrolling bars in the page listen.html and display each section in a different bootstrap raw. Another addition were the quotes in the contact.html page*

### User stories:

- As an event organiser I want to know more about the band, its members and the musical career of the band members, so I can decide if they are an appropriate band for the event that I’m organising.
- As a potential fan I want to know more about the band, the members and their musical career, so I can expand my knowledge about the Monkees.
- As a current / potential fan or event organiser I want to follow the band on social media, so that I can be up to date with their latest posts / news.
- As a current / potential fan I want to know if there is going to be new material released and when, so I can listen to it as soon as it is available.
- As a current / potential fan I want to know when the next concerts are due to take place, so I can decide if I can go or not.
- As a current / potential fan I want to buy tickets online for the concerts.
- As a current / potential fan I want to listen to old and new songs, so that I can be entertained.
- As a current / potential fan I want to download the song lyrics, so I can learn and sing the songs.
- As an event organiser I want to know about the opinions from other people who booked the band before, so I can decide if I want the band to perform at my event or not.
- As an event organiser I want to contact the band to see if they can play at my event.
- As a member of the band I want to know the type of events, number of people, days, times and places where the event organisers would like to book the band.
- As a current / potential fan I want to subscribe to the website so I can receive notifications for future concerts, new material and offers.

## Features

### In all pages

- **GoogleFonts:** They are used to customise the website and create a style that matches with the Monkees branding. I have used Bangers and Cuprum and I have added the following code in the Style.css file.

  `@import url('https://fonts.googleapis.com/css?family=Bangers|Cuprum:400,700');`

### index.html

- **Carousel:** Allows users to see some of the best pictures of the Monkees rotating automatically. They can click on the arrows to go to the next or previous picture faster but if they don’t click  on the arrows the pictures will rotate automatically.
The carousel feature has been taken from bootstrap and then the css has been modified to suit the needs of the website.

- **Redirects:** By clicking on the Logo or by clicking on the word “Enter” the users get redirected to the page “theband.html”.

### theband.html, news.html, listen.html and contact.html
#### Navigation-bar
It will allow users to navigate to other pages of the website by clicking on the navigation items. I’ve used the navigation element from bootstrap, removed the navigation items that I didn’t need and updated the style with CSS.

  The navigation bar will be the same for the four pages with the link to the current page highlighted in dark blue.

- **Logo:** The logo in the navigation-bar will redirect the users to the page “index.html”.

- **Hamburger button:** The navigation bar will collapse for small screens. I have used the Hamburger button from Bootstrap and customised it with CSS.

- **Modal:** in the navigation-bar we have the “Subscribe” button that will open a modal window to enter contact details and subscribe to the newsletter. The modal feature has also been taken from bootstrap and the CSS styles have been updated.

- **Form:** Inside the Modal window I have added a Form (also taken from Bootstrap). 
I have removed the fields that were not needed and I have updated the CSS. I have also added the attribute “required” to make the fields compulsory and to avoid wrong emails being entered.

#### Footer
In the footer the user can see the contact details email and phone number (I used dummy contact details) and also the social media links - in case the user wants to follow the band on social media.
The footer is the same for the four pages in order to keep the website consistent.
The navigation bar and footer are always visible and the content is scrollable.

- **Social-Links:**  Allows users to follow the band on social media (Facebook, YouTube, Twitter) by clicking on the icons at the bottom of the page.

- **FontAwesome:** The FontAwesome icons are used to add extra meaning in several pages (i.e. social media buttons, share button in listen.html).

### theband.html
The users get redirected to this page from index.html.
This page is split in three main areas “History of the band”, “Members” and “Discography” and is aimed for users who don't know much about the band or for those who want to learn more about them.

- **History of the band:** The content is taken from Spotify and the users can continue reading on Spotify by clicking on “Read more”.

- **Members:** In this section you can learn about the members. The content is taken from Wikipedia and you can also read more by clicking on the links “Read more”.

- **Discography:** Contains all the albums released from the beginning until the present day. The information comes from Wikipedia.

### news.html
The news.html page has two sections. The first one is “Concerts coming up...” and the second “The latest”
#### Concerts coming up...
This section will display a list of the next 7 concerts, information about the amount of tickets available and it will allow the users to buy tickets online.

- **Progress bars:** I have used progress bars from bootstrap in order to show the tickets available for future contents.

- **Label:** I have used labels to add emphasis to the amount of tickets left. When there are less than 15% of tickets available the label will say “Hurry up!!” and it will blink (the blink effect has been done using @keyframes), if the tickets are sold out the label will be red and will say “Sold out”, if there are still plenty of tickets left then the label won't be displayed, and if the tickets are not available yet the label will be blue and will say “Tickets available soon”.

- **Keyframes:** The blinking effect for the yellow labels has been made using keyframes

- **Book Now buttons:** A modal containing a form will open when the user clicks on “Book Now”. In this modal the users will type their name and email in order to book the tickets.  Both fields are compulsory and the email needs to be a valid email address. Then the user should receive an email with the next steps to buy the tickets online (this part is not done yet because I still need to learn how to do it).

#### The latest
In this section the users can see videos of the latest performances by the Monkees.

- **Iframe:** I have used iframes to add videos from YouTube. In order make the video responsive to the size of the screen I’ve followed the instructions in the link below:
	
  https://www.youtube.com/watch?v=X4t0JxiBeO0

### listen.html
I have split this version in two sections. The first section is “What's New!” and the second is “The Classics!”.
#### What's New!:
This section contains the play lists for the most recent albums by the Monkees.

- **iframe:** I have embedded two albums from the Monkees from Spotify by copying the embedded code from the Spotify website. Then I have added a frame around it with CSS.

  The users that are already members of Spotify will be able to listen to the full album and the users that are not Spotify members will be able to listen to a fraction of the songs.
I have also added a follow us link (embedded code taken from Spotify) so the fans can follow the Monkeys on Spotify.
#### The Classics

In this section the users can play some of the more famous songs from the Monkees.

- **Audio:** I have added the element audio with the controls so the users can play and pause the songs.

- **Keyframes:** In order to improve the user experience I have added a rotation effect on the vinyl images. I have downloaded a vinyl image from Google and I have placed on top a picture from the Monkees (with a circular shape). If the user hovers over the image on the vinyl the circular image on top of the vinyl will rotate.

- **Download lyrics:** The users can download the lyrics in “.txt” format so they can learn and sing the songs. The lyrics have been copied from Google.

- **Share button:** (this will be a future addition when I learn how to do it). This button will allow the users to share the classics with family and friends.

### contact.html
This page is aimed for event organisers who want to contact the band to play in an event.

- **Form:** This page will have a contact form where the event organisers need to enter their contact details, details about the type of event, day, time, number of assistants and additional comments (optional).

- **Quotes:** The users who are planning an event can read the opinions from other people who have booked the Monkees in the past.

## Features Left to Implement

- **Online payments:** At the moment the users need to enter their contact details and then they should receive an email in order to complete the payment online, but it will be easier for the users if they could complete the online payment while they are on the website.

- **Share button:** Once I learn how to do it I would like to allow users to share the songs on their social media websites when they click on the icon “Share” (listen.html)

- **Pop-up window after the forms are filled out and submitted:** I would like to display a message saying “You are subscribed now!” when the users fill in the form and click on Subscribe. I would also like to display a message for the other two forms in the website (in the contat.html and in the news.html pages). I could have added the Modals with the messages but I still need to learn how to check if the fields have been filled before displaying the message.

- **Rotation when play is pressed:** Once I learn JavaScript I would like to rotate the vinyls when the play icon is pressed and stop them when paused is pressed (right now they only rotate if you hover over the small image).

- **Audio:** When the play control in the audio element is pressed it makes sure previous audio elements stop playing and the same for the iframes from Spotify and YouTube.

- **Start rating:** I would like to add a 'Start rating' scale under the audio elements so when the users listen to the songs they can give them a rating.

## Technologies Used

#### Languages:

- **HTML5:** Is the main language used to create the structure of the website.

- **CSS3:** Is the language used to add styles to the HTML.

#### Development environment:

- **[Cloud9:](https://c9.io/ 'https://c9.io/')**
I have used the cloud9 development environment to write the code. In cloud9 I have been able to see the changes in real time as I type the code. I have also used the terminal from cloud9 in order to use Git, create my local repository and then push the repository to the GitHub (remote repository).

#### Version control system:

- **[Git:](https://git-scm.com/ 'https://git-scm.com/')**
I have used the version control system Git from the cloud9 terminal in order to track changes in the website and push them to GitHub.

#### Hosting service:


- **[GitHub:](https://github.com/ 'https://github.com/')**
I have used GitHub Pages in order to deploy the website and it is also the remote repository where I have pushed the changes from cloud9.

#### Frameworks:

- **[Bootstrap:](https://getbootstrap.com/docs/3.3/,'https://getbootstrap.com/docs/3.3/')**

  The style sheet from Bootstrap is placed inside HTML <head> but before my own style sheet so I can overwrite the styles with my own CSS code: 
  
  `https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css`

  I have used bootstrap in order to be able to use the grid system to structure the content in an organised and responsive way and also in order to use some of the components (i.e. arousel, navigation bar, progress bars, form, modal and typography).

#### Libraries:

  The style sheet from FontAwesome is placed inside HTML but before my own stylesheet so I can overwrite the styles with my own CSS code:

- **[FontAwesome:](https://fontawesome.com/ 'https://fontawesome.com/')**

   `https://maxcdn.bootstrapcdn.com/font-awesome/4.6.3/css/font-awesome.min.css" `

  I have used it to add icons in several places in the website to improve the user experience and to add social media links.

- **[Google Fonts:](https://fonts.google.com/ 'https://fonts.google.com/')**
I’ve used the fonts from Google Fonts to style the fonts in the website.

- **JavaScript from Bootstrap and JQuery**

  `https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js`
  `https://code.jquery.com/jquery-3.3.1.min.js`

  I have used these two libraries because they are required for some of the bootstrap components (i.e. Modals, Carousel...). It is important to add them in the right order: first JavaScript from Bootstrap followed by jQuery. They need to be at the end of the code (just before the `</body>`  tag).

## Testing

### Validation

- **HTML:** I have used https://validator.w3.org/ in order to validate the HTML code.
- **CSS:** I have used https://jigsaw.w3.org/css-validator/ in order to validate the CSS code.


After running the validation I found several errors (i.e. typos, obsolete and wrong attributes, duplicated attributes, duplicated code...). I also found some warnings but most of them were actually correct code and they could be ignored.
### Features and responsiveness testing
  Once all the errors and some of the warnings were fixed I started testing the website page by page, checking every feature in all possible screen sizes.

  In order to make sure I checked all the features I created a spreadsheet with a check list to make sure everything got tested. This list contained all the features for each screen size so I could check the features and website responsiveness all at once.
  

  Click [here](https://github.com/elenasacristan/the-monkees-website/tree/master/Documents/Check-list.pdf) to see the check-list that I have used to test all the features in all the screen sizes.

### Additional testing
I have used development tools in Google Chrome to check how the website would look in different devices. In addition to that testing I have also asked friends and family to have a look at the website to let me know if everything looks fine on their browsers and devices.


### Problems and bugs:
- **Padding from Bootstrap elements:** One of the issues that took me longer to fix was the padding than one of the rows (from bootstrap) which was creating an overflow.

- **Form error message not being displayed:** I also had issues with the form inside the Modal that appears after clicking “Subscribe”. The problem was that the error message wasn't being displayed if the fields were left empty. Then I found out than when I was working on styling the original form I end up taking the button out of the "form" tags. Once I added the button again (inside the form tags) the form was working fine.

- **Elements alignment:** I struggled centering elements vertically and horizontally until I watched a tutorial about flex-box which helped me to understand better how to center elements.

  https://www.youtube.com/watch?v=JJSoEo8JSnc&t=372s

- **Custom attribute:** In theband.html the custom attribute “data-year” was initially called “year“ and it was giving me errors in the validator. I asked in slack and they told me that I should add “data-” before "year" in order to fix the issue.

## Deployment
I have used GitHub Pages to deploy the website. In order to do that I have followed the steps below:

1. I have created a repository in GitHub called: “elenasacristan/the-monkees-website”
https://github.com/elenasacristan/the-monkeys-website.git
2. I have initialised git from the terminal in Cloud9:
  
    `git init`

3. I have added the files that I was working on to the Staging area by using: 

    `git add .`

4. I have run the commit command with the first commit

    `git commit -m “initial commit`

5. I have copied from GitHub the following path and I have run it in the cloud9 terminal in order to indicate where is my remote repository:

    `git remote add origin https://github.com/elenasacristan/the-monkeys-website.git`

    `git push -u origin master`

6. Then from my GitHub repository I have gone to settings, I have selected the master branch, I have saved and the website was published at:

    https://elenasacristan.github.io/the-monkees-website/ 

7. After this was done I have ran regular commits after every important update to the code, and I pushed the changes to GitHub pages.

8. Also I have used “git clone" https://elenasacristan.github.io/the-monkees-website/” in order to download the website to my computer and to be able to work offline.


### My repository


https://github.com/elenasacristan/the-monkees-website/


## Credits


#### Content
- The content in “theband.html” section “history of the band” was copied from Spotify 
  
  https://open.spotify.com/artist/320EPCSEezHt1rtbfwH6Ck/about

- The content in “theband.html” section “members” and the dates for the albums in the section “discography” were copied from Wikipedia

  https://en.wikipedia.org/wiki/The_Monkees

#### Media

##### index.html 
- The photos used for the carousel were obtained from Google images using the Advance Search and selecting “free to use, share or modify, even commercially”. 
 
   https://commons.wikimedia.org/wiki/File:The_Monkees.jpg 
  https://cs.m.wikipedia.org/wiki/Soubor:The_Monkees_May_1967.jpg
  https://commons.wikimedia.org/wiki/File:The_Monkees_1967.jpg

##### theband.html:

- All the photos on theband.html page were obtained from the assets that were provided by codeinstitute for the project.

##### news.html:

- The videos in “The Latest” section were obtained from YouTube.

##### listen.html:
- The iframes with the recent albums from the Monkees were obtained from Spotify. 

  https://open.spotify.com/album/3WzJHiv489Wb9So4K7csLy
https://open.spotify.com/album/618fk3ITH2nXQtT0nTTZ84
- The vinyl image was obtained from Google images using the Advance Search and selecting “free to use, share or modify, even commercially”.

    https://pixabay.com/en/vinyl-platinum-disk-music-dj-2241789/
    
- The photos on top of the vinyl images were obtained from the assets that were available for the project.
- The mp3 files were also obtained from the assets that were available for the project.

##### contact.html
- The photos on this page were obtained from Google images using the Advance Search and selecting “free to use, share or modify, even commercially”.

  https://www.flickr.com/photos/ralphandjenny/7712255662

  https://www.nps.gov/orgs/1207/07-26-2016-birthday-month.htm

  https://www.pexels.com/photo/christmas-corporate-dinner-formal-576431/

## Acknowledgements
- I received inspiration for the rotating vinyl on the “listen.html” when I was looking for music themes and I saw a vinyl rotating when the play button was pressed (https://codepen.io/joshbader/pen/GqXbVk). 
Since I still haven't learnt about JavaScript I decided to do something similar using @keyframes instead.
- Thanks to the slack community for helping me solve some questions while I was working on the website.
- Thanks to my mentor (Guido Cecilio García Bernal) for his advice on the final touches to improve the website, for training me on Git and helping me better understand how to run the code locally.
 

