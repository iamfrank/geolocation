# GeoLoc

Javascript convenience functions for accessing and using Geolocation Web API

## Getting started

```Javascript
import GeoLoc from "./index.js";
const geol = new GeoLoc();

document.body.addEventListener("change:geolocation", (ev) => {
  console.log("Got position from event", ev.detail);
  console.log(geol.coordinate)
});

const position = await geol.getPosition();
console.log("Got position from Promise", position);
console.log(geol.coordinate)
```
