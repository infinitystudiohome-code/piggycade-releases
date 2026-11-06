# Qurio — NEW task list · 6 November 2026

This is the new active batch, separate from completed1.0.63 work. Every new request is added here before implementation. Checked means implemented and verified, not necessarily published. Published1.0.63/code64; working1.0.64/code65. Artwork consistency, saved progress and persistent rooms remain mandatory. No PC sleep/shutdown.

## 1. Pool blocked turn — supplied screenshot/report FIRST
- [x] Identify exact blocker: Illegal break requires a choice; Focus hides the choice buttons. Report shows no canvas fault, no busy wait and no room connection. Source and screenshot agree.
- [x] Keep every required decision visible/actionable with controls hidden, without forcing optional controls open.
- [x] Verify illegalbreak and8-on-break choices, solo/host/guest/spectator,375×747 andlandscape; retain current game/score.
- [x] Expand diagnostics to distinguish mandatory decision, cue-ball placement, turn and graphics wait from a freeze.

## 2. NPC art consistency — entire roster
- [x] Audit all NPC portraits together against the approved chibi roster: proportions, shading, outline, optical size and transparent edges.
- [x] Lady Gaga: approved chibi style, supplied blonde bow/sunglasses/outfit reference.
- [x] Miles Morales: approved chibi style, unmasked in Spider-Man suit.
- [x] Paris Hilton: approved chibi style, pink outfit/sunglasses/dog reference.
- [x] Zendaya: approved chibi style,2015AcademyAwards white dress/dreadlocks reference.
- [x] Zara Larsson: approved chibi style, preserve intended outfit/look.
- [x] Terry Crews: approved chibi style, shirtless/muscular.
- [x] Eren Yeager: approved chibi style, recognizable look and appropriate expression.
- [x] Bono: SouthPark-inspired look adapted to shared chibi style, sunglasses/cowboyhat/black-red leather/openchest.
- [x] Correct any other inconsistent NPC, compare beside approved roster, ensure no clipped bodies/neighbours and equal optical scale.
- [x] Audit correction: PewDiePie chibi consistency.
- [x] Audit correction: Michael Jordan chibi consistency.
- [x] Audit correction: Nicki Minaj chibi proportions, retain pinkhair/referenceoutfit.
- [x] Audit correction: Tobey Maguire chibi consistency.
- [x] Audit correction: Willy Wonka chibi consistency.
- [x] Audit correction: Oompa Loompa chibi consistency.
- [x] Audit correction: Jesus chibi consistency.

## 3. UNO presentation and interactive house rules
- [x] Make hand cards bigger, touchable and readable on narrow phones/landscape without hiding actions.
- [x] Place human and computer players around the table in multiplayer; preserve circular order and clear centre piles.
- [x] Flip: show both card sides where allowed by the mode, keeping opponents' hidden hands private.
- [x] Flip: bold FLIP card back/label and a prominent centre button so each player manually flips their hand when triggered.
- [x] Slap: last human or bot to slap gets the configured penalty; verify timing/ties/disconnect behavior.
- [x] Exchange: visible clockwise prompt/arrows and manual drag-to-next-player hand transfer; synchronize all clients before play continues.
- [x] Keep existing quick shuffle/individual deal, turn locks, all variants and private information correct; test solo/live/rejoin/reduced-motion.

## 4. Solitaire
- [x] Make Shuffle a little bigger with comfortable touch target.
- [x] Make stock pile bigger and centered.
- [x] Add a right-handed Draw button under Shuffle, acting on the stock.
- [x] Hints show useful legal moves with clear source/destination/explanation; avoid pointless cycles.
- [x] Shuffle randomizes remaining cards and automatically reveals next hand; avoid showing identical order again where alternatives exist; no added moves/points.
- [x] Add faint circus details to card backs while keeping them calm and readable.
- [x] Stop forced instant auto-finish; let player complete the foundation stacks manually, with an optional explicit finish action if appropriate.
- [x] Verify drag/drop/top-waste/undo/manualfinish and all five difficulties; buttons fit phones/landscape.

## 5. Texas Hold’em
- [x] After losing/new game, place New opponents and Deal again controls at the bottom; keep table, profile/chips and multiplayer room behavior.
- [x] Verify both choices work and preserve appropriate chips/history; no overlay blocking table.

