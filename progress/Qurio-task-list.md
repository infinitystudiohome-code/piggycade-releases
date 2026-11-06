# Qurio — NEW task list · 6 November 2026

This is the new active batch, separate from completed1.0.63 work. Every new request is added here before implementation. Checked means implemented and verified, not necessarily published. Published1.0.64/code65; working1.0.65/code66. Artwork consistency, saved progress and persistent rooms remain mandatory. No PC sleep/shutdown.

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
- [x] Ask handedness before starting; place power rail accordingly and remember choice.
- [x] Verify wrong first contact gives opponent ball-in-hand anywhere legal; both groups and actual hosted play.
- [x] Make table/cue/balls bigger responsively while retaining visible required controls.
- [x] Software verification: freezes/required decisions/touch/background-return/two-client shot and aim pass against exact1.0.66 bundle; realCamonphone feedback remains separate.

- [x] Review supplied MiniclipGIF https://support.miniclip.com/hc/article_attachments/41975201180817 for smooth placement/ball motion; improve ball rendering/motion without changing legal physics.

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
- [x] Software checks across every game loader: background/return preserves state and working inputs, including delayed startup, active timers/canvas and explicit pauses. Physical phone validation remains listed below.
- [x] Snakes: use supplied lush jungle/adventure reference (temple/treasure/waterfalls/vines/animals, winding stone path), keep Qurio name/consistent illustration, correct1–100 playable numbering and matching snakes/ladders.

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
- [x] Preserve Bluetooth match records, local rankings/profiles and existing cloud-room session separately across updates; no lost/duplicate local results.
- [ ] Automatic upload of Bluetooth/solo results after internet returns remains part of the previously deferred live-rankings release; queued local records are preserved.
- [x] Validate Bluetooth protocol, host authorization and version compatibility with native compilation, framing and simulated two-client tests.
- [ ] Validate actual Android two-phone Bluetooth pairing, play and reconnect; simulated links do not establish radio compatibility.
- [ ] Confirm gameplay and background/resume on the partner’s Camon 30 Pro after installing the update.

## 18. Six new card/party games — PUBLISHED1.0.65
These new additions arrived during1.0.64 final release checks. Keep that verified update moving; implement these one by one in the following isolated game batch, preserving the current work.
- [x] Bullsh*t!: research mobile examples/official rules; face-down claims, bluff challenge, liar/false-accuser pile pickup, legal round completion, avatars/live/Bluetooth/solo where appropriate, recorded sounds and animated cards.
- [x] Rummy: research mobile examples/rules and clearly document chosen variant; valid sets/runs, draw/discard/meld, round scoring/end, avatars/live/Bluetooth, recorded sounds and animated cards.
- [x] Old Maid: research mobile examples/rules; matching pairs, manual draw from next player, single unmatched card/last-player loss, avatars/live/Bluetooth/solo, recorded sounds and animated cards.
- [x] Cockroach Poker: research mobile examples/official rules; animal claims, pass/reveal/accept/challenge, correct failed-claim pile assignment and defeat rule, themed artwork, avatars/live/Bluetooth, recorded sounds and animations.
- [x] Cards Against Humanity-style party game: research mobile examples/rules; original prompt/answer decks, anonymous submissions, rotating human judge, points/rounds, avatars/live/Bluetooth, animated reveals and recorded sounds.
- [x] What Do You Meme?-style caption game: research mobile examples/rules; original image/caption content, hidden submissions/rotating human judge/points, avatars/live/Bluetooth, image/caption reveal effects and recorded sounds.
- [x] Search existing free licensed downloadable audio/asset libraries first for all six; retain sources/licenses, balanced/compressed recordings and sound menu/mute.
- [x] Apply shared responsive controls, no duplicated NPCs, profile/ranking/save persistence, clear turn guidance, celebrations and background/rejoin protections; real rule/input/multiplayer tests and screenshots per game.

### 1.0.65 implementation milestones — staged, not yet published
- [x] Research all six rules/mobile examples; retain official sources and choose explicit variants.
- [x] Implement all six authoritative engines/private views;237combined backend/rule checks pass.
- [x] Create original24scene/8critter artwork; inspect framing and32atlasregions.
- [x] Integrate firstthree touch interfaces and actualbundled offline/privateclient tests.
- [x] Finish fullHost-flow and otherthree bundled renderer tests; fix discovered Rummy leave crash/background loading race.
- [x] Pass1.0.65 release gate, verify live-room continuity, sign/publish and verify updater/APK.

