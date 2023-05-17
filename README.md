# Dissipative Particle Dynamics Simulation

## Problem A
https://www.youtube.com/watch?v=uFnVnSD1wJM

In this section we only look at the behaviour of fluid particles. The boundary of the walls are periodic and the conservative force coefficient $aij = 25$. The result of running this simulation for 1000 iterations is illustrated below in figure 1.

<p align="center">
<img width="655" alt="image" src="https://github.com/ShmamShmiff/dissipative-particle-dynamics-simulation/assets/25768413/9010ab27-41e7-4474-936b-9c07eaf20709">
</p>

Here, we can see the simulation converged to a solution in which fluid particles are approximately equally distanced from one another. We also notice the system temperature initially spikes up after the system initiation because particles were originally randomly placed in an unbalanced config- uration. Last, we notice the total system momentum remains 0 (at least very close at $10^{−14}$) as expected.

## Problem B
https://www.youtube.com/watch?v=Td5D3pKSsX4

Here, we simulate Couette flow with 42 chain molecules. For simulation setup, we have two walls on either side of the boundary with particles flowing in opposite direction at constant velocity. All particles are placed randomly in the simulation. The values for $v_{wall}, K_S$, $r_S$, and $a_{ij}$ are initialized as described in the assignment handout. The results of this simulation after 1000 iterations can be seen below in figure 2. Additionally, a youtube video of the simulation is provided; showing the evolution of movement of particles.

<p align="center">
<img width="680" alt="image" src="https://github.com/ShmamShmiff/dissipative-particle-dynamics-simulation/assets/25768413/09537a63-dd5a-4e05-93d5-8fa479716351">
</p>

Here we see a behaviour where particles move to an ordered state. 1) Fluid and molecule particles (A and B) are repelled from the walls and find themselves pushed together. 2) Chain molecules are attracted to one anther were the B particles align together to form clusters. 3) Fluid particles form ’halos’ around the molecule clusters as they are pushed away. 4) We also see fluid particles on either side of the simulation slightly move in the direction the walls are moving. (note this can be seen in the video)

We also see temperature follows a similar pattern to problem A where we measure an initial spike and then a tapering to around 5 units where the system is in a more-balanced state. Total momentum, however, differs from problem A as it is not constant. Here we notice fluctuations in total momentum. This is as expected as we are not allowing the effect of particles influence the acceleration of wall particles.

## Problem C
https://www.youtube.com/watch?v=0uCf3rC0ZOk

Here we simulate Poiseuille flow with 10 ring-molecules. The initial setup conditions are as de- scribed in the assignment handout. Walls do not move and all non-wall particles have a constant, applied upwards acceleration force of 0.3. Additionally, $K_S = 100$, $r_S = 0.3$ and $a_{ij}$ are initiated as described. The results below in figure 3 show the simulation after 1000 iterations. The simulation was also run for 10,000 iterations to observe the effects of turbulence (refer to youtube video for recording).

<p align="center">
<img width="694" alt="image" src="https://github.com/ShmamShmiff/dissipative-particle-dynamics-simulation/assets/25768413/9c97c127-2fe9-4969-ae0b-ed9adeee76b3">
</p>

Initially we see a result similar to part B where particles are repelled from the two walls and pushed to the center. We also see the rings remain their shape and push fluid particles away to form a ’halo’ effect. The fluid particles also align themselves to a more ordered state. Initial temperature is also similar with a spike and total momentum is not kept constant.

However, the effects on total momentum and temperature go further. We see total momentum continuously increases and temperature also increase after initialization. This is expected as we are constantly applying an upwards acceleration force to all fluid, A, and B particles. Therefore mean velocities are not conserved.

<p align="center">
<img width="633" alt="image" src="https://github.com/ShmamShmiff/dissipative-particle-dynamics-simulation/assets/25768413/1f8f3646-de63-4701-b918-79c505de7079">
</p>

This effect is greatly amplified at around 10,000 iterations were we see a large increase in both total momentum and system temperature. We also observe turbulence in the fluid, A, and B particles as they pass a certain velocity. This motion can be seen in the linked youtube video. Here, we notice the particles near the edge of the walls move chaotically and less predictably compared to those particles in the center of the simulation. I believe this is because the walls are not flat - comprised of small crevasses in which fluid particles can enter - and induce a friction-like resistance to the particles moving past. This throws those bordering particles into a chaotic movement thereafter effecting neighboring particles. We also notice the fluid particles and ring molecules at the sides move slower than those at the center.


