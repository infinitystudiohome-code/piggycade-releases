# Qurio — NEW Game Update Suite · 6 November 2026

Status: ACTIVE, unpublished 1.0.71 workspace. Published stable: 1.0.70. Checkboxes mean implemented AND verified, not a promise. Games are handled in the exact requested order. A current game must pass before the next starts. Existing rooms and saved scores are protected.

## Global Cross-Game Requirements
- [ ] Character Correction Fix: Fix Phoebe Buffay currently showing Rapunzel / Sabrina Carpenter. Correct her asset and sprite to actual Phoebe Buffay in the established chibi style.
- [ ] Play Again Feature: All games. Keep human players; NPC opponents may randomize. Verify the existing 1.0.70 implementation for this suite.
- [ ] Menu Player Management: Main-menu options to configure/add multiple human players and computer opponents.
- [ ] Global Audio Standard: All games have audio; source free SFX libraries including Mixkit and keep licensing/provenance.
- [ ] Global Art & Character Standard: Consistent chibi artwork, complete silhouettes and equal scale; regenerate mismatched assets and verify visually.

## Master Development Queue (Live Tracker)

### 1. Cards Against Humanity / "What do you meme" (Apply fixes to both)
- [x] Fix error in UNO game modes where players cannot go back.
- [x] Announce who wins clearly for both the judge and the players.
- [x] Shuffle the entries automatically so the judge does not know which player submitted which entry.
- [x] Include pop culture references, mixed with a healthy balance of explicit, satirical, and normal sentences.
- [x] Add silly background music and sound effects (SFX).
- [x] Include punchlines, innuendos, and dad jokes in the card pool.
- [x] Add a singular-word card mechanic/option.
- [x] Apply these exact fixes and changes to both Cards Against Humanity and What Do You Meme.

### 2. Cockroach Poker
- [x] Completely remove this game from the platform.

### 3. Old Maid
- [ ] Allow players to look at their hand first and shuffle manually before the other person picks, then allow card removal.
- [ ] Add more sound effects.
- [ ] Make the game occupy the whole screen as much as possible without covering the active buttons and menu.
- [ ] Allow players to clearly see the cards they picked.
- [ ] Disable automatic matching; players must manually pair cards.
- [ ] Improve the shuffling animation so players can visually see the other player shuffling their cards.
- [ ] Increase the overall size of the cards.

### 4. Rummy
- [ ] Make the cards bigger.
- [ ] Make the table layout bigger.
- [ ] Implement a real-life hand-holding and arrangement mechanic (fan mechanic): players must be able to lift cards and squeeze them in between wherever they want in their hand.
- [ ] Allow players to add cards onto the melded pile.

### 5. Bartender
- [ ] Add sound effects.
- [ ] Improve text readability/rendering (make words appear better).
- [ ] Add tropical bar background music.
- [ ] For multiplayer, implement a split-screen view so players can see each other, with both serving at the same time at the beginning.
- [ ] Add gibberish chatting background sounds.

### 6. Pacman
- [ ] Make the on-screen control buttons bigger and fit them neatly to the left and right sides.
- [ ] Make the arcade cabinet screen viewport bigger.

### 7. Pinball
- [ ] Remove any placeholder/copy-paste text.
- [ ] Add more obstacles to bounce and slide on.
- [ ] Add more flickering lights in the middle of the board (currently too concentrated on the sides).
- [ ] Properly position the buttons for the left and right thumbs, and place the nudge and "pull/launch" controls at the bottom.
- [ ] Make the arcade view bigger.

### 8. 8-Ball Pool
- [ ] Add an option for left-handed or right-handed players before the game starts, moving the cue/lever accordingly.
- [ ] Stretch the aiming guideline much further out.
- [ ] Announce who won after the game with clear "YOU WIN" and "YOU LOSE" screens.

### 9. Checkers
- [ ] Add a mirrored board/camera version for the second player so it is fair and nobody has to play upside down.

### 10. Snakes and Ladders
- [ ] Fix the exact winning tile rule: rolls exceeding tile100 bounce backward, e.g.99+3 lands98. Win only on100 with an exact count.

### 11. Solitaire
- [ ] Reduce card size slightly (they don't need to be overly massive).
- [ ] Upscale all card graphics to fix low-quality/blurry rendering.
- [ ] Add sound effects when shuffling cards.
- [ ] Add sound effects when placing cards down.
- [ ] Add sound effects for win/loss states.
- [ ] Add a buzzer/error sound effect when placing a card on the wrong pile.

### 12. Roulette
- [ ] Eliminate the need to scroll to look at the wheel.
- [ ] Move the dealer directly beside the wheel.
- [ ] Position players surrounding the wheel in multiplayer, or side-by-side in 2-player mode.
- [ ] Add spinning wheel sound effects.
- [ ] Add celebratory confetti and sound effects when someone wins.
- [ ] Add sound effects when someone loses.
- [ ] Add rolling ball sound effects.
- [ ] Add coin/chip placement sound effects.

### 13. Uno
- [ ] In "Uno Flip" game mode, all players must be able to see both the top and back of the cards like in real life (seeing the flip side, and seeing the normal side when flipped).

### 14. Blackjack
- [ ] Make the table slightly longer to provide each player proper spacing, but optimize layout to prevent vertical scrolling.

### 15. Extreme Tic-Tac-Toe
- [ ] Return the board to its normal aspect ratio (it is currently stretched too much).
- [ ] Change tiles from rectangular to square with rounded corners.

### 16. Sudoku
- [ ] Change the incorrect-entry sound effect to a distinct buzzer and add a screen shake effect.
- [ ] Implement two distinct game modes:
  - Mode1: Standard single-player puzzle.
  - Mode2: Competitive PvP mode where players try to solve the exact same puzzle simultaneously against each other.

### 17. Wordle
- [ ] Allow players to intentionally input incorrect/dummy letters on purpose to test and find letter placements.
- [ ] Add mechanical typewriter sound effects when typing letters.

## Current next actions
1. ACTIVE: Game3, Old Maid manual pairing/offer/shuffle and bigger cards. Games1–2 staged and verified; not published yet.
2. Globals remain tracked above and are verified without changing the queue order.
3. Infinity AI advisory requested; bridge refuses inference while MASTER-PAUSE protects its active workload. No bypass performed. Codex continues.

## Evidence
- Stable1.0.70 remains published. New workspace: .qurio-release-1.0.71. No new APK published for this suite yet.
- No physical phones attached: desktop/mobile viewport evidence is separate from actual phone acceptance.

- Game1: 24 focused backend tests including200 restored sessions, both actual touch judging flows, 12 responsive views, one-word10-seat deals,80 anonymous-entry shuffles, music decode/30%/mute/background checks and11 root navigation paths pass. See .qurio-release-1.0.71/FamilyQuest/delivery and tools/screenshots/suite171-*.png.

- Game2: new backend starts rejected atomically; solo/menu/host registrations and bundled presentation assets absent. Private compatibility for already-running old rooms retained; no room reset.
