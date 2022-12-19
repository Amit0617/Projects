# Projects
My Projects, Your projects, Everyone else's Projects. A projects showcase for programmers who are busy on something more priority. Fork. Deploy. Share.

## GOAL
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
- [ ] Offer light mode and dark mode options.
- [ ] Sound with every shape transition would be awesome.
