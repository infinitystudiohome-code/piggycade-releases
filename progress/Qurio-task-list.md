# Qurio task list — 5 November 2026

Last updated: 6 November 2026 (continuing the 5 November task list). This is the master checklist for the requests visible in this conversation today, including Lexie's pasted messages. Add every new request here before implementing it. Work one feature at a time; retain earlier requirements when new messages arrive.

## Status and release discipline

- `[x]` means implemented and checked. This release is now published and its download/updater hash verified.
- `[ ]` means outstanding, partially implemented, or awaiting the stated verification.
- Published APK: **1.0.63 / versionCode 64** — https://github.com/infinitystudiohome-code/piggycade-releases/releases/download/v1.0.63/Qurio.apk
- Published source: `.qurio-release-1.0.63/FamilyQuest`. Previous 1.0.62 baseline retained.
- Keep the original `FamilyQuest` directory's unfinished feature work. Do not accidentally ship that whole tree; merge the requested features deliberately.
- Do not reset active rooms, scores, player sessions or saved games. Do not sleep or shut down this PC.

## 1. Solitaire

- [x] Red circus table; responsive phone/tablet/desktop layout; use available table space.
- [x] Circus-themed illustrated deck rather than a standard plain deck.
- [x] Inspect the deck against the complete requested cast: clowns, lions, doves, elephant, rat/mouse and ringmaster. Add any missing subject while preserving the approved artwork.
- [x] Stock/draw deck at the bottom, nearer the player.
- [x] Draw three cards; only the top waste card can be moved.
- [x] Shuffle the remaining stock/waste without disturbing tableau or foundations.
- [x] Shuffle adds no moves or points. Checked locally and against the live server.
- [x] Proper unbiased shuffle; every deal and reshuffle preserves 52 unique cards. 10,000-deal check exists.
- [x] Four Ace foundations centered at the top.
- [x] Manual card/stack movement and manual foundation placement.
- [x] Verify dragging a foundation card back to a legal tableau destination; distinguish this from placing cards into a foundation.
- [x] Larger centered stock/waste area; much smaller shuffle button with a usable touch target.
- [x] Easier fast drag/drop and magnetic snapping only to legal destinations.
- [x] Opaque card faces and separated card layers prevent symbols leaking through.
- [x] New deal/new game and Undo remain usable at all difficulties.
- [x] Center the completed-game panel and New Game button.
- [x] Shuffle animation moves several cards apart and back together; cleans up afterwards.
- [x] Real recorded placement/slide/shuffle audio integrated into shared card sounds.
- [x] Replace the busy card backs with a plain, restful back.
- [x] Simplify excessive face decoration without removing the requested circus illustrations or approved layout.
- [x] Endgame auto-play triggers only when every remaining card is revealed and a complete legal foundation path is verified. Does not auto-play uncertain positions.
- [x] Final regression of long stacks, all five difficulties, landscape, larger accessibility text, live shared play and completion after the final visual changes.

## 2. Pinball — Space Cadet reference

- [x] Opened and visually inspected the supplied Space Cadet reference.
- [x] Larger responsive machine; left/right keyboard and touch flippers.
- [x] Open center drain and side drains; finite ball saver and proper game over.
- [x] Manual pull/release spring, including holding Space and releasing.
- [x] Longer visibly compressing spring and stronger launch, up to 150% power.
- [x] Multiple bumpers, slingshots, target banks, raised ramp, orbit, wormholes and kickout holes.
- [x] Missions, multipliers, fuel bonus, combination bonus and mission jackpots.
- [x] Chasing lamps, hit flashes, moving targets, rings, sparks and score popups; reduced-motion behavior and bounded effects.
- [x] Digital-style scoreboard and mission display.
- [x] Downloaded the user-supplied pack: all 50 original WAVs and ZIP backed up under `F:/infinity/Qurio/source-audio/pinball`.
- [x] Compressed and level-balanced MP3 effects; mapped flippers, impacts, bells, slots/bonuses, launches, drains and game-over cues.
- [x] Prepared a lightweight space-arcade music loop with saved volume/mute handling.
- [x] Reconcile both music requests: SFX always available; **music optional in Sound settings, off by default**, rather than forced background music.
- [x] Final play/visual/audio comparison to Space Cadet's responsiveness and busy table; do not claim an exact original engine.
- [x] Fixed-step physics, all-difficulty accelerated finite-run checks, pause/background handling and low-end CPU rendering checks.

