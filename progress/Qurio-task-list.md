# Qurio — NEW Game Update Suite · 6 November 2026

Status: ACTIVE, unpublished 1.0.71 workspace. Published stable: 1.0.70. Checkboxes mean implemented AND verified, not a promise. Games are handled in the exact requested order. A current game must pass before the next starts. Existing rooms and saved scores are protected.

## Global Cross-Game Requirements
- [x] Character Correction Fix: Fix Phoebe Buffay currently showing Rapunzel / Sabrina Carpenter. Correct her asset and sprite to actual Phoebe Buffay in the established chibi style.
- [x] Play Again Feature: All games. Keep human players; NPC opponents may randomize. Verify the existing 1.0.70 implementation for this suite.
- [x] Menu Player Management: Main-menu options to configure/add multiple human players and computer opponents.
- [x] Global Audio Standard: All games have audio; source free SFX libraries including Mixkit and keep licensing/provenance.
- [x] Global Art & Character Standard: Consistent chibi artwork, complete silhouettes and equal scale; regenerate mismatched assets and verify visually.

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
- [x] Allow players to look at their hand first and shuffle manually before the other person picks, then allow card removal.
- [x] Add more sound effects.
- [x] Make the game occupy the whole screen as much as possible without covering the active buttons and menu.
- [x] Allow players to clearly see the cards they picked.
- [x] Disable automatic matching; players must manually pair cards.
- [x] Improve the shuffling animation so players can visually see the other player shuffling their cards.
- [x] Increase the overall size of the cards.

### 4. Rummy
- [x] Make the cards bigger.
- [x] Make the table layout bigger.
- [x] Implement a real-life hand-holding and arrangement mechanic (fan mechanic): players must be able to lift cards and squeeze them in between wherever they want in their hand.
- [x] Allow players to add cards onto the melded pile.

### 5. Bartender
- [x] Add sound effects.
- [x] Improve text readability/rendering (make words appear better).
- [x] Add tropical bar background music.
- [x] For multiplayer, implement a split-screen view so players can see each other, with both serving at the same time at the beginning.
- [x] Add gibberish chatting background sounds.

### 6. Pacman
- [x] Make the on-screen control buttons bigger and fit them neatly to the left and right sides.
- [x] Make the arcade cabinet screen viewport bigger.

### 7. Pinball
- [x] Remove any placeholder/copy-paste text.
- [x] Add more obstacles to bounce and slide on.
- [x] Add more flickering lights in the middle of the board (currently too concentrated on the sides).
- [x] Properly position the buttons for the left and right thumbs, and place the nudge and "pull/launch" controls at the bottom.
- [x] Make the arcade view bigger.

### 8. 8-Ball Pool
- [x] Add an option for left-handed or right-handed players before the game starts, moving the cue/lever accordingly.
- [x] Stretch the aiming guideline much further out.
- [x] Announce who won after the game with clear "YOU WIN" and "YOU LOSE" screens.

### 9. Checkers
- [x] Add a mirrored board/camera version for the second player so it is fair and nobody has to play upside down.

### 10. Snakes and Ladders
- [x] Fix the exact winning tile rule: When near the end and a roll exceeds tile 100, the player must bounce backward. (Example: If on tile 99 needing 1 to win, and you roll a 3, you count forward 1 to 100, then bounce backward 2 steps, landing on tile 98). You can only win on tile 100 with an exact count.