## 6. Blackjack
- [x] Put Deal and New opponent buttons at the bottom.
- [x] Make table and cards bigger responsively.
- [x] Keep Hit/Stand/Double at the bottom but lifted above the phone edge; all split/double/stand controls remain reachable.
- [x] Verify solo and hosted actions, payouts and persistent-table behavior at narrow/tall/landscape sizes.

## 7. Roulette
- [x] Make wheel bigger responsively.
- [x] Make player/NPC characters bigger in hosted and computer games while preserving shared avatar scale/style.
- [x] Verify betting buttons, wheel, announcements and bubbles do not overlap or clip.

## 8. Bartender
- [x] Reproduce/recheck real launcher→bar load on bundled assets; handle any loading error with a useful message/retry instead of indefinite loading.
- [x] Verify start/mix/serve and native background/return; preserve saved bar progress and local audio.

- [x] Bartender guests arrive automatically and clearly demand/request drinks, with varied personality and reactions.
- [x] Show an illustrated finished-drink target; default order does not reveal the ingredient/mixing solution, player figures it out.
- [x] Expand drink recipes and ingredient variety with useful interactions; keep recipe data, appearance and scoring consistent.
- [x] Verify the full customer→visualtarget→mix→serve→reaction loop on phone, offline and live highscore mode; no loading deadend.

## 9. Pinball
- [x] Use stronger appropriate bell/ding/metal contact samples, with volume/mute and no clipping.
- [x] Add bounded central-machine effects/flickering lights and ramp-hit lights.
- [x] Make cabinet bigger while controls remain reachable on all screens.
- [x] Add coherent bounce/slide obstacles; every visible solid element matches collision geometry and no new traps.
- [x] Verify digital-style scoreboard readability and score/ball state.
- [x] Recheck freezing/recovery, spring pull/release sound, open drains, all difficulties, explicit pause/background and saved relaunch.

## 10. 8-Ball Pool controls/rules/layout
- [x] Make cue manipulation directly on the stick easier, without accidental shots during aiming.
- [x] Make cue-ball pickup/placement easier.
- [x] Allow continuous white-ball pickup/repositioning during ball-in-hand until pulling/taking the shot; small lifting-hand indicator/animation, cancelled drag/pull handled; no illegal normal-turn pickup.
- [ ] Ask handedness before starting; place power rail accordingly and remember choice.
- [ ] Verify wrong first contact gives opponent ball-in-hand anywhere legal; both groups and actual hosted play.
- [ ] Make table/cue/balls bigger responsively while retaining visible required controls.
- [ ] Verify freezes, required decisions, touch, background/return and two-client shot/aim behavior.

- [ ] Review supplied MiniclipGIF https://support.miniclip.com/hc/article_attachments/41975201180817 for smooth placement/ball motion; improve ball rendering/motion without changing legal physics.

## 11. Checkers audio/immersion
- [x] Distinct move swoosh and landing sound.
- [x] Capture sound for a regular piece.
- [x] Promotion-to-King sound.
- [x] Distinct King capture and multi-capture cues.
- [x] Verify optional/backward captures, flying kings and chains remain unchanged; no duplicate/shared sound spam.

## 12. Snakes & Ladders
- [x] Physical swipe/throw dice gesture across board with strong/weak visual throw while outcome remains fair.
- [x] Enlarge settled dice result so everyone sees the number.
- [x] Tile-by-tile hopping sounds and transient tile glow.
- [x] Manual placement ends with the character correctly on the destination tile.
- [x] Make board longer/larger with larger tiles/snakes/ladders and larger character pieces, responsive on phones.
- [x] Verify roll completes before movement, manual/live synchronization and exact-roll finish.

## 13. Hangman, Sudoku and app foreground — latest additions
- [x] Hangman correct word: grand recorded victory cue, confetti/fireworks/sparkles, then advance only after celebration; live players stay synchronized.
- [x] Hangman wrong letter: wrong/buzz effect plus supported-phone haptic vibration, honoring mute/haptic settings and no repeats for an already-tried letter.
- [x] Sudoku: larger board/tiles responsively, controls/notes still reachable.
- [x] Sudoku: small sun/moon Light/Dark switch with white/dark board, per-player saved preference, no puzzle reset.
- [x] Sudoku: unique completed row/column sound and bounded flicker/highlight once per newly completed line.
- [x] Sudoku: wrong-number buzz sound and clear feedback without exposing correct answers.
- [ ] All games: brief app-background/return resumes state and buttons smoothly; test solo/live and respect explicit pause/finished state without lag or screen freeze.
- [ ] Snakes: use supplied lush jungle/adventure reference (temple/treasure/waterfalls/vines/animals, winding stone path), keep Qurio name/consistent illustration, correct1–100 playable numbering and matching snakes/ladders.

