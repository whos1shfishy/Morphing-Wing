# Assembly Guide

This guide describes a suggested assembly order and key setup notes for the Flying Fish morphing wing.

## Parts checklist

Recommended printed parts:
- Central spine / internal frame
- Left and right side shells
- Sliding trailing-edge section
- Two rack components (left and right)
- Two pinion gears sized for the SG90 servo shafts
- Servo mounts and any mounting brackets
- Vertical trailing-edge guide shaft and associated supports

Hardware:
- 2 × SG90 (or similar) micro servos
- Screws or fasteners for securing servos (if needed)
- Any alignment pins or small screws used in the design

## Suggested assembly order

1. **Print all components**  
   Print the central spine, side shells, racks, pinions, trailing-edge section, servo mounts, and any small alignment parts.

2. **Prepare the servos**  
   - Center both SG90 servos (e.g., using a servo tester or microcontroller) so they start from a neutral angle.
   - Press-fit or secure the custom pinion gears onto the servo output shafts.

3. **Install servos into the spine**  
   - Mount both servos into the central spine or internal frame.
   - Ensure they are firmly fixed and aligned so the pinions sit at the correct height relative to the racks.

4. **Install the racks**  
   - Slide the racks into their guides on each side of the trailing-edge structure.
   - Mesh each rack with its corresponding pinion.
   - Verify the teeth engage cleanly without excessive backlash or binding.

5. **Attach the sliding trailing-edge section**  
   - Connect the trailing-edge section to the racks and to the vertical guiding shaft.
   - Ensure the connections allow the trailing edge to move smoothly while staying aligned with the rest of the airfoil.

6. **Check motion before closing the shells**  
   - Gently actuate both servos (by hand or with low-angle commands).
   - Confirm that:
     - Both racks move in the expected direction
     - The trailing edge moves symmetrically
     - There is no significant binding or collisions

7. **Install the side shells**  
   - Fit the left and right side shells over the spine and mechanism.
   - Secure them according to the design (snap-fit, screws, or glue).
   - Make sure the outer surface remains smooth and continuous.

8. **Final motion test**  
   - Run the servos over the intended deflection range.
   - Check that the trailing edge morphs as expected and returns close to neutral when the servos go back to their centered position.

## Setup notes and tips

- **Backlash and clearance**  
  Aim for low backlash in the rack-and-pinion mesh, but avoid over-tight engagement, which can cause binding and excessive friction.

- **Servo synchronization**  
  Start both servos from the same neutral position. If driving them electronically, ensure they receive matched signals for symmetric motion.

- **Print tolerances**  
  Tolerances may need tuning depending on printer, material, and settings. Slight scaling or light sanding of racks and guides may be required for smooth motion.

- **Maintenance**  
  The three-piece structure and modular parts make it easy to swap out a damaged rack, pinion, or trailing-edge section without reprinting the entire wing.
