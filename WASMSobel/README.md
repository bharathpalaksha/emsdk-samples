## WASMSobel
Simple example to show comparing JS/WASM implementations for a Sobel filter
Compile change.c with emscripten using:
```
emcc -o change.js change.c  -lm -O3 -s WASM=1 -s EXPORTED_FUNCTIONS="['_change']" -s BINARYEN_IMPRECISE=1
```

To Run:
```
source ../emsdk/emsdk_env.sh
emrun index.html
```
Original Sobel algorithm created by [Miguel Mota](https://github.com/miguelmota/sobel), and adapted for this demo under the terms of the original [license](https://github.com/JasonWeathersby/WASMSobel/blob/master/SOBEL-LICENSE.md)


### Exercise
Write commented fundtions 1 and 2 in sobel.js