## 14. Ultimate Tic-Tac-Toe — latest addition
- [x] Enlarge board and use available bottom space on narrow/tall phones; preserve large touch targets and landscape/desktop fit.
- [x] Add recorded free-library placement/action/won-box sounds, respect mute and avoid replay sounds on reconnect.
- [x] Preserve pink heart/purple X, orange/green turns, dice mini-game, rankings and current rules; verify real touch input and screenshots.

- [x] Hide controls expands UTTT board further into the available height; verify larger than shown-controls state.
- [x] Heart and X use clearly distinct recorded placement effects; conquered box separate from whole-match result.

## 15. Sound effects priority — latest request
- [x] Source engaging recorded effects from free online libraries; keep license/source records, compress carefully and balance volume without clipping.
- [x] Distinct victory and defeat cues for each player according to their result; appropriate draw/shared-win behavior, no wrong winner cue or reconnect replay.
- [x] UTTT conquered small box has a distinct satisfying cue; separate from placement and whole-match victory.
- [x] Audit requested games for meaningful action/interaction/finish audio; avoid generic repetitive placeholder sounds. Respect effects volume/mute, background, reduced effects and phone performance.

## 16. Performance stars — latest request
- [x] Stars measure performance independently of winning; a strong losing player can earn half/full stars, especially UTTT.
- [x] Record game-appropriate performance metrics for both players; explain the percentage, keep actual win/loss and points separate, preserve previous records.
- [x] Verify good losing performance earns stars, poor play differs, draws/empty data handled honestly, no fabricated mistakes or speed targets.

## 17. Bluetooth-only nearby hosting — latest request
- [x] Add an optional Bluetooth-only checkbox to Host; no internet, Wi-Fi router or Wi-Fi transport required. Preserve existing online Host/Join.
- [x] Search nearby devices, show paired devices, pair/select/join with clear connection status and permission guidance.
- [x] Host phone runs authoritative room/game rules locally; synchronize actions/private views over Bluetooth, retain all existing game modes and game privacy.
- [x] Handle permission denial, Bluetooth disabled, cancellation, disconnected/reconnecting peer and host departure without stuck screens or resetting unrelated games.
- [x] Preserve saves/rankings and defer server sync until internet returns; no lost/duplicate results.
- [ ] Verify protocol/host authorization/version compatibility and actual Android two-phone pairing/play/resume; clearly distinguish simulated checks from real-device validation.

## 18. Six new card/party games — NEW queued batch
These new additions arrived during1.0.64 final release checks. Keep that verified update moving; implement these one by one in the following isolated game batch, preserving the current work.
- [ ] Bullsh*t!: research mobile examples/official rules; face-down claims, bluff challenge, liar/false-accuser pile pickup, legal round completion, avatars/live/Bluetooth/solo where appropriate, recorded sounds and animated cards.
- [ ] Rummy: research mobile examples/rules and clearly document chosen variant; valid sets/runs, draw/discard/meld, round scoring/end, avatars/live/Bluetooth, recorded sounds and animated cards.
- [ ] Old Maid: research mobile examples/rules; matching pairs, manual draw from next player, single unmatched card/last-player loss, avatars/live/Bluetooth/solo, recorded sounds and animated cards.
- [ ] Cockroach Poker: research mobile examples/official rules; animal claims, pass/reveal/accept/challenge, correct failed-claim pile assignment and defeat rule, themed artwork, avatars/live/Bluetooth, recorded sounds and animations.
- [ ] Cards Against Humanity-style party game: research mobile examples/rules; original prompt/answer decks, anonymous submissions, rotating human judge, points/rounds, avatars/live/Bluetooth, animated reveals and recorded sounds.
- [ ] What Do You Meme?-style caption game: research mobile examples/rules; original image/caption content, hidden submissions/rotating human judge/points, avatars/live/Bluetooth, image/caption reveal effects and recorded sounds.
- [ ] Search existing free licensed downloadable audio/asset libraries first for all six; retain sources/licenses, balanced/compressed recordings and sound menu/mute.
- [ ] Apply shared responsive controls, no duplicated NPCs, profile/ranking/save persistence, clear turn guidance, celebrations and background/rejoin protections; real rule/input/multiplayer tests and screenshots per game.

