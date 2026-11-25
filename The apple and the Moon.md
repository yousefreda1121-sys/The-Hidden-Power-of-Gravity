# The apple and the Moon

An apple falls straight down. The Moon does not fall at all. In 1666 Newton asked whether one pull could explain both.[1](#fn1) Two rules are enough to find out, and every number on this page is computed live from them.

Gravity: **F = G · m₁ · m₂ / r²**\
Motion: **F = m · a**

## Plate I. The pull between two masses

Every mass pulls on every other mass. Move the sliders and watch the arrows. Press **Mark** to remember the current force, change *one* slider, and read how the force compares. What happens if you double a mass? If you double the distance?

Fig. 1. Two bodies and the pull between them. Arrow length shows the force (it stops growing when it runs out of room).[2](#fn2)

m₁10 m₂10 r10

## Plate II. Throwing the Moon sideways

Gravity does not move the Moon. It changes the Moon’s velocity, a little more every instant, and *a = F / m* says by how much.[3](#fn3) Choose a sideways launch speed and see if the Moon crashes, circles or leaves. Then change the Moon’s mass. Does the path change?

Fig. 2. Earth (blue) and the Moon (grey), seen from above. Blue arrow: velocity. Orange arrow: acceleration, always toward Earth. Both are recomputed at every step.[4](#fn4)

Speed2 Moon mass1

Pick a speed and press Launch. Somewhere between 2 and 5 is interesting.[5](#fn5)

## What you found

Gravity gets stronger with mass and weaker with distance, and a force changes motion, not position. Throw something sideways fast enough and it keeps missing the ground. That is an orbit, and it is the same pull that dropped the apple.

## Notes

1. The story was recorded by Newton’s friend William Stukeley in 1726, from Newton’s own memory. Whether an apple really hit him is uncertain; the question he asked is real. [↩](#r1)
2. Units are normalized so numbers fit on screen: G = 1 on Plate I and G·M = 100 on Plate II. In SI units G is about 6.67 × 10⁻¹¹ N·m²/kg². Only the size of the numbers changes, never the rule. [↩](#r2)
3. The real Moon falls toward Earth by about 1.4 millimetres every second. It never arrives because it also moves sideways at about 1 kilometre per second. [↩](#r3)
4. Time moves in fixed slices of 0.01 using velocity Verlet: update the position, recompute the acceleration there, then update the velocity from the average of the old and new acceleration. Nothing on this page is pre-drawn; the code is this page, so View Source shows all of it. [↩](#r4)
5. Escape speed is √2 times the circular-orbit speed at the same distance. Try to find both. [↩](#r5)