## 3. 8-Ball Pool — original Miniclip reference

- [x] Downloaded and inspected the linked `0wwafa/8ball` repository on F:.
- [x] Established that the repository is a wrapper around Miniclip's hosted runtime, not a standalone open pool engine.
- [x] Found and downloaded original table texture atlases and original gameplay/turn/win/loss sound resources from the runtime URLs referenced by that wrapper. Backups on F:.
- [x] Recreate the reference's complete table appearance, balls, cue, HUD, power control and effects using the supplied references/resources. This is one of the **three** requested style recreations, alongside pinball and Pac-Man; do not redesign every other game.
- [x] Integrate the original table atlases cleanly, retaining correct pocket/cushion alignment and responsive portrait/landscape rendering.
- [x] Integrate original cue, ball collision, cushion, pocket, rack, foul, turn, win/loss and cheering recordings, with appropriate gain and mute behavior.
- [x] Portrait view now places the cue/player at the bottom and the rack above.
- [x] Stick can be pulled and released to shoot; fine aim and power controls remain available.
- [x] Further improve cue maneuvering and match the reference's control feel; verify fast swipes do not fire accidentally.
- [x] Show the cue immediately, including before the initial ball-in-hand placement is completed.
- [x] Add a pre-game left-handed/right-handed choice and position the power bar accordingly.
- [x] Verify the power bar stays fully visible on narrow phones without making balls too small.
- [x] New Round action exists.
- [x] Put New Round/New Game at the top, not underneath the table.
- [x] Wrong first contact is a foul; the opponent receives ball in hand at any clear legal position. Existing engine test covers this.
- [x] Standard called-ball/pocket, break decisions, group assignment, 8-ball and scratch rules exist; shared shot simulation is deterministic.
- [x] Audit those rules against the requested original-game experience; keep normal rules consistent between solo and hosted play.
- [x] Show the opponent's cue position, aim and pull live, before the shot, without excessive network traffic.
- [x] Clear turn notification **after balls stop**: original turn sound, lit active-player border and a short Your Turn/name announcement. No wrong-player alerts on reconnect.
- [x] Automatic background songs are suppressed for pool; sound settings remain in the menu.
- [x] Finish the requested original-style recreation and test on phone, landscape, desktop and two real room clients before marking complete.

## 4. Snakes & Ladders

- [x] Fair die result; strength affects animation, not odds.
- [x] Manual tap/drag of the character to the legal destination.
- [x] New patterned, tapered snakes with distinct heads, eyes and forked tongues, based on the physical-board reference.
- [x] Improved board colors; readable numbered tiles.
- [x] Tokens now animate through intermediate squares rather than teleporting after manual placement.
- [x] Recorded dice roll and board-hop effects; automatic music suppressed.
- [x] Add the missing jungle graphics/foliage and verify the board/tile size uses available room sensibly.
- [x] Do not reveal the destination, highlight or rolled result in the visible notice/journal until rolling finishes.
- [x] Final check of manual moves, ladders/snakes, exact-roll finish and all difficulties in solo/live play.

## 5. Dice, shared by Snakes & Ladders and the opening Tic-Tac-Toe contest

- [x] Replace flat die characters with proper animated 3D six-sided cubes and pips.
- [x] One d6 for Snakes & Ladders; two players' d6 in Tic-Tac-Toe.
- [x] Downloaded and inspected Sarah Rosanna Busch's MIT dice reference on F:; attribution/license retained.
- [x] Swipe velocity/distance interaction adapted from that reference; click/tap and keyboard activation also supported.
- [x] Rolling animation, bounce/tumble and authoritative final result.
- [x] Verify final TTT roll timing, result hold, dice hiding, best-of-three score and touch swipe behavior after all changes.
- [x] Confirm no early destination reveal in Snakes & Ladders and no accidental double roll.

