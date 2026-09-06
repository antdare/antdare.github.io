# antdare.github.io
```javascript
// setup() is called once at page-load
function setup() {
    createCanvas(800,800); // make an HTML canvas element width x height pixels
}

// draw() is called 60 times per second
function draw() {
    let hr = hour();
    let min = minute();
    let sec = second();
	
    background(135, 206, 235);
    textSize(24);

    // Print Hours
    for(let x = 0; x < 4; x += 1){
    	fill(4, 26, 64);
      text(x, 30, (x+1)*30)}
    for(let x = 4; x < 5; x += 1){
      fill(250, 134, 7);
      text(x, 30, (x+1)*30)}
    for(let x = 5; x < 6; x += 1){
      fill(250, 150, 27);
      text(x, 30, (x+1)*30)}
    for(let x = 6; x < 7; x += 1){
      fill(252, 176, 51);
      text(x, 30, (x+1)*30)}
    for(let x = 7; x < 9; x += 1){
      fill(254, 204, 81);
      text(x, 30, (x+1)*30)}
    for(let x = 9; x < 11; x += 1){
      fill(255, 228, 105);
      text(x, 30, (x+1)*30)}
    for(let x = 11; x < 13; x += 1){
      fill(255, 245, 123);
      text(x, 30, (x+1)*30)}
    for(let x = 13; x < 15; x += 1){
      fill(255, 228, 105);
      text(x, 30, (x+1)*30)}
    for(let x = 15; x < 17; x += 1){
      fill(252, 176, 51);
      text(x, 30, (x+1)*30)}
    for(let x = 17; x < 18; x += 1){
      fill(252, 176, 51);
      text(x, 30, (x+1)*30)}
    for(let x = 18; x < 19; x += 1){
      fill(250, 150, 27);
      text(x, 30, (x+1)*30)}
    for(let x = 19; x < 20; x += 1){
      fill(250, 134, 7);
      text(x, 30, (x+1)*30)}
    for(let x = 20; x < 24; x += 1){
      fill(4, 26, 64);
      text(x, 30, (x+1)*30)}
    // Print Minutes
    for (let y = 0; y < 24; y += 1){
      fill(y);
      text(y, 90, (y+1)*30)}
    for (let y = 24; y < 48; y += 1){
      fill(y);
      text(y, 150, (y-23)*30)}
    for (let y = 48; y < 60; y += 1){
      fill(y);
      text(y, 210, (y-47)*30)}
    // Print Seconds
    for (let z = 0; z < 24; z += 1){
      fill(60 - z);
      text(z, 270, (z+1)*30)}
    for (let z = 24; z < 48; z += 1){
      fill(60 - z);
      text(z, 330, (z-23)*30)}
    for (let z = 48; z < 60; z += 1){
      fill(60 - z);
      text(z, 390, (z-47)*30)}
  
    // Hour Hand
    noFill();
    strokeWeight(4);
    square(26, hr*30, 35);
    // Minute Hand
    noFill();
    strokeWeight(4);
    if(min<25){
      square(86, (min-1)*30, 35)}
    if(24 < min < 49){
      square(146, (min-24)*30, 35)}
    if(48 < min < 61){
      square(206, (min-48)*30, 35)}
    // Second Hand
    noFill();
    strokeWeight(4);
    if(sec<25){
      square(266, sec*30, 35)}
    if(25<=sec<49){
      square(326, (sec-24)*30, 35)}
    if(49<=sec<61){
      square(386, (sec-48)*30, 35)}
}
```
