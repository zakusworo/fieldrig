# How to use Fieldrig

Each tool has a **?** button in its title bar that opens its guide. Load the demo data first (Settings → Demo data → Load demo data) to try every tool with ready-made samples.

## Map
Everything you have switched on, drawn over the street map or your offline basemap.
1. Tap **+** (red) to import a survey file, or the **folder** button to open the map library.
2. Tap the **target** button to centre on your position. Your position shows as a blue dot with a heading cone.
3. Pinch to zoom, drag to pan, and rotate with two fingers.
4. To measure, tap the **ruler** button, then tap points on the map. The panel shows distance, the last leg and its bearing, and the area once you have three points. Use **Undo**, **Clear**, or **Done** to finish.
- Layers are switched on and off in the map library, not on the map.
- With no signal the street map stays blank. Import an MBTiles or PMTiles basemap to work offline.
- TIN triangles fade out when zoomed out and appear as you zoom in.

## Map library
All your maps, kept on the phone.
1. Before importing files in metres (DXF, STR, projected CSV), set the **Default UTM zone** to the zone of the file, for example 48S for West Java or 50S for East Kalimantan.
2. Tap **Import** and pick a file. Supported: DXF (lines, polygons, points, 3DFACE TINs), Surpac STR, KML, CSV (P,N,E,Z,D or lat/lon), GeoPDF, plain PDF drawings, and MBTiles or PMTiles raster basemaps.
3. Use the switch to show or hide a map. **View** zooms the map to it. A plain PDF opens as a document instead.
4. The **⋮** menu lets you rename the map, change its UTM zone (if it was imported on the wrong zone), open a PDF as a document, or delete it.
- Deleting a map removes Fieldrig's copy only. The original file is not touched.
- If a file lands in the wrong place, its UTM zone was wrong. Use **Change UTM zone** to fix it without importing again.

## Cut & fill
Volume between a design surface and the ground.
1. **Design surface:** pick a map with a TIN (3DFACE triangles), for example a pit design.
2. **Original ground:** choose **Flat elevation (RL)** and type a level, or **Another surface** and pick a topography TIN.
3. **Boundary (optional):** limit the calculation to the polygons of one layer, for example the pit limit.
4. **Options:** leave the grid cell blank for automatic, and type a density to get tonnes.
5. Tap **Compute volume**. Cut is ground above the design (to dig). Fill is design above the ground (to place).
- Smaller grid cells are more accurate but slower. The automatic size is a good start.
- If design triangles overlap, the lowest surface is used and the overlap is reported.

## Stakeout
Walk to planned points and record where you actually pegged them.
1. Tap **New layout** and choose:
   - **Survey line** or **Grid of lines:** start point, azimuth (true or grid), length, station spacing and, for a grid, the number of lines and line spacing;
   - **Typed point;**
   - **Points from a saved map** (with vertices if you want them);
   - **Field stations.**
2. Open the layout and tap **Go to next point**.
3. Turn until the arrow points up, then walk. The arrow points relative to the top of the phone. The panel also shows the distance and how far east or west, north or south you still have to go.
4. When it says **On point**, tap **Mark staked here**. The app moves on to the next point.
5. **Export** gives a CSV with design and as-staked coordinates and the offset of each point, or a KML.
- "On point" only appears when the GPS is good enough to tell (fix of 3 m or better). With a poor fix it asks you to wait.
- Phone GPS suits stations 10 m or more apart. For sub-metre pegging use survey-grade GNSS.

## GPS tracks
Record where you walked or drove, or the area inside a boundary.
1. Choose the accuracy limit, for example **±20 m**. Worse fixes are not recorded.
2. Tap **Record a traverse** for a line, or **Walk a boundary (area)** to measure an area.
3. Put the phone away. Recording continues with the screen off, and a notification shows progress.
4. Tap **Stop and save** and give the track a name. For a boundary, stop near your starting point: the area closes back to the first point.
5. Tap a saved track to show it on the map, export it as GPX, KML or CSV, rename it, or delete it.
- Standing still does not add points, so GPS wander does not grow the track.
- If the phone kills the app while recording, the track is saved as "Recovered …" the next time you open it.

## Compass
A sighting and walking compass that checks its own magnetometer.
1. Hold the phone flat with the bubble in the centre ring, then point the top edge. Read the heading under the red index.
2. To sight a target, hold the phone upright and aim the back of the phone at it. The compass switches to sighting mode on its own.
3. **True north** needs a GPS fix (declination from the World Magnetic Model). Choose **Magnetic** to read the raw compass.
4. **Hold** freezes the reading. **Set target** marks the current bearing on the card and tells you to turn left or right to stay on line.
5. Read the box at the bottom:
   - **Calibrate:** wave the phone in a figure 8 until the accuracy reads high.
   - **Magnetic interference:** move away from vehicles, steel and magnetite-rich rock.
