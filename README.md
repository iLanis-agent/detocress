# Detocress 1.0 TEST
Native Android Detour room-turn puzzle. Android 8+ (min26), target35. Package com.gg007.detocress. Six original unique boards on a 4x4 grid.

## Rules
Detour on a 4x4 grid divided into four outlined rooms. Draw one noncrossing orthogonal loop through all sixteen cells exactly once. Each room number gives the total number of right-angle turns made in that entire room. Straight passages do not count. Zero means no turns in that room. The loop may enter the same room more than once. Every cell needs exactly two links; no branches, skipped cells or separate loops. Tap gaps between neighboring cells to add/remove links. Six original uniquely solved room layouts with six distinct loop solutions; undo/reset, levels and saved palette/optional room letters. Known Detour adaptation.

## Download and status
https://mega.co.nz/#!lYkCwbpI!lDaKLsPzNPCRiyUMJp53qh0LzdGoP3Q6SUfekK6jQ7o
APK SHA256 dd053fd83b1fdd0145bc77665420440c3f272cf903711d6c3db74ff6d3eb5119; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Portable seed-781110 generator checks 117 connected four-cell room partitions and enumerates all six Hamilton loops of the 4x4 grid. It selects six distinct uniquely solved room layouts, one for each distinct loop geometry, rather than padding twelve boards with repeated solutions. Independent oracle uses disjoint-set connectivity, degrees and horizontal/vertical edge-incidence counts for room bends; production walks a cycle and classifies neighbor directions. All 100,663,296 complete edge-state checks plus 120,000 randomized/invalid room-clue cases agree. Bounds, undo/replay/reset and solved lock pass. Actual drawing-adapter edge-midpoint taps solve all six and check menu, privacy, levels, next and saved palette/room letters/completion. Seven drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 209 live studio descriptions and the 803-entry web registry. No functional match for full-grid single-loop room turn quotas. Turncress makes white circles within a room uniformly turn or uniformly go straight, while ordinary cells can be skipped; Detocress counts every bend in the room and must cover every cell. Glowwillow counts turns along firefly beams in a network, not room totals in one full-grid loop. Known Detour adaptation; original generated layouts, code and visuals, not a global invention. Six sources cover independent rules, constructor posts, a genre index, research and implementation history. The rules agree; the origin sidebar on Janko conflicts with constructor/research attribution, so no origin attribution is adopted. No source layouts, code or art copied.
Rules https://www.janko.at/Raetsel/Detour/index.htm ; independent rules https://ihnnpuzzles.blogspot.com/2019/09/puzzle-68-detour.html .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/detocress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.detocress.DetoBoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Detocress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, optional room letters and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 210-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/cp103b3oqli1-detocress-source-archive . Repository https://github.com/iLanis-agent/detocress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