## 19. Shared sound sourcing, checks and release
- [ ] Add cohesive bounded motion: subtle floating/idle elements, arrival/serve/pour effects, responsive feedback bubbles and transitions. Keep aiming/dragging stable, pause hidden motion, honor reduced-motion and verify phone performance.
- [x] Prefer downloaded free licensed sound libraries; record sources/licenses, compress recordings, balance volumes and preserve mute controls.
- [x] Use localAI for bounded assistance, verify its suggestions and monitor resources; do not unpause unrelated Infinity master work.
- [x] Test and screenshot changed layouts and real input paths, narrow/tall/landscape/tablet/desktop; no unnecessary unrelated redesign.
- [x] Preserve existing rooms/saves/chips/profiles/rankings and old snapshot compatibility. Version any new multiplayer rule state; no room resets.
- [ ] Pass mandatory launcher/update-recovery gate, sign with existing appID/key, publish and verify the in-app updater/download hash.
- [ ] Publish final source backup and deliver APK link/PC path; mark published only after verification.

## Verification evidence
- Avatar audit:113 rendered portraits,148±2 optical size/clear alpha; all15 replacements installed, mainfour retained.
- Casino: bundled fiveviewport layouts plus two-client Hit/Stand/Fold/replay/next/newopponents/roulettebets; persistent rooms/tokens/chips; all pass.
- UTTT: fiveviewport fit/81targets, real local/live placements and recorded sounds/dedup/mute; existing colors/rules/saves retained.
- Pool placement: backend legality/snapshot/repeatedplacement/cancelledinvalidshot/validshotlock; actual touch and drag glove preview/commit/cancel, foreground, no scriptfaults pass.

- Bundled UNO interaction/layout checks now pass all variants at portrait/landscape/tablet after fixing7px clipped actions in phone landscape.
- Bartender complete customer/target/mix/serve loop,48recipes/36ingredients, retries/legacy saves/nativepause pass against bundled assets.
- Solitaire manualfinish/rightDraw/centredstock/usefulhints and500shuffles/52cards/no addedpoints tests pass.
- Hangman/Sudoku realinput/theme/feedback/resume/snapshot tests pass; no physicalCamon test claimed.

- Final mandatory gate:50/50 checks +197backendtests +actualHost/Update/broken-launcher recovery PASS. Report delivery/newbatch-164-gate-report.json.
- Backend deployed adb982a2-d057-4acd-8c47-cfb8f66f6599; actualpre/postdeployment Sudoku board/notes/start/player-sessions retained. No room reset.
- Bluetooth no-internet two-client Host/Search/Pair/Join/ready/UTTT/foreground UI and33authoritycases/nativecompile/framing pass. Realphonepairing stillrequiresdevicevalidation.
- Nextsixgames researched withofficialrules/mobileviews; firstthreepureengines pass15stagingtests. Newstagingwork stays onF: outside1.0.64 release. LocalGPUcaptiondraft reviewed/revised; invalidlocalrulesadvice rejected.

## Current next actions
1. ACTIVE:1.0.64 full50-step release gate PASSED; signedAPKbuild is nowrunning (buildscript repeats mandatorychecks), then source/updater publication. Pool, Solitaire, UNO, Bartender, casino layouts, all15chibi replacements, Pinball, Snakes, Hangman/Sudoku, UTTT and player-specific recorded outcomes have targeted passing evidence. Bluetooth nativecompile/framing/33authoritycases and actualtwo-clientHostUI pass; physicalphonepairing remains untested.
2. Every new request goes into this NEW list; previous work remains in Qurio-task-list.md. Public APK is still1.0.63 until this batch is checked and published.
3. LocalAI provides advisory checks only; implementation and screenshots are verified. All avatars must match the same approved chibi style.