- The back bearing (+180°) is shown for back-sighting along a line.
- Check against the sun compass when the readings look wrong.

## Clinometer
Dip and dip direction of a plane, or the angle of a slope.
1. **Flat on surface:**
   - Lay the back of the phone on the bedding plane, joint or ramp. Any rotation works.
   - Read the dip in large digits, and the dip direction as the red arrow against the compass ring.
   - Strike (right-hand rule) and grade are shown below.
2. **Edge along slope:**
   - Rest the long edge of the phone on the slope, lying flat or standing on its side.
   - Read the angle on the protractor, plus the grade and the 1 : n ratio.
   - The tube vial levels to ±10° for fine work.
3. Tap **Hold reading** to freeze the value before lifting the phone.
- On an overhang, or a plane too small for the phone, lay a clipboard on it and the phone on the clipboard.
- To save a measurement with its position, use **Field stations → Measure a structure**.

## GPS camera
Photos stamped with position, bearing, time, address and a QR map link.
1. Wait for a GPS fix. The status line shows accuracy and satellites. Green means good.
2. Tap the **pencil** to set the photo label, for example "Pit 3 bench 45 crack", and to switch the street address and the QR code on or off.
3. Aim and press the red shutter.
4. Tap the thumbnail to open the photo log. From there you can show the photos on the map, export a CSV, or delete photos.
- Photos are saved in Pictures/Fieldrig with GPS in the photo's EXIF data.
- The address needs signal. Offline, the stamp keeps the coordinates and UTM.
- Scanning the QR code opens the photo's position in a map app.

## Sun compass
Sun position, daylight, and a magnet-free check of your compass.
1. Read the sun's azimuth and elevation, sunrise, solar noon, sunset and the daylight left.
2. To check the compass:
   - Stand a pencil upright on a flat surface in the sun.
   - Lay the phone flat with its long edge along the pencil's shadow, top end pointing away from the pencil.
   - Read the **compass error**: within 3° is fine; more means calibrate, or there is magnetic rock or steel nearby.
- The sun must be at least 8° up for a usable shadow, and not so high that the shadow becomes too short.

## Field stations
Your field notebook: one station per outcrop or observation point.
1. At the outcrop, tap **New station**. It takes your GPS position and the next station code (set the prefix with **Station codes start with**).
2. Type the lithology (recent ones appear as chips) and your notes.
3. Tap **Measure a structure** and choose the type (bedding, joint, fault, vein, lineation…). Then measure in one of two ways:
   - **Phone sensor:** lay the phone on the plane, or its edge along the lineation, and tap **Record**.
   - **Type compass reading:** enter dip and dip direction, or strike and dip (right-hand rule). Choose magnetic or true, then tap **Record**.
4. **Add sample** gives a sample code. **Attach photo** adds GPS-camera photos.
5. **Export** gives stations and structures as CSV, samples as CSV, or stations as KML for Google Earth.
- All measurements are stored against true north, using the declination at the station.
- **Retake position** fixes a station recorded with a poor GPS fix.

## Stereonet
Plot and analyse your structure measurements.
1. Choose the data: all stations or one station. Tap the type chips to show or hide bedding, joints and other types.
2. Choose **Equal area** (Schmidt) or **Equal angle** (Wulff). Switch **Poles**, **Great circles** and **Density** on or off.
3. Tap anywhere on the net to read that line, and the plane it is the pole of.
4. Under **Means**: the mean plane of each type, its Fisher k and α95 cone, then the strike rose.
5. **Slope check:**
   - Enter the face dip and dip direction (or record a Slope face at a station) and the friction angle.
   - It counts planes that can slide (planar), pairs that form sliding wedges, and planes that can topple.
- The slope check is kinematic screening, not a factor of safety.

## Drillholes
Core logging at the rig, with strip log and intercepts.
1. **New hole:** take the collar from your GPS position or type surveyed E, N and Z. Set the azimuth, dip (90 = vertical), planned depth and grade unit.
2. **Log next interval:** the From depth fills itself. Enter:
   - To, lithology;
   - core recovered (m) and pieces ≥ 10 cm (m), for recovery and RQD;
   - grade and sample ID.
3. **Add survey reading** with each downhole survey (depth, azimuth, dip). The trace is desurveyed by minimum curvature.
4. Set a cut-off and the internal dilution under **Intercepts** to get results like "8 m @ 3.0 g/t from 55 m".
5. **Export CSV** gives collars, surveys and intervals in the form Leapfrog and Surpac import.
- Tap an interval to edit or delete it. Gaps and overlaps are flagged under the strip log.
- GPS elevation is rough. Type a surveyed collar Z when you have one.

