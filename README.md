# Outlaw VR (Atari 2600 First-Person Remake)

A first-person 3D WebXR and desktop remake of the classic Atari 2600 Outlaw showdown.

## Multiplayer Opposite-Sides Showdown:
- **Host (Room Creator):** Always assigned to **WEST SIDE** (Player 1, Blue, `X = -13`), facing East towards the opponent.
- **Guest (Room Joiner):** Always assigned to **EAST SIDE** (Player 2, Red, `X = +13`), facing West towards the opponent.
- **Opponent Representation:** Both clients explicitly initialize and synchronize the remote player on the opposite side of the canyon across the neutral obstacle zone.
- **Boundary Clamping:** West player is strictly bounded to `X: [-15.5, -6.5]`, East player is strictly bounded to `X: [+6.5, +15.5]`.

## Other Features:
- **Clickable Quest VR Restart:** Right controller laser points at side wall scoreboards; pulling the trigger restarts the match anytime without shooting.
- **Large Scoreboard Numbers:** 170px bold numbers with cyan/rose contrast.
- **Platform Selection Upfront:** Choose **Desktop Browser** or **Oculus Quest VR** at the top of the start screen.
- **No Position Reset on Hit:** Getting hit preserves your position.
- **Configurable Fire Rate (Unlimited Ammo):** Default 3 bullets per 1.0s.
- **Authentic Pioneer Covered Wagons:** Authentic 1800s Conestoga prairie schooners with rolling wooden spoked wheels and ribbed canvas bonnets.

## Quick Start (Local Run)

```bash
python3 -m http.server 8000
```
Then open: `http://localhost:8000`