## 19. Shared sound sourcing, checks and release
- [x] Add bounded idle/arrival/pour/bubble/card effects; preserve aiming and dragging, pause hidden motion and respect reduced-motion. Browser/phone-layout checks pass; real-phone performance validation remains below.
- [x] Prefer downloaded free licensed sound libraries; record sources/licenses, compress recordings, balance volumes and preserve mute controls.
- [x] Use localAI for bounded assistance, verify its suggestions and monitor resources; do not unpause unrelated Infinity master work.
- [x] Test and screenshot changed layouts and real input paths, narrow/tall/landscape/tablet/desktop; no unnecessary unrelated redesign.
- [x] Preserve existing rooms/saves/chips/profiles/rankings and old snapshot compatibility. Version any new multiplayer rule state; no room resets.
- [x] Pass mandatory launcher/update-recovery gate, sign with existing appID/key, publish and verify the in-app updater/download hash.
- [x] Publish final source backup and deliver APK link/PC path; mark published only after verification.

## Published1.0.64
- Download: https://github.com/infinitystudiohome-code/piggycade-releases/releases/download/v1.0.64/Qurio.apk
- SHA256:9fe3d0b0168e786cc70fa4c2ac4841a506ff5f84ff82429c50237abc5e6c515d;59167237bytes; appID/key unchanged.
- Both updater feeds, publicredownload, private source backup andpublicGPLsource verified. Native64-bitDefender found no threats.

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
1. ACTIVE: 1.0.69 disables accidental long-press selection/copy menus on game UI while preserving editable fields, copy buttons and gameplay gestures. Testing all game documents before release.
2. Every new request goes into this NEW list; previous work remains in Qurio-task-list.md. Public APK is 1.0.67/code68. Six new games, Pool/room recovery, the Snakes reference presentation and shared background/resume fixes are shipped.
3. LocalAI provides advisory checks only; implementation and screenshots are verified. All avatars must match the same approved chibi style.

- 1.0.65 staging evidence: six-mode private authoritative room wrappers, versioned actions/deadlines/replays;237backendtests pass. Simulated-native Bluetooth sixmode adapters pass. Bundledfirstthree actualtouch inputs,18viewport layouts,15difficulty setups, privateclients/replay/winloss/saves pass. 1.0.65 published and verified.

## Published1.0.65
- Sixnewgames shipped. Download https://github.com/infinitystudiohome-code/piggycade-releases/releases/download/v1.0.65/Qurio.apk
- SHA256:0326d7b2708b7d880bf74fc83ad76ffebfa052b051938716045880ceee83a959;60540291bytes;actualstableappID/signingcertverified.
- 239backend/rulechecks;11changedgamegates+mandatoryHost/Update/brokenlauncher;662source/bundlecomparisons;589APKassetchecks;publicredownload/bothupdaters/GPLsource/privatesourcebackup;Defender no threats.
- ActualHTTP sixmode actions/privacy/pause/rejoin/freeplaynorankPASS. Bothbackenddeployments retainedactiveQA Sudoku board/notes/start/sessions.
- Poolremainingaudit: handedness/reload, bothsolids/stripeswrongfirstcontact, repeatlegalplacement/responsiveballradius15 and two-clientaim pass. Found freshhostpack usesrules4insteadof5; fix tracked below.

## 20. Pool and room recovery — published 1.0.66
- [x] Fresh hosted Pool uses the current rules, regardless of the previously opened game. Existing rooms keep their original rules.
- [x] Show the cue before initial placement; preserve the lifting hand, legal placement and shot locks.
- [x] Test fresh hosting, two-player inputs, Pool rules, placement, aim and resume. Verify unchanged games, sign, publish and verify the update.

- [x] FixfreshFXonlyroomswithmalformedmusic-offmetadata; normalizeolderpartialroommusicwithoutchangingboards/notes/chips/turns.244backendchecksandactualHTTPfivegamesPASS; deployed43efb1b4-e043-4185-8edb-50b42bf35a3cwithactiveSudokuroomcontinuityPASS.
- [x] Root/two-clientfreshPoolrules5/radius15/cuevisible/touchplacement/oneshot/requiredchoices; malformedlegacymusicwirestatedoesnotfreezeUI.

## 21. Snakes reference graphics — published 1.0.67
- [x] Draw a winding stone path with jungle gaps, keeping all 100 interactive squares and existing rules aligned.
- [x] Add larger patterned snakes with open mouths, fangs and tongues. Keep the approved illustrated jungle frame.
- [x] Fit the complete board and separate dice dock without covering bottom squares or wasting space. Test phone, tall and landscape layouts, touches, throws and hops.

- Snakesfunctional12casesPASSon1.0.65(all5levels,touchstrength,manualplacement,exactfinish,legacy/snapshot/rejoin/reducedmotion/background). Referencevisualgapremainsunchecked; lushframealreadyhasvines/temple/chest/waterfall/parrot/monkey.

