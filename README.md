# ACCRETE (Update 0.1.0)
### Planetary system creation simulation in the browser, or the server.

The codebase has been completely reimplemented from scratch and in a form that more **closely resembles that put forth in the original Dole paper**.

### Usage
For now, just use accrete.js, which includes each module concatenated in order. Include that script in any environment and the following will output your basic planet data for a system similar to our own:

#### Browser
```javascript
<script src="accrete.min.js"></script>
const system = new Accrete.System();
system.create();

const planets = system.planets;
```

#### Node
```javascript
import Accrete from 'Accrete';

const system = new Accrete.System();
system.create();
const planets = system.planets;
```

### Goals
- [x] Organize the codebase into a more modern, and JavaScript friendly structure.
- [x] A full build process for Browser/Node scripts and modules.
- [ ] Implement a good chunk of [StarGen's](http://www.eldacur.com/~brons/NerdCorner/StarGen/StarGen.html) features.
- [ ] Live WebGL view and screenshot options for created systems.
- [ ] Other cool things to take advantage of this amazing program.

### History of Ac(c)rete

Accrete.js is a port of the awesome planetary system simulation algorithm, [Accrete](http://www.rand.org/pubs/papers/P4226.html) to JavaScript. Originally published* and partly programmed (via FORTRAN) by the amazing Stephen H. Dole. Almost a decade later Carl Sagan and Richard Isaacson refined Dole's model -- which shortly thereafter was also implemented in FORTRAN, and again elaborately and academically published by Martin Fogg.

The late 80's came and Matt Burdick brought this priceless program to the masses (via Turbo Pascal and C). Since then, many versions of *Accrete* have popped up around the internet, adding varying degrees of planetary specifics the most notable (and ingenious) being [Jim Burrow's](http://www.eldacur.com/~brons/) implementation [StarGen](http://www.eldacur.com/~brons/NerdCorner/StarGen/StarGen.html). [Ian Burrell's](http://znark.com/) [Java port](http://znark.com/create/accrete.html) is another great up-to-date example (and a huge help in Accrete.js).

### THANK YOU
Nothing here could have ever (ever, ever, ever) been done without the following amazing, generous, and brilliant people:

- Stephen H. Dole
- Carl Sagan
- Richard Isaacson
- Martin Fogg
- Matt Burdick
- Jim Burrow
- Ian Burrell
- The many brilliant minds that have contributed their knowlege to, and insights into our awe-inspiring universe.

* The original Dole Paper can be [viewed here](http://www.rand.org/pubs/papers/2005/P4226.pdf).
