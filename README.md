# Flying Fish Morphing Wing

A compact morphing wing concept featuring a **sliding trailing-edge mechanism** driven by a custom dual rack-and-pinion system. This repository documents the sliding-mechanism wing from the UNSW DESN1000 morphing wing project, focusing on the design, CAD structure, assembly, and visual documentation for the `Flying Fish` concept.

## Project overview

The Flying Fish is a 3D-printed morphing wing based on a NACA 0015 airfoil profile with a 150 mm chord and 90 mm span. The design uses a sliding, morphing trailing edge to vary wing camber, with bilateral actuation intended to keep the trailing-edge motion symmetrical and reduce twist.

The project evolved from an earlier single-servo prototype that proved the rack-and-pinion concept worked but highlighted issues such as uneven trailing-edge deflection, twisting under load, and high torque demand on a single actuator. The final Flying Fish design addresses these issues with a dual-servo layout and mirrored mechanisms.

## Key features

- Dual-servo actuation using two SG90 servos, one on each side of the wing
- Custom rack-and-pinion transmission converting servo rotation into linear trailing-edge motion
- Sliding trailing-edge section integrated into the wing structure
- Vertical shaft near the trailing edge to reduce oscillation and maintain primarily horizontal motion
- Lightweight, fully 3D-printed construction for fast iteration and low material usage
- Three-piece assembly (central spine plus two side shells) designed for simple assembly and maintenance

## Design concept

The core idea behind the Flying Fish is to create a morphing trailing edge that can continuously adjust camber without relying on discrete hinged control surfaces. By embedding a rack-and-pinion mechanism inside the wing, servo rotation can be converted into controlled linear motion, pulling or pushing the trailing-edge section.

The initial single-servo concept demonstrated that PLA parts could support morphing, but concentrated load into a single actuator. This produced:
- Asymmetric trailing-edge movement
- Twisting of the morphing section
- Higher torque demand and a greater risk of servo stalling

The dual-servo configuration distributes the load across both sides of the wing and pulls the trailing edge more evenly, improving symmetry and reducing torsional effects.

## Mechanism summary

Each SG90 servo drives a small pinion gear that meshes with a straight rack mounted along the internal trailing-edge structure. As the servo rotates, the pinion drives the rack linearly, which in turn slides the morphing rear section to change camber.

Because the mechanism is mirrored on both sides:
- Both racks move in a coordinated manner
- The trailing edge can be pulled symmetrically
- Twisting and binding are reduced compared with a single central actuator

A vertical shaft near the trailing edge ties the moving section to the upper skin and helps keep the motion primarily horizontal, reducing oscillations during actuation.

## Airfoil and structure

- Airfoil: NACA 0015
- Chord length: 150 mm
- Span: 90 mm
- Materials: PLA for early prototypes, PETG for later versions to increase flexibility and morphing capability
- Structural layout: central internal spine plus two side shells forming the full airfoil profile

The NACA 0015 profile was selected because:
- Its 15 % thickness provided sufficient internal volume for servos, racks, and structural elements
- It offered a good balance between aerodynamic behavior and practical manufacturability with FDM 3D printers

## Repository structure

```text
.
├── README.md
├── cad/
│   ├── assemblies/
│   ├── parts/
│   ├── exports/
│   └── screenshots/
├── images/
│   ├── prototype/
│   ├── final-wing/
│   ├── mechanism/
│   └── presentation/
└── docs/
    ├── project-summary.md
    ├── mechanism-notes.md
    ├── assembly-guide.md
    └── image-checklist.md
```

### `cad/`

Store all CAD assets for the wing.

Suggested subfolders:
- `assemblies/` – full wing assemblies (e.g., complete Flying Fish assembly)
- `parts/` – individual parts such as racks, pinions, side shells, central spine, trailing-edge section, and servo mounts
- `exports/` – neutral/shareable formats such as STEP and STL
- `screenshots/` – CAD renders and orthographic views, including section cuts and annotated views of the mechanism

### `images/`

Store all project images and visual references.

Suggested subfolders:
- `prototype/` – early proof-of-concept builds, single-servo version, cardboard/PLA trials
- `final-wing/` – final assembled Flying Fish in various views
- `mechanism/` – close-ups of racks, pinions, servo mounting, sliding trailing-edge details, and section cuts
- `presentation/` – images from demo/presentation day, wind-tunnel setup, table display, and team photos (if desired)

### `docs/`

Store written documentation that supports the repository.

Recommended files:
- `project-summary.md` – overview of the project, design intent, and evolution
- `mechanism-notes.md` – detailed explanation of the rack-and-pinion architecture and dual-servo design
- `assembly-guide.md` – basic assembly order and important fit/tolerance notes
- `image-checklist.md` – list of recommended photos/diagrams to include

## Hardware and control

This project focuses on the mechanical design rather than custom control firmware. The morphing mechanism can be driven using:
- Two SG90 (or similar) micro servos
- A simple microcontroller (e.g., Arduino) providing PWM signals

For basic demonstrations, both servos can be driven with identical signals so the racks move symmetrically. More advanced control schemes can add:
- Separate channels for each servo
- Potentiometer-based manual control
- Automated morphing profiles

## How to use this repository

1. Clone the repository.
2. Open the CAD assemblies in your preferred CAD package.
3. Export or use the provided STLs from `cad/exports/` for printing.
4. Print and assemble parts following the `docs/assembly-guide.md`.
5. Add your own photos and screenshots into the `images/` folders.
6. Optionally extend the mechanism or control scheme and document changes.

## Short description (for GitHub)

> Compact 3D-printed morphing wing with a dual-servo rack-and-pinion sliding trailing-edge mechanism based on a NACA 0015 airfoil.

## Topics / tags

`morphing-wing` `airfoil` `naca0015` `cad` `aerodynamics` `3d-printing` `servo` `rack-and-pinion` `mechanical-design` `unsw` `desn1000`
