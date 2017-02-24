Things to do:

1) find a thicker arrow svg
2) change out photos
3) switch out bear photo and apply overlay to replacement (see code below)






archive: 

Deep Water in a Sleeping Volcano

Surrounded by cliffs almost 2,000 feet high and boasting a picturesque island a violent volcanic past, Crater Lake is also home to hikes in old-growth forest and cross-country ski trips in the winter months. Many of the roads and facilities close during the winter, but the park is open and accessible all year long.


CSS overlay code from "CSS Transitions and Transforms" course
"Animatable CSS Properties" video:

/* ---- Photo Overlay ---- */
.photo-overlay {
  color: #fff;
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0; 
  left: 0;
  padding-left: 20px;
  padding-right: 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: rgba(0,0,0, .65);    // this is the item that darkens the photo.  It is on top of the photo in the css.
}

/* ---- Photo Overlay Transition ---- */

.photo-overlay {
  opacity: 0;
  transition-property: opacity;
  transition-duration: .5s;
}

.photo-overlay:hover {
  opacity: 1;
}