# Ecommerce Project III

Live version: https://tycode-ecommerce-final.netlify.app/

## Project Overview

## Built With

<p dir="auto">
  <a target="_blank" rel="noopener noreferrer" href="https://camo.githubusercontent.com/0c3a16a22ae058cfe38a06dc9ea16404cf006409262f547c9ccfa3ec8b30f71e/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2d48544d4c352d4533344632363f7374796c653d666c61742d737175617265266c6f676f3d68746d6c35266c6f676f436f6c6f723d7768697465"><img alt="html5" src="https://camo.githubusercontent.com/0c3a16a22ae058cfe38a06dc9ea16404cf006409262f547c9ccfa3ec8b30f71e/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2d48544d4c352d4533344632363f7374796c653d666c61742d737175617265266c6f676f3d68746d6c35266c6f676f436f6c6f723d7768697465" data-canonical-src="https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&amp;logo=html5&amp;logoColor=white" style="max-width: 100%;"></a>
  <a target="_blank" rel="noopener noreferrer" href="https://camo.githubusercontent.com/af676aa114d3e054bb2d7b823f8b1dbf1814214d2c6f49e6a6cb70ab1837bd59/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2d4353532d3066363166613f7374796c653d666c61742d737175617265266c6f676f3d43535333266c6f676f436f6c6f723d7768697465"><img alt="CSS" src="https://camo.githubusercontent.com/af676aa114d3e054bb2d7b823f8b1dbf1814214d2c6f49e6a6cb70ab1837bd59/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2d4353532d3066363166613f7374796c653d666c61742d737175617265266c6f676f3d43535333266c6f676f436f6c6f723d7768697465" data-canonical-src="https://img.shields.io/badge/-CSS-0f61fa?style=flat-square&amp;logo=CSS3&amp;logoColor=white" style="max-width: 100%;"></a>

 </p>

## 2. Requirements

We are going to implement some cool new features this week now that we have all of the React building blocks at our disposal.

What you need to have done at the end of the week:

- There should be a context that stores the `id` of all of the favourites of the user. You should not store the whole object!
- For the images in the product list as well as the product details page there needs to be a heart that if clicked will update the favourites array in the context. The heart should show the right svg file depending if it is favourited or not.
- Your app should have a favourites page to list all of the products the user has favourited. You will need to perform multiple fetches as you only have the `id` of the favourites.
  > Storing the whole object would make this easier of course and in this example would probably be a better solution, but we want to challenge you a bit by adding a multiple fetch scenario.
- Add a navigation bar at the top that handles routing between `/` and `/favourites`. The `/favourites` route should go the favourites page.
- If you did the same things as us then in the Products and ProductDetails pages you will have quite a lot of duplicate logic concerning the `loading` and `error` states of all those requests. Fix that by creating a `useFetch` custom hook.
  > Your custom hook will have a couple of challenges. The URL for the products changes and you will have to perform that fetch whenever the user clicks a category so you will need to give the user of your hook the option to do that.
  > Extra challenge: We purposefully do not say Favourites page here as that would make the custom hook even more difficult to build. If you are up for the challenge, add functionality to your hook for multiple fetches!
