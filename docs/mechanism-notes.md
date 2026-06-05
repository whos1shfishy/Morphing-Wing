# Mechanism Notes

## Core mechanism

The Flying Fish uses two mirrored rack-and-pinion systems to drive a sliding trailing edge. Each servo is mounted inside the wing and equipped with a small pinion gear fixed to its output shaft. The pinion meshes with a straight rack aligned along the trailing-edge structure.

When the servo rotates:
- The pinion gear turns with it
- The rack translates linearly
- The morphing trailing-edge section is pulled or pushed, changing the airfoil camber

Because this layout is duplicated on both sides of the wing, both racks move in a coordinated fashion, helping the trailing edge morph symmetrically.

## Why dual servos

The initial concept used one central servo driving a single rack-and-pinion. While this validated the mechanical idea, it created several issues:
- The single actuator carried all aerodynamic and structural loads
- The trailing edge deflected unevenly, leading to twisting
- The torque demand on one servo increased, making stalls more likely at higher deflections

Moving to a dual-servo system provides several advantages:
- Load is shared between two actuators
- Each side of the trailing edge is driven independently but symmetrically
- Twisting is reduced, improving the predictability of camber changes
- The system scales better for higher morphing deflections

## Structural guidance

A vertical shaft is positioned near the trailing-edge section to connect the moving morphing part to the upper skin. This shaft:
- Helps maintain alignment of the sliding section
- Guides motion to be primarily horizontal rather than allowing large vertical oscillations
- Works together with the outer shells to preserve the airfoil shape during morphing

The surrounding side shells capture the racks and trailing-edge section, forming a continuous aerodynamic surface while allowing internal components to slide.

## Material considerations

Early builds used PLA due to availability, which provided stiffness but limited flexibility. Later iterations used PETG to increase elasticity and allow greater morphing range while still maintaining structural integrity.

Key trade-offs:
- PLA: stiffer, easier to print, higher risk of fracture in highly flexed regions
- PETG: more flexible, better for morphing sections, requires more tuning of print settings

The combination of PETG trailing-edge components and internal racks allowed the trailing edge to deform under servo actuation while returning close to its original shape when unloaded.