## Published1.0.66
- Download https://github.com/infinitystudiohome-code/piggycade-releases/releases/download/v1.0.66/Qurio.apk
- SHA256:eaf2754b47f97783f18625eef87edde6baa6af634163597e58c539222080c6f9;60540907bytes;bothupdaterfeeds/publicredownload/privatesourcebackupverified.
- Existingroomprogressretained;noreset. Newcanonicalquietmusicstatefixesfreshroomloadingforfivearcadegames. TargetedPoolrules/cue/placement/shotchecksPASS;allothergameart/rulesretained.

## 22. Background and resume — published 1.0.67
- [x] If a game finishes loading while the app is hidden, keep its timer and animations suspended until the app returns.
- [x] Pause decorative animations in the background. Preserve explicit game pauses, saved state, rules and visible layouts.
- [x] Test each game loader, delayed solo/host loading, active canvas and timers, sound cleanup, real inputs after return and unchanged progress.

## 23. Final 1.0.67 delivery
- [x] Pass the final bundled release gate, preserve all other game source/room rules, sign and scan the APK, publish the update and verify the public download and both updater feeds.

- 1.0.67 staged evidence: 20 late-load/background/return cases across all game loaders; same game/board/seat IDs retained; explicit pauses and decorative CSS pauses preserved. Snakes: 600 tile checks across six viewports, all heads inside the frame, real roll/manual drag/ladder, four-player narrow layout and seven game-mode switches/restarts pass.

## Published 1.0.67
- Download: https://github.com/infinitystudiohome-code/piggycade-releases/releases/download/v1.0.67/Qurio.apk
- F: copy: F:/infinity/Qurio/releases/Qurio-1.0.67.apk
- SHA256: 2de9bd72bef4b8ab1983f88052bc16a4bbc90fc1972bed16e6e47dd6ea25237f; 60,545,023 bytes. Stable appID and signing certificate verified.
- Seven changed-game gates and mandatory Host/Update/broken-launcher recovery pass. Twenty lifecycle cases, 600 tile checks, six viewports and real touch/restart flows pass. All backend/native/other-game source remains unchanged from 1.0.66.
- Public redownload, both updater feeds, public GPL source and private complete-source checksum verified. Defender found no threats in the APK or source package; flagged Bartender reference payloads are excluded and blocked from future packaging.
- No backend deployment for this version. Existing rooms, rules, profiles, scores and saved game state are retained.

## 24. Room-preserving back button — published 1.0.68
- [x] Qurio Back / menu navigation returns the host and whole group to the lobby without leaving or disbanding. Same room code, players and host.
- [x] Only explicit Exit room leaves. Guests stay connected; preserve authority, scores and active rooms until the host explicitly returns to lobby.
- [x] Stop hidden game activity in the lobby, successfully start another game, test actual two-client buttons, sign/publish/verify the update.

- 1.0.68 evidence: 248 backend tests and actual two-root-client Pool/Poker header/Menu/Android Back flows pass. Same room/host/players/tokens; no leave or false win on Back. Cached Pool→Snakes startup and explicit Exit room pass.

## Published 1.0.68
- Download: https://github.com/infinitystudiohome-code/piggycade-releases/releases/download/v1.0.68/Qurio.apk
- Same room code, host, players and connections remain when the host uses Qurio Back, Menu → Return to lobby, or Android Back. Only Exit room leaves. Ready/start another game works; no false score/result on leaving the unfinished round.
- SHA256: 47c2394340c158c587f3700919dbe436c5f5b4cf546500ded7f736f89f7fffbb;60,545,087bytes. Stable appID/signing certificate verified.
- 248 backend tests, six focused gates, actual two-root-client controls, live HTTP transitions and 33 Bluetooth authority cases pass. Mandatory Host/Update/broken-launcher recovery, 590 APK asset checks, public redownload/both updater feeds/private source backup and clean APK/source Defender scans verified.
- Backend 5656215d-6154-4596-9ff3-cd1fdf9c73fb preserves the active test room’s Sudoku board/notes/start and both sessions. No automatic room reset.

## 25. Long-press game controls — 1.0.69
- [x] Disable accidental selection and native copy/paste callouts on game UI in every game document, including nested players.
- [x] Keep name/room-code/numeric fields editable and selectable, and preserve explicit clipboard/report controls.
- [ ] Verify real long holds, normal taps, Pinball hold/release, Solitaire dragging, dice swipes, Wordle keys and sliders; preserve lobby/group navigation, then sign/publish/verify the update.

- 1.0.69 staged evidence: all 13 actual bundled documents, real long holds/taps, editable fields and actual report Copy, numeric/range controls, Pinball hold/release, Solitaire drag, 3D dice swipe and Wordle key feedback pass. No backend changes.
