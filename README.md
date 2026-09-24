# PointBalls

The second computational physics exploration by a CS student turned Physics student, turned CS student again after abandoning the project for the first time.

## About

The repo contains three Jupyter notebooks. One describes the RK4 method and (will) contain a script visualizing the calculation process, another describes the Barnes-Hut N-body algorithm and (will) contain a script visualizing the process, and the last contains the N-body simulator itself.

## Features

Two simulation methods - naive and basic Barnes-Hut, both feeding into an RK4 integrator.
Displays for total energy and elapsed time, so you can see how badly Barnes-Hut doesn't conserve energy with the current parameters, how how good RK4 is at keeping errors down.
Gravitational softening, to prevent weirdness (but creating a non-Newtonian gravity law)
Lovely pictures.

## Things to do here

Run the n-body simulator, trying both the naive and Barnes-Hut methods to see the difference, which you can do by changing if ```rk4_naive()``` or ```rk4_bh``` is called in ```update()```
- Run ```rk4_naive()```, with ```softening = 0```. See how well that goes!
- Run ```rk4_naive()```, this time with ```softening = 2```.
- Run ```rk4_bh()```, with ```THETA = 0``` . It's exactly identical to the naive case, as BH degenerates to the naive simulation in that case.
- Play with ```THETA = 0.2, 0.3,``` etc. and see where the errors begins to blow up in the energy
Read my descriptions and diagrams of:
- The Barnes-Hut simulation. In case you have no idea what recursion or a tree is. I put a lot of time into these Google Slides drawings, so if you do know what those are please look anyways.
- RK4 integration. Where I have used someone else's Wikipedia image, but gave them credit.

## Features to be done

- Tune the simulation parameters
- UI for:
  - Number of bodies
  - The parameters (```THETA, softening```)
  - Toggle between naive and BH
- Implement my BH improvements
  - Multipole Expansion
  - Delta Parameter (COM skew)
- Animations for BH and RK4 demo notebooks
- REWRITE IT IN ~Rust~ C++



```isn't my code highlight cool? I didn't know how to make these until right now```
