# Milestone Project One: Champion guide
In this project, I hope to display the skills I have learnt so far in coding appealing and eye-catching websites using HTML and CSS. 
League of Legends is one of the biggest MOBA (Multiplayer Online Battle Arena) games around with 151 unique champions to currently pick and choose from.
The purpose of my project is to give insight and indepth knowledge of one of those champions, Lucian. Lucian has one of the biggest skill gaps when comparing new 
and experienced players, the main goal of my website is to help bridge that gap.

Most League of Legends players choose to 'main' a role and a champ. This means they put most of their play-time into their specific position (Top, jungle, Mid, Bot and Support).
Players then also further specialise by putting most of their time into a few specific champions that do well in their preferred role. LoL sites usually focus most of their attention 
on the statistics of a champ and how their winrate is performing during the current patch (most patches last two weeks). By presenting the knowledge I have gained through play experience 
in a more graphical nature I can help players gain more knowledge on champs they may not be comfortable playing.

## UX
One thing all champions have in common is 3 basic abilites and 1 ultimate ability bound to 4 separate keys (usually QWER) that have varying cooldowns after use. This makes up a champions 
kit and gives a champion their identity.
Champs can also have multiple passive effects which can make learning a champion's combos and playstyle quite daunting. 

### User Stories
As a user, I would like to understand the optimal way of spending my champions skill points.
* I achieved this by creating a responsive bootstrap table highlighting the best order to spend Lucian's skill points. Inspired by ![Skill Point Tree](https://res.cloudinary.com/dksxe1yku/image/upload/v1605829495/lucian_leveling_mfdhdg.jpg) which can be found on [Lucian's u.gg page](https://u.gg/lol/champions/lucian/build)

As a user, I'd like to learn more about a champion that I'm unfamiliar with. 
* This was acheived through my collapse videos and embeds. These showcase all parts of a champions kit, allowing users to see a visual example of an ability/combo in-use.

As a user, I'd like to understand synergies/disadvantages my champ has in relation to other champions.
* This was acheived through the use of progress bars and bootstrap media objects, which relay this information in a visually appealing manner.

As a user, I'd like to know more about a champions itemisation.
 * This was acheived through the use of boostrap's grid sturcture and colour coded font awesome icons clearly displaying pros and cons of popular items on Lucian.

As a user, I'd like to know more about Lucians rune tree choice.
* This was acheived through a nested bootstrap image field, bringing attention to his first choice runes and text to provide context.

Main features to include are:
* A full page background showcasing Lucian's 'Splashart' (As league of legends has a very capable and talented artwork team)
* An interactive 3d image carousel used to navigate to different pages within my site (Bonus feature)
* Embed video from YouTube with controls added so video can be paused and started (The video will show gameplay of Lucian and using his abilities)

## Features
### Full Width Backgrounds
* League of Legends is a game with beautiful iamges, called splash arts, used to depict their champions in different settings/situations. I wanted
to use these images as full width backgrounds - as a way of showcasing them.

### Load In Animation
* Inspired from the courses Love Running project, there's a slight zoom effect as the page is loaded. This brings even more attention to the full width images.

### Gifs 
* All gifs are from either in game footage or game cinematics. this helps produce a positive response from users as they can see 
chaaracters they may know in action.

### Font Awesome Icons
* Font awesome icons help sections/words stand out or link to their content (coin icons referring to the ingame currency gold) which helps elicit a positive
emotional response from users.

### Interactive Cards
* 3 interactive cards, gold hover effect, with a teaser of the section they link to. Example, the card that describes lucian laning links to 3 of the top supports that he likes to lane with.

### Responsive table
* With 18 skill points available to be spent on a champions 4 abilities, a table was the best way to respresent this data. This allows a user to quickly see at glance where to spend 
their skill points.

### Collapse
* I made use of a few collapse elements, sourced from bootstrap, to help me display the abilities I described on my abilities page. 
By using a collapse instead of regular iFrames, it helps bring more interactivity into my site whilst also giving users an action to perform whilst using my site.

### Youtube Embed videos
* Embedding youtube videos of a champions abilities in action, allows the user to visually see the ability in action next to its explanation.

### Responsive images/videos
* All embeds have aspect ratios coded into their display, this was done to stop big black bars appearing when the video was forced to play in the wrong aspect ratio due to fixed heights and 
widths.

### Bootstrap Progress Bars 
* A visual representation of data rather than just the usual win-rate with/vs x champion. This will help users understand the why behind the data.

### Contact form 
* This section showcases use of the boolean atrribute required

## Features Left to Implement
Potential features to include:
* A forum style page where people can post comments about the state of the champ and his best item build path
* More pages on other Champs from League of Legends. Currently the two links in my dropdown (Samira and Xayah) circle back to my home page. In the full site, these would link to their own specific 
guides

## Technologies Used
* [HTML](https://www.w3.org/html/) (links to be added)
  * Used to create the basic structure of my page

* [Bootstrap](https://getbootstrap.com/)
  * Used to make styling my page easier
  * Bootstraps java library is also used for two elements, namely the nav collapse and for my tooltips

* [CSS](https://www.w3.org/Style/CSS/Overview.en.html)
  * Used to make my website unique

* [Cloudinary](https://cloudinary.com/)
  * Cloudinary was used as a CDN to help speed up the load times of my site as all my images are hosted there.

* [Giphy](https://giphy.com/)
  * Giphy was usesd to convert my raw mp4s into gifs. Reducing their file size and lowering the load time of my site. 

* [Nvidia Shadowplay](https://www.nvidia.com/en-gb/geforce/geforce-experience/shadowplay/)
 * Was used to record ingame footage from League of Legends.

* [Github Pages](https://pages.github.com/)
 * Github pages was used to host my live site.

* [Favicon io](https://favicon.io/)
 * Used to generate a favicon for my webpage

* [Font Awesome Icons](https://fontawesome.com/)
 * Font awesome and their free icons was used for all text icons found in my html.

## Testing
Firstly, after opening github I would open my project in a separate window using the command 'python3 -m http.server'. I would have my project open in another window and 
after altering my code I would save using ctrl + s. To view the result I would refresh product window using ctrl + shift and the refresh button, fully loading the site instead of loading from 
my locally cached version.

The Inspect tool was also critical in testing as I only had my iPhone as another viewing device so I could simulate other device sizes using a this.

I have tested my live site in chrome, firefox, Safari, Opera and Microsoft Edge. The feature I was most worried about not translating was the zoom effect when my page loads. 
From both my live site and my locally launched site, the feature was preserved.

Before my 2nd call with my mentor, he asked me to deploy my page to Github pages. After doing so, only my boostrap and font awesome links were affecting my page.
Almost all my images and my css were not rendering. It was pointed out that the file paths I was using, whilst relative and technically correct when run locally, were wrong when looked 
at from a live perspective. After some trail and error it was pointed out to me on slack that the paths had to be more precise. The following commits: 
* 1a215a0d5bf87e96804dcdca65629a91092657a0
* aebc534ddb729601a4473c8576e94ca1daa12407
* 7e1b6f82c1940e8fa3e57d745cc3c447e76f97ee
* 692c8ea358e70abefbbf79f7cede323b4688354f 
were my efforts in getting images to load when my page was loaded from the deployed version. After understanding this all images were subsequently added using properly coded file paths.
Once the project was mostly completed, my images were copied to cloudinary and all src attributes were changed to the corresponding cloudinary url. This was commited and pushed to ensure
I hadn't made the same mistake.


## Deployment
Deployment was done through github pages and followed this procedure.
* Logging on to github and opening my repository -> clicking on the settings tab -> scrolling down to the "GitHub Pages" section -> Under the "Source" heading the master branch was 
selected and the "root" folder was selected for github to build my page from. -> the "save" button was then clicked and my page was built at [https://futhimhlas.github.io/MS-One/](https://futhimhlas.github.io/MS-One/)

* Running my code locally is done through gitpod. By signing into my github account and accessing my source code through my github account.

## Credits
### Code 
https://css-tricks.com/perfect-full-page-background-image/ -> Here is where I took the css code for the full width backgrounds used in my project

https://stackoverflow.com/questions/17687328/getting-a-link-to-go-to-a-specific-section-on-another-page -> Taught me how to link to a specific part of another html page

# Media
https://www.leaguesplash.com/wp-content/uploads/2013/09/Lucian-Classic.jpg source of 'full-width-lucian.jpg' The image used for my full
width background on my index page

https://www.unrankedsmurfs.com/blog/lol-ranks-explained source of 'challenger.png', 'master.jpg' and 'grandmaster.jpg' the three images found at the bottom of my
index page.

https://rankedboost.com/assassin-tier-list/ source of "adc.png, assassin.png, mage.png, tank.png and fighter.png" used as dividers and also decoration/badges next to champions name.

https://leagueoflegends.fandom.com/wiki/ source of all other images in my project. (Used in te rune-tree, abilities section and items section) 

All gameplay gifs and embed videos I captured myself from the League of Legends game using nvidia shadow play.

The cinematic gif of Lucian battling Thresh came from a [cinematic](https://www.youtube.com/watch?v=ZjvDFvzfxsQ) which was turned into a gif using [Giphy](https://giphy.com/).

## Acknowledgements
### w3schools.com
w3schools was a big help when it came to helping me get my css to do exactly what I wanted. (Specifically my 'plaque' divs)

### Lucian's [u.gg page](https://u.gg/lol/champions/lucian/build)
The inspiration for the responsive bootstrap table came from this site.

### My mentor Rahul
Rahul pointed me towards features like the table and using cloudinary to help the loading times of my site. He also helped me add more personality to my site by suggesting more icons and the collapse feature.

### [Full Width Backgrounds](https://css-tricks.com/perfect-full-page-background-image/)
Provided most of the CSS when it came to this feature

### Slack user JimLynx_lead
JimLynx_lead helped me when after opening my site in my first deploy, none of my links were loading, only bootstrap. He pointed me towards my file paths which were 
denoted incorrectly.