## 6. Checkers

- [x] Recorded chip impacts available through shared SFX; automatic music suppressed.
- [x] Optional captures, backward captures by men and flying diagonal kings in current relaxed rules.
- [x] Blocking pieces still prevent impossible king moves; no jumping across occupied squares except a legal capture.
- [x] New Game action exists; universal menu can restart or exit.
- [x] Fix the pale orange to a richer clear orange and visually verify it on a phone.
- [x] Remove premature automatic repetition/quiet-move endings for the requested relaxed rules. Finish only for a real terminal position or explicit surrender; preserve legacy-room behavior where needed.
- [x] Add/verify explicit surrender and test that a losing bot cannot prematurely terminate a playable game.
- [x] Final live/touch/capture-chain regression.

## 7. UNO — variants and optional house rules

Merged into the pending update while retaining the published classic engine for older snapshots. Engine rules, 108 accelerated rounds, hosted pause/restore/score continuity and responsive variant UI checks passed. Final release/live-worker verification is still pending.

- [x] Mode picker with explanations on hover and touch.
- [x] Speed: five-second turns with a timer at the active character.
- [x] Roulette: a central animated mystery wheel selects a temporary rule each round.
- [x] Tournament: continuing rounds, accumulated points and an overall winner/crown.
- [x] Partners: one teammate card transfer per round.
- [x] Mystery: genuinely secret objectives with correct progress and end conditions.
- [x] No Mercy: penalty stacking, stronger action cards, 7–0 actions and elimination at 25 cards.
- [x] Flip: complete two-sided deck and light/dark side transition.
- [x] Teams: 2v2 or 3v3 with correct teammate rules and optional shared penalties.
- [x] Pre-game individual house-rule switches with clear explanations.
- [x] Stacking: match/equal-or-stronger draw penalties and pass the accumulated total correctly.
- [x] The requested 7 hand-pass rule and 0 hand rotation, following play direction.
- [x] Six Slap race, hand animations and configurable one/two-card last-player penalty.
- [x] Exact-card jump-in/out-of-turn play; correct skipped-player handling.
- [x] Double Trouble: two identical color/value cards together.
- [x] Optional 25-card elimination.
- [x] Sudden Death after the first reshuffle, with correct passing and no endless stalemate.
- [x] End-of-round reveal/count of remaining hands and identify the highest total/loser.
- [x] Continue with retained scores or explicitly start a new match.
- [x] Hide/show score board.
- [x] Visible special-rule reminders, rotation arrows, wheel/slap/swap tools and animations.
- [x] Final two-client hosted variant check and deployed-worker verification; local room deadlines, privacy, snapshot restoration and score continuity tests pass.
- [x] In published 1.0.60: draw/discard piles persist, active playable cards lift, action sounds and Catch UNO race/penalty work.
- [x] Preserve and recheck those 1.0.60 fixes when merging the variants.

## 8. Wordle and previously requested 5 November maintenance

- [x] Published 1.0.60: typing/deleting/submitting sounds, invalid/wrong-word buzz and shake.
- [x] Misses are counted in solo and online modes.
- [x] Purple 2× indicator for already confirmed repeated letters; do not reveal unearned answers.
- [x] Larger board and keyboard, raised keyboard, softer rounded tiles.
- [x] Published poker New Game fix and NPC rotation without duplicates/main-character opponents.
- [x] Published updated Zendaya (2015 Oscars reference), Paris Hilton, Lady Gaga and shirtless Terry Crews portraits.
- [x] Nicki Minaj replacement succeeded on retry: pink blunt-bang hair, cream outfit and gemstone necklace from the supplied reference, rendered in the existing avatar style with transparent margins. Source backed up on F:.
- [x] Published warm, rounded menu/result styling in Qurio colors, without fake levels/shops/items.
- [x] Published local avatar/medal rankings and performance-percentage half-star awards; Android backup mirror and merge-safe backup/restore.
- [ ] Live permanent server ranking sync was explicitly deferred by the user in 1.0.60. Track separately, verify deployment/idempotency before enabling, and never delete existing results.
- [x] SoundCloud and YouTube removed; saved local sound/music settings retained.

