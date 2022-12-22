# Projects
My Projects, Your projects, Everyone else's Projects. A projects showcase for programmers who are busy on something more priority. Fork. Deploy. Share.

## Demo
<!-- https://user-images.githubusercontent.com/71893015/209192137-4ef87d01-4e51-4e4d-bd0c-389588a08b73.mp4   -->

[![Demo](https://i9.ytimg.com/vi/DcRUrq8FwfA/sddefault.jpg?sqp=CJyvkp0G-oaymwEmCIAFEOAD8quKqQMa8AEB-AHSBoAC4AOKAgwIABABGFUgRShyMA8=&rs=AOn4CLDd1nxdaDd4CMQIiqJFKXxJeKr7ig)](https://youtu.be/DcRUrq8FwfA)

## How to get it setup?
1. Fork it.
2. Deploy it on Github pages.
3. Enjoy. That's it.

## How does it works?
Basically there is one fixed pattern of the url of the deployed project. So if you would fork this repository, url of the deployed page would be `https://USERNAME.github.io/Projects`. Therefore, using some string operations username can be extracted and can be used with github api to fetch all user repositories. Then that data is used to render your project showcase!

## How to Customize?
If you want some selected repositories in your projects showcase, then you can use this API `https://api.github.com/users/${username}/repos?&sort=pushed&per_page=100` to get all of your repositories upto 100 (Check docs for more). Save the response as `repos.json` file, remove those objects you don't want or reorder that according to your choice and add it into the repository. It will first check for that and only in absence of that file, it calls Github api.

## GOAL of the Project
It should be generalised and templatised completely, so that can be turned ON after forking and opting for hosting by GitHub. 
 
### Steps
- [x] Use GitHub api endpoint /{user}/repo.
- [x] Parse it, use Name(clickable with the link to that repo) and description in a card.
- [ ] Cards with great bevel, small nice circular corners with appropriate light and shadows (experiment) with autorotation.
 - [ ] Fetching Images by link preview for social media preview to comeup as image would be a huge plus.
- [ ] Scene(Background) should be matrix like floor.  
 ~1 card should be visible at once. Next card should emerge with sideways scroll(arrows for next and previous cards).~ Grids, sphere and various shapes with some animation and control is better for sure.
- [x] GitHub Api is little conky, returns 30 repo in one request and may give different set of repos on different instances. So, to manage that and to make a predictable or a fixed response of website to various people configurable through internal .json file should be allowed.

#### Intermission steps
- [ ] Add an svg on hover for external link.
- [x] Try a smoother foggy substr for description.
~Readjust font size according to the length of string.~ Readjusting causes large no. of recursions, call for only few large ones (maybe check size or no. of characters to limit that.)
- [ ] Add layers for sliders with adjusting options- like radius of sphere, distance between cards, their positioning, various colors.
- [x] Offer light mode and dark mode options.
- [ ] Sound with every shape transition would be awesome.
