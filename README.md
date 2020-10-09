# Animated Template

![Animated Template](assets/images/snapshot.PNG)

## Overview
- Animated template using a [Creative Tim Tailwind Starter Kit](https://www.creative-tim.com/learning-lab/tailwind-starter-kit/presentation)

## Technologies

- [Tailwind Starter Kit](https://www.creative-tim.com/learning-lab/tailwind-starter-kit/landing)
- Animation from [AOS | Animate On Scroll Library](https://michalsnik.github.io/aos/)
- Loading 3rd party .js scripts effectively was researched in this [Google article](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/loading-third-party-javascript). 
  - Contemplated using `<script async>` or `<script defer` to download the AOS.js 3rd party library. Decided on `<script defer>` in the head. **Why?** With defer, parsing finishes just like when we put the script at the end of the body tag, but overall the script execution finishes before-hand, because the script has been downloaded in parallel with the HTML parsing. This scenario will trigger the faster domInteractive event that is used for page loading speed. With async, the order in which your script will execute varies based on how fast the script is fetched, so order can be compromised. Futhermore, async scripts are executed inline and pause the parsing of the HTML. Rule of thumb is that async should be used for packages that do not rely on any other scripts. 

## Credits

### Content

- Template from [Creative Tim](https://www.creative-tim.com/)
- Icons from [Font Awesome](https://fontawesome.com/)
- Images from [Unsplash | Paweł Czerwiński](https://unsplash.com/@pawel_czerwinski)
- User images from [Random User Generator](https://randomuser.me/)