## Samples and QA/QC
Lab batches with quality-control samples and chain of custody.
1. Tap **New lab batch**. Name it, and set the laboratory and the analysis requested.
2. Tick **Add the waiting field samples** (from stations and drillholes), and/or type more sample IDs.
3. Set the QA/QC plan:
   - a standard, a blank and a field duplicate every N samples;
   - the list of standards to rotate;
   - the QC bag ID prefix.
4. Check the rates and the bag order. The app warns if a bag ID is used twice.
5. **Sheet (CSV)** is for the lab. **Custody (PDF)** prints with signature lines. Tap **Mark as sent** when the batch leaves.
- A small batch always gets at least one standard and one blank.
- A duplicate is split from the sample just before it.

## Geophysics logs
Record readings in the field and see the profile or sounding as you go.
1. Tap **New survey** and choose the method:
   - **Magnetics** or **Other readings** (set its unit);
   - **Resistivity profile** (array and spacing a);
   - **Resistivity sounding (VES)**.
2. Optionally follow a stakeout layout: the next station and its chainage are then suggested.
3. Tap **Add reading**. Time and GPS position are attached on their own.
   - **Magnetics:** read the **Base station** at the start and the end of the loop, and every hour or so. Drift between base readings is removed.
   - **Resistivity:** enter ΔV (mV), I (mA) and, for dipole arrays, n.
   - **VES:** enter AB/2, MN/2, ΔV and I. When you change MN, overlap two readings.
4. The plot updates with each reading: a profile, a pseudo-section, or the log-log sounding curve. Tap it to read a point.
5. Tap a reading to edit it. **Export CSV** gives the corrected values.
- On a grid, use the line chips (L1, L2…) to plot one line at a time.

## Cycle time
Truck cycle time and cycles per hour.
1. Tap an example, or enter the loading time, haul distance, loaded speed, dumping time, return speed and spotting or queue time.
2. Read the haul and return times, the total cycle time and the cycles per hour.
- Time a few real cycles with a stopwatch to set the loading and dumping times.

## Matching fleet
Trucks matched to the loader, and shift output.
1. Tap an example, or enter:
   - the truck cycle, loader passes and loader cycle;
   - payload, efficiency and shift length;
   - the number of trucks and loaders.
2. The match factor tells you which side waits. Below 1, loaders wait for trucks. Above 1, trucks queue at the loader.
- Output is capped by whichever side limits the fleet.

## Calculators
Field calculators grouped by discipline.
1. Tap a calculator in the list.
2. Tap **Example 1** or **Example 2** to see it worked with typical values, then type your own.
3. Results update as you type. The formula and its assumptions are shown under the result.
- The coordinate converter and the gravity reduction can **Use my position**.

## Calculator
1. Tap **Example 1** or **Example 2** to fill in a worked example, or type your own values.
2. Results update as you type. If something is missing, the result box says what to enter.
3. Read the formula and assumptions under the result before relying on the number.
- Choices such as the array type or units are the chips above the input fields.

## P2H pre-start
Daily pre-start inspection of a unit (P2H).
1. Tap **New P2H check**. Choose the unit type, then enter the unit number, hour meter, operator, supervisor and shift.
2. Answer every item **OK**, **Defect** or **N/A**. For a defect, write what is wrong.
3. Watch the verdict:
   - **Fit to operate;**
   - **Operate, defects reported;**
   - **Do not operate:** any critical item (brakes, steering, seat belt, horn, reverse alarm, fire extinguisher…) has a defect.
4. Tap **Save check**. Open a saved check for its **PDF** with signature lines. **Export all checks (CSV)** builds a log for the site.
- There is no "all OK" button on purpose: every item has to be looked at.

## Daily report
The day's field report, half-filled for you.
1. Pick the day with the arrows.
2. **Recorded in the app** lists what you did that day: stations, holes, readings, staked points, tracks, photos and P2H checks.
3. Tick the weather. Fill in the crew, hours, activities, hazards (incidents and near misses) and the plan for tomorrow.
4. Tap **Save report**, then **Share as PDF** to send it.
- Saved reports are listed at the bottom; tap one to open it.

## Settings
1. **Name** and **photo:** shown on Home, on GPS photo stamps and on imported maps.
2. **Theme:** Light for sunlight, Dark for night shifts, or follow the phone.
3. **Demo data:** loads a made-up prospect with samples for every tool. **Remove demo data** takes out only the demo records.
4. **Default UTM zone:** set it in the map library.