## 9. Pac-Man — new request today

- [x] Downloaded and inspected the supplied Pac-Man reference, source and 15 audio files on F:.
- [x] Real maze/ghost/pellet/power-pellet/fruit/game-over engine integrated; source/license attribution retained.
- [x] High-DPI responsive rendering, swipe input, direction pad and keyboard controls.
- [x] Difficulty changes speed, starting challenge and lives.
- [x] Game is isolated in its own iframe program; host communicates through a data-only message protocol.
- [x] Finish post-isolation regression and disable inappropriate built-in debug/skip/menu shortcuts.
- [x] Verify full offline play and compressed audio volume/mute/background behavior.
- [x] Verify local rankings and multi-client simultaneous high-score contests, waiting for all players and keeping the same room for replay.
- [x] Verify live server support for this new mode before publishing.
- [x] Publish corresponding standalone GPL game source with the release and keep its source link correct.
- [x] Final reference look/play/sound comparison; this is the third requested reference recreation.

## 10. Shared presentation, audio, performance and menus

- [x] Reviewed all 109 existing NPCs and added two short signature/personality lines each. Corrected local-AI mismatches, preserved silent gestures and main-character voice rules, and checked IDs, line lengths and correct live bubbles. Added deterministic selection in shared bubbles without extra speech events.

- [x] Permanent project rule: keep NPC illustration/proportions, icon style/size, shared controls and effects consistent. Reference photos guide clothes/hair/appearance without replacing the established game art style.

- [x] All launcher game icons use one illustrated badge style, consistent frames and normalized artwork bounds.
- [x] Equal icon size checked at 320, 390, 768 and 1280px; current game count includes Pac-Man.
- [x] All 109 NPC portraits normalized to equal optical extent; clear edges checked.
- [x] NPC portrait frame dimensions equalized within the card table, including the top seat.
- [x] Smaller speech bubbles above characters in poker/blackjack, UNO and roulette.
- [x] Final speech bubble/card/viewport overlap and readability check on phones and with many seats.
- [x] Prefer real downloaded sound libraries. Kenney CC0 card/chip/dice recordings and supplied pinball sounds integrated.
- [x] Keep original downloaded sources on F:. Compress copies for Android; preserve source/credit notices. Pinball effects plus prepared music are about 1.5 MB.
- [x] Use the original pool recordings/resources now obtained and validate their levels, timing and provenance notices.
- [x] Universal top-right menu, renew/new game, exit to main menu and sound settings in every game, including Pac-Man.
- [x] Check/resolve freezing and lag in the changed games, with bounded animations, canceled background loops, offline assets and low-end-device checks. Never promise every device is lag-free without evidence.
- [x] Retain existing room identity, sessions, scores and active games through backend deployments and updates.
- [x] Triple-check requested layouts/controls on narrow/tall phones, landscape, tablet and desktop; retain approved Solitaire, Wordle and other game designs.

## 11. Bartender — now authorized during final work

- [x] Security scan found and quarantined the upstream nested Windows ZIP payload (not executed). ZIPs/binaries were excluded from the start; isolated 91-file web runtime was scanned separately with zero detections. Keep payloads out of all APK/source packages.

- [x] Downloaded the supplied Apache-licensed source to F: and isolated the game from existing modes.
- [x] Bundled Tone and compiled Tailwind locally, compressed seven audio tracks, and disabled external weather/location/music endpoints and camera/photo UI.
- [x] New painted bar background and 47 guest portraits rendered using the existing Qurio NPC renderer; icon matches the same badge/size rules.
- [x] Reviewed and applied 39 English UI translations drafted by the local AI.
- [x] Added Shake/Stir/Build controls to match the actual recipes; difficulty sets the shift duration.
- [x] Real-drink scoring, correct mixing methods, pause, mute/song switching, hide/show controls, 320px–desktop layouts and completed-shift ranking checks pass.
- [x] Verify two-player high-score contests, replay and live worker support, preserving existing rooms.

