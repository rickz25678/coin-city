# Big update: test checklist

This branch (`big-update`) has the next version of Coin City. It is **not live yet**. The live game only changes when this branch is merged into `main`.

## How to play the test version

1. Download this branch: **Code → Download ZIP** on GitHub (switch to the `big-update` branch first), or `git pull` and `git switch big-update`.
2. Open **`test.html`** in Chrome by double-clicking it.
3. The test version starts with **$999,999 and every vehicle unlocked**. It saves separately, so it won't touch real progress.
4. `index.html` is the real version: normal money, nothing unlocked.

Press **H** in game for the full controls.

## What to try

Tick each one and note anything broken, ugly or too hard or easy.

### Basics
- [ ] Game loads and the "Full screen?" pop-up works
- [ ] Drip outfit has no gold chain
- [ ] The city is bigger (14×14 blocks) and still runs smoothly. Note your FPS feel on PC and phone
- [ ] Cars parked and driving on the street are only basic ones (sedan, taxi, SUV, pickup)

### Doge Motors (blue **V** on the radar)
- [ ] Walk up to each vehicle's marker and press E. You get put in it on the road outside
- [ ] Super cars: Bolt GT, Phantom X, Thunder, Lowrider
- [ ] **Bulletproof** car: cops' bullets shouldn't hurt you inside it
- [ ] **Tank**: drives slowly, mouse turns the turret, click fires the cannon, rams and crushes cars
- [ ] **Helicopter**: Space goes up, Shift goes down, W/S fly, A/D turn. Try landing on a roof. You can't get out unless you're on the ground
- [ ] Shooting from the helicopter and bulletproof car works
- [ ] Taking out a vehicle you already own again replaces the old one

### Explosions
- [ ] Tank shells and the rocket launcher blow up cars
- [ ] Enough bullets make a car smoke, then explode
- [ ] Exploded cars turn black, burn, then disappear after about 40 seconds
- [ ] Explosions chain into nearby cars
- [ ] Being in a car when it blows up throws you out and hurts you

### Lucky Doge Casino (gold **♣** on the radar)
- [ ] 5 slot machines along the back wall, a roulette table and a blackjack table
- [ ] Slots: spin, win sometimes, but lose money over time
- [ ] Roulette: try Red, Black, Odd, Even, the 1–18 / 19–36 halves, the 3 dozens and one number
- [ ] Blackjack: Deal, Hit, Stand and Double. The dealer's second card stays hidden until you stand
- [ ] You can't bet more than you have
- [ ] Leaving the table puts you back in the game

### Robberies
- [ ] **ATMs** (small white dots on the radar): hold E for 3 seconds to get $60–200 and 1 wanted star. The ATM goes dark for 2 minutes
- [ ] **Diamond Dogs** jewellery store (cyan **◆** on the radar):
  - [ ] Press E at a glass case to smash it for $150. The alarm goes off
  - [ ] The two guards shoot you
  - [ ] You get wanted stars
  - [ ] The cases refill after 3 minutes if you're away from the store
- [ ] Shooting inside the store also sets off the alarm
- [ ] Both shops (Stick Up and Quik Cash missions) still work

### Bodyguards (orange **B** marker near the start)
- [ ] Hire for $250 each, up to 3
- [ ] They follow you, shoot cops (when you're wanted), gang members who attack you and jewellery guards
- [ ] They vanish into your car when you drive and reappear when you get out
- [ ] Explosions can kill them

### Money and saving
- [ ] Close the game and reopen it: money, outfit, gun, passed missions and bought vehicles are still there (use `index.html` for this, not the test version)
- [ ] Dying costs a flat **$100** hospital bill, or whatever you have if it's less
- [ ] Prices feel fair. The goal is that nothing takes more than about 10 minutes of play to afford:
  - Lowrider $400, Thunder $500, Bolt GT $600, Phantom X $1,200
  - Bulletproof $1,500, Helicopter $2,500, Tank $3,000
  - Bodyguard $250

### Phone / Telegram
- [ ] On a phone, the CAR button works for buying, the casino, ATMs (hold it) and smashing cases
- [ ] In the helicopter, the RLD and PUNCH buttons turn into UP and DOWN

## When it's all good

Merge `big-update` into `main`. GitHub Pages updates the live site and the Telegram game within about a minute.

Don't merge `test.html` into the live site. Delete it before merging, or it will give everyone free money at `/coin-city/test.html`.
