## Goal

Track movement of social / political groups (refugees, military units, immigrantion waves) based on live news events and visualize onto 3D map

## Steps

1. Wireframe / notes

   1. High level map UI in Figma
   2. Dropdown for search groups in Figma

2. Design map in Mapbox Studio

3. Design search on zoom / on navigation functionality

   1. event handling (zooming, panning) [Mapbox-Actions](https://docs.mapbox.com/android/navigation/mapgpt/actions/)
   2. Caching markers / data outside scope of map view so that they can be easily shown once in view again

4. Design placename search UX. How are you going to choose what to search for based on map view since it is not possible to search every placename in view?

   1. Define criteria for evalutating significance of a place
   2. Define criteria for evaluating centeredness of a place on the map

5. Azure News Search for place name + search group(s)

6. Define criteria for relavent article results and filter out irrelivant ones

7. Use AI library to parse for directional information

   1. Might need reverse geolocation API to get accurate lat/lng coordinates to place models

8. Use blender to create 3D models and rotate and place them based on coordinates [and directional criteria]

## Technologies used

### Libraries / APIs

- Mapbox
- Chat GPT JS
- Azure News API

### Markers

- Blender

### Frameworks / Scripts:

- Next JS
- Typescript
- Tailwind CSS

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
