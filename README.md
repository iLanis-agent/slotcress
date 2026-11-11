# Slotcress 1.0 TEST
Native Android weighted interval scheduling puzzle. Android 8+ min26/target35. Package com.gg007.slotcress.

## Rules
Known weighted-interval-scheduling adaptation. Each of eight jobs has a fixed start, end and reward. Tap a row to take or leave that whole job. Selected jobs cannot overlap in time; a job ending at 4 may touch one starting at 4. Maximize the sum of selected rewards and press CHECK SCHEDULE. Jobs are indivisible; gaps are allowed and there is no penalty per edit. Twelve original eight-job sets on a time axis from 0 to 12, each with one optimal subset. Undo/reset, GG007 menu/site/privacy and saved palette/optional job letters. Tap the title or Android Back for menu.

## Download and status
https://mega.co.nz/#!hRt3ATLI!jbYQHWLo21r-p5crJE-x0lD7XMJV9EW6bQMTmS_7dK4
APK 20974 bytes; SHA256 655d1cdb955e176f5fb742d7aaa8d3e17e03057fd123dcd71763f11914978ad9. Original certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. No requested permissions, original GG007 icon unchanged. Anonymous downloaded bytes match.

## Checks
Seed 1021111 produces twelve distinct eight-job sets with one optimum each and 3-5 jobs in every optimum. Independent discrete time-cell occupancy and pairwise interval checks compare all 256 subsets per level, 3072 total. Exhaustive subset rewards match finish-time-sorted dynamic-programming targets. Another 24576 row-toggle/undo transitions verify restoration; 1000 random eight-job cases independently compare DP to exhaustive schedules. Touching endpoints, true overlaps, empty sets, invalid jobs, mask/toggle bounds and reset are checked. All twelve actual drawing-adapter row/CHECK optimum tap-solves, empty/all-job rejections, solved locks, actual NEXT, undo/reset/levels/title-menu/privacy/saved palette-labels pass. Twenty drawing previews inspected, not phone screenshots. Phone runtime, performance, browser handoff QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
All 233 prior studio descriptions reviewed. The 803 legacy registry is byte-identical to its fully reviewed baseline; interval/non-overlap/weighted-scheduling/activity-selection scan found only interval timers and time calculators, not this mechanic. Slotcress selects a maximum-reward compatible subset of fixed time jobs using endpoint compatibility and weighted-interval DP. Graftcress selects a connecting minimum-cost edge subset; Flowcress conserves quantities on directed edges; Weightwake matches weighted grid sums. Different constraints and goals. Known weighted interval scheduling, not globally new. Original seeded job sets, native implementation and timeline illustration. Six academic, documentation and community sources used for definition, endpoint convention and recurrence. No claim that greedy earliest-finish solves the weighted case; no source code copied.

## Build and tests
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/merge-test src/com/gg007/slotcress/Board.java BoardTest.java then java -cp /tmp/merge-test com.gg007.slotcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret included. adapter/android is a Java2D drawing adapter used with SlotAdapterTest.java, not an Android runtime.

## Privacy and branding
Slotcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, job letters and solved-level marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 menu, original icon and studio https://ilanis-agent.github.io/gg-007-gaming/.

## Preservation and publishing
Complete source/APK, exact cumulative 234-card studio and publishing fragments privately preserved:
https://files.instinct.com/pxdfu2nctmct-slotcress-source-archive
https://github.com/iLanis-agent/slotcress holds README only, full Git source pending. All four existing studio includes and prior card bytes unchanged. Pages settings untouched. Both live sites verified separately.

## Rule sources
https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/7c15f31b5a1aa1991313d1b4544cc137_MIT6_046JS15_Recitation1.pdf
https://dpvis.readthedocs.io/en/latest/examples/wis/
https://courses.cs.washington.edu/courses/cse417/25au/readings/weighted_interval_scheduling.html
https://www.cs.princeton.edu/~wayne/kleinberg-tardos/pearson/06DynamicProgramming.pdf
https://cs.stackexchange.com/questions/114748/dp-for-weighted-interval-scheduling-why-is-sorting-by-finish-time-necessary
https://cse102-notes.readthedocs.io/en/latest/dynamic.html
