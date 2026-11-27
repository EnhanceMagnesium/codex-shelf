# RISAFloor lecture workflow reference

This reference extracts the class workflow once so Codex can use it without repeatedly rereading the lecture transcripts. The current assignment supplies the geometry and loads. Current RISAFloor controls and displayed values must still be observed before action. The two lectures contain example dimensions, loads and member sizes that must not be treated as defaults. CD-25 and CD-43 transcript wording is automatic speech recognition and may contain errors.

## Establish the problem and coordinate system

- CD-25 00:01–00:11 distinguishes slabs supported on beams from slabs supported directly on columns and discusses punching at the column–slab connection. Model the system shown in the current problem.
- CD-25 00:13:35–00:14:00 starts a new floor plan and selects Concrete Floor Slab. The inspected frame CD-25-V004 (00:13:45) shows reinforced-concrete slab type and Design Strips. The instructor's other displayed values are example-specific.
- CD-25 00:15:52–00:17:44 opens Project Grid and generates grid lines. CD-43 00:16:17–00:22:36 locates points by coordinates and uses point labels to inspect them. In the demonstrated RISA plan view, Z is horizontal and X vertical. Check the actual axes icon and units in the open application.
- A drawing grid is a placement aid. Define increments or coordinates that reach every required column position, and check whether a field means spacing, count or total extent. A project grid describes actual design axes. Do not import the instructor's example bay spacing or column sizes.

## Build the floor

- CD-25 00:18:44–00:20:04 uses Insert > Columns, defines a rectangular column section, then clicks each intended snapped intersection. Inspect the count and positions after placing them.
- CD-25 00:20:21–00:21:28 and CD-43 00:26:03–00:29:37 use Insert > Slabs, define slab thickness and choose Draw Slabs. Click the perimeter vertices and return to the first point to close it. Inspect both plan and isometric/rendered views for slab shape and column connectivity.
- CD-43 00:22:36–00:26:03 demonstrates defining and drawing beams between points when the actual assignment calls for beams. The example's members are not a basis for adding beams to another floor. Model openings and edge offsets from the actual figure or declared assumptions.

## Loads, combinations and analysis

- CD-25 00:22:27–00:26:48 and CD-43 00:30:11–00:33:05 describe area-load definitions and occupancy selection. The observed CD-25-V006 frame shows the relevant load menu. Inspect the actual chosen office live load and units. Enter assignment superimposed dead load separately and check program self-weight so slab weight is counted once. Apply the area load to the intended polygon or panels, checking the actual version's selection method.
- CD-25 00:27:28–00:28:40 and CD-43 00:33:05–00:35:53 inspect the load-combination spreadsheet and solve the model. The lecture explicitly discusses 1.2D + 1.6L. CD-43 ASR also contains an inconsistent 1.4L phrase; inspect the actual software combinations and class provision rather than relying on that transcription. Distinguish strength from unfactored service combinations.
- Check warnings and visible modeling errors. After revising geometry, loads or design settings, rerun analysis and capture the final state.

## Read results and design reinforcement

- CD-25 00:29:02–00:32:13 and CD-43 00:35:53–00:44:39 demonstrate slab color-fill contours in Mx and Mz under a strength dead-plus-live combination. CD-25-V009 (00:29:48) visibly shows the contour controls; that particular frame displays a service-dead selection, so it does not itself establish a strength result. Verify the current combination, axis directions, sign convention, units, actual result locations and values.
- Review both directions and both positive and negative regions. Capture design-strip/column-strip and middle-strip reinforcement where available, bar sizes and spacing, locations, punching shear and warnings. The instructor also demonstrates hand reinforcement design from moments; that does not establish that every version of RISAFloor has already generated a complete rebar schedule. Distinguish actual table values from the ends of a color legend.
- CD-25 00:42:13–00:44:48 and CD-43 00:45:45–00:46:40 switch to slab displacement with an unfactored service dead-plus-live combination. Read the numerical displacement and units; the deformed display can be magnified visually.
- CD-43 00:48:13–00:51:47 locates concrete beam bending results when beams are actually modeled and column-force results for column design. Extract column axial forces and moments with their combinations and locations. Do not infer an actual result from a worked lecture example.
- CD-43 00:54:34–00:56:44 emphasizes capturing figures with legends. Preserve screenshots or exports of the inputs, grid, loads, combinations, warnings, slab force and reinforcement tables, deflection and column demands. Maintain a concise progress log so another session can reproduce the model state.

## Evidence and scope

CD-25 source: https://www.youtube.com/watch?v=vXvLt1q6iGw. CD-43 source: https://www.youtube.com/watch?v=RzBqXA85Fy8. CD-25 frames V004, V006 and V009 were visually inspected in a portable lecture reference. The indexed CD-43 image folder was not present in the inspected project; its detailed workflow above comes from the timestamped transcript and is not a visual verification of every menu. Frame names and timestamps are retrieval aids, while the actual active application determines which controls are available.

For the current assignment use the separate Q3 computer-use resource for its 20-column grid, stated assumptions and requested GridCraft deliverable. No results have been asserted by this reference.