- [x] Inspected the linked Bartender-EN repository and answered that integration is technically possible with mobile adaptation and testing.
- [x] NEW REQUEST: integrate the supplied Bartender-EN game with a responsive full-screen phone layout, offline assets/audio, consistent icon and standard menu/restart/exit/sound controls. Check input, performance and game ending before publishing.

## 12. Live checklist and ongoing tracking

- [x] Created this master Markdown checklist and recorded additions from the day.
- [x] Published a phone-friendly live HTML view: https://infinitystudiohome-code.github.io/piggycade-releases/progress/ . It refreshes every 15 seconds.
- [x] Public page and checked/open filters verified at 320px and 390px. Publish task progress after each verified item; continue to the next task automatically.

- [x] Refresh button verified against the public site: makes a fresh request, updates Last checked, retains tasks during a network failure, and recovers. Tasks last changed is shown separately.

## 13. Final update delivery — published and verified

- [x] Audit every item above against the actual source and evidence; move unchecked items to checked only after implementation and a relevant check.
- [x] Preserve all prior fixes while merging unfinished UNO work.
- [x] Backend regression tests, room-restore tests and targeted live checks pass.
- [x] Required `check-launcher.cjs` gate passes on the final bundled assets, including Update with a deliberately broken launcher.
- [x] Build the signed APK with unchanged application ID/signing key and incremented version/code.
- [x] Package private source and the separate required Pac-Man source archive without signing secrets.
- [x] Publish APK, verify public updater manifest/hash/version/download, and copy the final APK to the usual delivery folder.
- [x] Provide the download link and PC location. Do not say the update is available before publication is verified.

## Latest verification evidence

- Additional 10 live two-client cases pass: all five difficulties, Snakes overshoot/exact finish/manual drag/token tap, Checkers backward captures for both colors and optional chain ending. A cell-locator interception was checked against real token input and correctly rejected as a false bug; no unnecessary runtime handler added.

- 169/169 backend tests pass, including active room restoration and legacy snapshots.
- Full browser gate passed before the last screenshot corrections. Final build reruns that mandatory gate on the final bundle; no bypass.
- Screenshots compared at phone/landscape/desktop: original pool textures, rotated bottom-side cue and visible rack, pinball lamps/spring/scoreboard, circus Solitaire, patterned jungle snakes, richer orange Checkers, classic Pac-Man maze and painted Bartender.
- Screenshot review found UNO action text crossing card labels and an oversized pair checkbox. Fixed separate announcement lane and compact 22px checkbox; tests now assert no overlap with piles, names or labels.
- Independent audio reviewer found sampled bets were identical and pool fallback outcomes were card flicks. Fixed distinct bounded chip stacks and proper outcome fallbacks; 22 actual-recorded/fallback audio render checks pass.
- Live worker receipt: UNO Speed/private hands, pool shared cue previews, Pac-Man and Bartender progress accepted in the same QA room; no fake ranked results created.
- Pac-Man audio fully local: 15 decoded tracks, mute/unmute and paused audio verified with no external requests. Corresponding GPL source archive generated.
- Reference recreations use the available original resources with Qurio controls and custom pool/pinball engines; they are not the original proprietary binaries. Automated browser and 6× CPU-throttle checks do not guarantee every physical phone.
- Local Infinity AI returned final QA suggestions; unsupported specific physical-device claims were not treated as completed evidence. No Android device is attached to ADB.

## Current next actions

