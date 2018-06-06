# 2018-interactives
See our [current Code Repository](https://github.com/benetech/accessible-interactives) which is a work in progress for some of the areas we are thinking of and have already started building this out.

## Background Information
 [Phet Interactive Simulations](https://phet.colorado.edu/)

## Possible Projects
* Smoothing function for draggable items. Create a function that can take in array of xy coordinates and return an array of xy coords smoothened to a coherent path. As a simplification, think of it as the smoothing of a curve; the first path is a person moving a mouse and then we "untangle" the movements to produce the user's "intention." Maybe using Kalman filtering? Then possibly plug this into [PhET Simulation scaffolding](https://phet-dev.colorado.edu/html/diagram-demo/1.0.0-dev.1/phet/diagram-demo_en_phet.html) to see it in action.
* Drag and Drop where path matters. Perhaps it's its own topic, and maybe an expansion on the bullet above. Can we make a smoothing curve accurate enough to effect the intentional path, not just destination. To dodge "bad" areas on the way to the end target of the drag, or to follow a specific path.
* Making IOS 11 multi-item Drag and drop sessions for the Web (Changes in ARIA for Drag and Drop) consider best practices.
* Pick a difficult PhET Interaction and work to make it navigable with more than mouse technology. One strategy is to try to map it to native HTML, ARIA, and, when needed, custom javascript. a goal for any of these problems would be to figure out a solution that could be generalized to other interactions outside of PhET. These simulations outline the potential difficulties of making an interaction accessible, but the work done on any of these problems can have as much or as little to do with the actual simulations as we choose.
    * "Pulling apart" different cards within a freely moving, draggable interface, [Make a Ten](https://phet.colorado.edu/sims/html/make-a-ten/latest/make-a-ten_en.html).
    * Dragging out of a toolbox, [Function Builder - easier](https://phet.colorado.edu/sims/html/function-builder-basics/latest/function-builder-basics_en.html), and [Circuit Construction Kit - harder](https://phet.colorado.edu/sims/html/circuit-construction-kit-dc/latest/circuit-construction-kit-dc_en.html)
    * Manipulating a 3D model. [Molecule Shapes](https://phet-dev.colorado.edu/html/molecule-shapes/1.1.12/molecule-shapes_en.html)
    * Drag and drop where the speed of the drag matters, [Faraday's Law](https://phet.colorado.edu/sims/html/faradays-law/latest/faradays-law_en.html)
    * Large number of drop targets [Area Builder](https://phet.colorado.edu/sims/html/area-builder/latest/area-builder_en.html).

## Set Up

* Depending on what project we decide on, setting up a PhET development environment may be important to the work. Please see the "Getting Started" section for your OS here https://docs.google.com/document/d/1Ys1EiwnqQGYuzGOcQSr4uXDes35mF1v1XhMZIl10nk8/edit# to get set up with the initial github repos. 
* Next, clone the diagram demo PhET sim located at https://github.com/phetsims/diagram-demo/, with `git clone https://github.com/phetsims/diagram-demo.git`. This sim will serve a barebones PhET architecture that we can expand on with out code.
* Clone one more dependency that is needed for this demo: `git clone https://github.com/phetsims/twixt.git`.
