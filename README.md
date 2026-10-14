# TestBot Drive Sim

A browser simulator for Bionic Beef's 2026 TestBot. It runs a JavaScript port of the robot's drive, shooter, intake and vision code (from `2026TestBot` at `94fb4fb`) on a 3D REBUILT field. Drive it with the keyboard or an Xbox controller, and change any constant to see how it affects the robot.

## Controls

| Key | Controller | Action |
| --- | --- | --- |
| W A S D | Right stick | Drive (the robot can strafe) |
| Q E / ← → | Left stick | Turn |
| Space | RT | Hold to shoot |
| Shift | LT | Hold to run the indexer backwards |
| 1 | A | Raise / lower the intake |
| 2 / 3 | B / X | Rollers in / out (toggle) |
| [ / ] | LB / RB | Nudge the intake hinge down / up |
| R | Start | Zero the gyro |
| F / G | Y / Back | Auto-aim and shoot / stop the shooter |
| C / H | | Change camera / show help |

Press **H** in the sim for the full guide.

## Deploying

It's one static `index.html` with no build step. Import the repo into Vercel with the "Other" framework preset and no build command, and it serves as-is. Three.js and the fonts load from CDNs.

To run it locally, run `python3 -m http.server` in this folder and open http://localhost:8000.