1. COMPLETE:1.0.63/code64 published. Publicdownload and both updaterendpoints verified; SHA256 `8417b6549b2b172e33c4c18081b1210483948a8d1ea86e75305a80d7b1bf90b8` . PCcopy C:/Users/Administrator/Documents/ChatGPT/win/FamilyQuest/delivery/Qurio.apk . Download https://github.com/infinitystudiohome-code/piggycade-releases/releases/download/v1.0.63/Qurio.apk .
2. Reproduced/fixed delayed saved-room response replacingSolo witholdpausedgame; normalauto-restore/manualrejoin/newroomcreation remainvalid, savedtoken retained. Reproduced/fixed offlineSudoku inputdeadlock afterbackground. Reproduced/fixed transientcanvasfault losingPinball/Poolanimation; bounded3retry recovery/contextrestore preservesball/score/shot, explicitpause/background honored. Pooltexturesloadonlywhenneeded.
3. Targeted actual-index/device-density/touch/graphicsfault/multiplayer/paused/visible tests passed. Mandatory scopedHost/Update/brokenlauncher gate passed forbuildandpublication.495APKassets match finalbundle;476unrelatedassets/allbackendmodules unchanged. Signing/appID unchanged; Defender APKscan clean. Private source andpubliccorrespondingPac-Man source published. No roombackenddeployment/reset.
4. Partner should test1.0.63 onactualCamon. Ifitstillfreezes: Menu → Connection & performance report → Copy report. Actualdevicecause notconfirmed byemulationalone. Report stayslocal, redacts tokens andincludes WebView/version/framehealth withoutboards/answers; pauses localgame whilecopying. Permanentserverrankings remainpreviouslydeferred. PC notputtosleep/shutdown.

## 14. Reported after 1.0.61 publication

- [x] Fix Bartender getting stuck on main-menu loading; verify real launcher entry, not only direct game URL.
- [x] Check the same launcher ready handshake for Pac-Man.
- [x] Fix pinball ball becoming stuck; compare visible rails with collision geometry using supplied screenshot, and test corner/ramp/launch-lane escapes.
- [x] Build and publish the corrective update with saved games and rooms retained.
- [x] Add supplied Space Cadet music from https://youtu.be/j5K5TMabOXM as a short seamless compressed loop instead of an hour-long file; preserve volume/mute settings.
- [x] Check upper-left pinball pass-through and all visible solid obstacles against collision geometry; add a regression for reported passage.
- [x] Solitaire Shuffle should automatically reveal the next draw-three hand, top card only playable, with no extra tap, move or point cost; verify solo/live/undo.
- [x] Wordle on-screen keys must show consistent press/flash animation on every touch, including repeated taps; preserve key clue colors.
- [x] Pinball launcher spring needs audible mechanical pull/tension while dragging, matching supplied Space Cadet pack where available, plus release sound; volume/mute respected.
- [x] Top navigation/Menu/Qurio/Back buttons need reliable press feedback; leaving a game must confirm first and explain unfinished progress may be lost while saved scores/profiles remain. Cancel must leave game playable.
- [x] UNO opening: visible shuffle then round-robin cards fly from stock to every player; no playable cards until deal completes, avoid replaying intro on reconnect, support reduced motion and all seat counts.

## 15. Camon30Pro freezing report

- [x] User confirmed Solo also freezes and Menu remains responsive. Network/location is not the primary explanation.
- [x] Investigated connection/lifecycle: Pinball passed nine native/visibility resume cycles; shared network delays cannot explain Solo freeze. No server change for this update.
- [x] Checked native/visibility lifecycle,3× mobile-density diagnostics, transient/persistent graphics faults and lazy texture loading. No physicalCamon attached; report captures its actual WebView and errors.
- [x] Fix reproduced offline Sudoku input deadlock after background/resume without resetting timer/board/notes.
- [x] Recover Pinball/Pool from transient canvas or media frame failure/context loss without resetting score/ball/shot; add copyable diagnostics for actual device error.
- [x] Build/publish1.0.63, verify primary/fallback updater, publicdownload hash/signature, and provide partner test/report instructions.
- [x] Prevent delayed saved-room restoration from replacing an already started Solo game; keep saved reconnect identity and test oldpausedroom response.
