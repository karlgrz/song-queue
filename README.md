Song Queue
----------

![Song Queue screenshot](/screenshot.png =421x444)

After cloning the repository you should run `npm install`, followed by `npm start`. You should now be able to visit http://localhost:8008 to view the application.

This is intended to be run as a service somewhere for my personal use at band practice.

## JSON endpoints

`/keys` returns an array of all the possible keys, including sharp and flat keys.

`/scale/:key-:mode` returns an array named for the mode, with the notes of the requested scale, e.g. `/scale/ab-minor-pentatonic`, if available. If `:mode` is major or minor, the corresponding pentatonic scale is also returned.

`/scales` returns an array of the available scales.

`/scales/:key` returns an object of arrays with scales in the provided key for each of the available scales.

### Available scales

+ major
+ minor
+ dorian
+ major pentatonic
+ minor pentatonic