### 11. Solitaire
- [x] Reduce card size slightly (they don't need to be overly massive).
- [x] Upscale all card graphics to fix low-quality/blurry rendering.
- [x] Add sound effects when shuffling cards.
- [x] Add sound effects when placing cards down.
- [x] Add sound effects for win/loss states.
- [x] Add a buzzer/error sound effect when placing a card on the wrong pile.

### 12. Roulette
- [x] Eliminate the need to scroll to look at the wheel.
- [x] Move the dealer directly beside the wheel.
- [x] Position players surrounding the wheel in multiplayer, or side-by-side in 2-player mode.
- [x] Add spinning wheel sound effects.
- [x] Add celebratory confetti and sound effects when someone wins.
- [x] Add sound effects when someone loses.
- [x] Add rolling ball sound effects.
- [x] Add coin/chip placement sound effects.

### 13. Uno
- [x] In "Uno Flip" game mode, all players must be able to see both the top and back of the cards like in real life (seeing the flip side, and seeing the normal side when flipped).

### 14. Blackjack
- [x] Make the table slightly longer to provide each player proper spacing, but optimize layout to prevent vertical scrolling.

### 15. Extreme Tic-Tac-Toe
- [x] Return the board to its normal aspect ratio (it is currently stretched too much).
- [x] Change tiles from rectangular to square with rounded corners.

### 16. Sudoku
- [x] Change the incorrect-entry sound effect to a distinct buzzer and add a screen shake effect.
- [x] Implement two distinct game modes:
  - Mode1: Standard single-player puzzle.
  - Mode2: Competitive PvP mode where players try to solve the exact same puzzle simultaneously against each other.

### 17. Wordle
- [x] Allow players to intentionally input incorrect/dummy letters on purpose to test and find letter placements.
- [x] Add mechanical typewriter sound effects when typing letters.

## Current next actions
1. ACTIVE: Signed APK built and scanned; publishing and verifying public updater/download. Games1–17 staged and verified; not published yet.
2. Globals remain tracked above and are verified without changing the queue order.
3. Infinity AI advisory requested; bridge refuses inference while MASTER-PAUSE protects its active workload. No bypass performed. Codex continues.

## Evidence
- Stable1.0.70 remains published. New workspace: .qurio-release-1.0.71. No new APK published for this suite yet.
- No physical phones attached: desktop/mobile viewport evidence is separate from actual phone acceptance.

- Game1: 24 focused backend tests including200 restored sessions, both actual touch judging flows, 12 responsive views, one-word10-seat deals,80 anonymous-entry shuffles, music decode/30%/mute/background checks and11 root navigation paths pass. See .qurio-release-1.0.71/FamilyQuest/delivery and tools/screenshots/suite171-*.png.

- Game2: new backend starts rejected atomically; solo/menu/host registrations and bundled presentation assets absent. Private compatibility for already-running old rooms retained; no room reset.

- Game3: manual51-card deals, explicit pairing/ready/owner offer/private picked-card reveal; complete2–10seat simulations with JSON restore and conservation; actual two-client touches and5responsive screenshots pass. Owner shuffle animates on the opponent phone; speech bubble moved above controls. Legacy snapshots retain their original rules.

- Game4: real CDP finger lift/reinsert, persistent private hand arrangement, drag onto an opponent run, exact physical-card conservation and5responsive views/screenshots pass. Existing Rummy meld/layoff/rules tests pass.

- Game5: live bounded station snapshots show real opponent ingredients/orders, both simultaneous shifts, decoded tropical/pour/chatter audio, score/finish/pause/replay and actual375px full service loop pass. Inputs validated before authority mutation. New media compressed; credits included.

- Game6: larger58–66px actual thumb targets split left/right, no maze/control overlap across5viewports. Real maze movement,15audio tracks, scoring/results/pause/room replay and persisted records pass.

- Game7:18physics tests pass including new spinner/guide contact, old saves, drains and stuck spots. Five actual layouts,150% spring pull/recorded spring cleanup, bumper/ramp scoring, pause/resume pass. Centre lamps animate with reduced-motion support; thumb controls separated; decorative centre copy removed.

- Game8: two-phone first-time hand choices, persistent opposite power sides, rendered guideline pixels beyond old360px limit and YOU WIN/YOU LOSE pass. Existing pool presentation/audio/required decisions/live opponent aim/real shot/turn notification checks pass.

- Game9: each client sees its own army at the bottom; actual taps from opposite orientations submit correct world-coordinate moves for both turns. Existing relaxed checkers ending/surrender tests retained.

- Game10: all36 near-finish from94–99 / die1–6 combinations, exact manual finish,100-crossing not a win, bounce then snake and JSON snapshot paths pass. Ten actual two-client cases cover all difficulties and retained Checkers touch rules. Old active snapshots retain their previous finish rule.

- Game11: complete52-card1846x852 restored atlas (142x213px/card), same circus design; slightly smaller cards. Actual shuffle/placement/abandoned-deal/win sample starts and invalid local/remote buzzer pass. Rules, top-waste/manual drag, shuffle/no-move cost, Undo, optional Finish and5responsive layouts pass. Landscape sidebar overflow found and corrected.

- Game12:10layouts cover2/4players, pinned wheel under betting scroll, beside dealer, side-by-side2P and ring4P, full avatars/controls. Actual wheel/ball clip pause/resume and winning confetti pass; authority payout/ready/lock/persistence/two-client replay pass.

- Game13: all outward Flip faces visible while current playable hands stay private; pending manual-turn exposure and light/dark restore pass. Three actual client flips, clockwise drag exchanges, reduced motion and2–10seat opening deals pass.

- Game14: longer580px felt, responsive opponent widths prevent narrow-phone overlap;10 actual four-player viewport/focus checks pass without vertical scrolling,39 card-rule/Blackjack tests pass.

- Game15: square board and81 rounded square touch tiles at5 viewport sizes; recorded heart/X sounds, accepted live moves/no duplicate sounds, save/resume, themes, focus expansion and7 dice rules pass.

- Game16: separate Standard/PvP labels and default competitive host choice; distinct recorded buzzer and brief shake/deduped mistakes. Two actual independent client boards use the same puzzle, first finish stops both;13 Sudoku rules plus theme/notes/resume checks pass.

- Game17: made-up/exploratory guesses accepted at all5 difficulty levels with five-letter validation, duplicate rejection and correct scoring; hard-mode clues no longer forbid experiments. Recorded CC0 mechanical typewriter sample actually decodes/plays for10 keystrokes and respects mute. Touch flash, duplicate clues,4 responsive sizes and online no-repeat feedback pass.

- Global replay: actual two-root UNO/Wordle/Checkers final recaps, guest requests/host approvals, same group, UNO scores/rules, both scoreboard routes, separate lobby and offline replay pass. Phoebe replaced with bohemian singer portrait and refined head scale after gallery comparison.

- Globals: main-menu saved two-human pass-phone profiles and selected computer seats verified in real new games; separate-phone humans retain Host/Join. All113 portraits rendered at148±2 optical extent with full alpha margins; reviewed all4 gallery sheets, Phoebe proportion correction accepted. Downloaded casino/board/outcome samples and new per-game audio checks pass, credits and compressed sources retained.

- Final integrated gate:40/40 checks pass plus mandatory actual Host/Update/broken-launcher recovery;265 backend tests;695 source/bundle comparisons and616 unchanged runtime/backend/native files. Backend1dbef243-9318-451e-b242-60916e46c2a7 deployed with a live Sudoku room preserving board, notes, start time, scores and player IDs; partner move accepted afterwards. Signed APK1.0.71/code72 built:70,300,667bytes,613 bundled files verified, stable appID/certificate retained. APK and full private source Defender scans found no threats. Publication and public-download verification in progress.
