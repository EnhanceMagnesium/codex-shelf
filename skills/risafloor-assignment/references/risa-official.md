# RISAFloor official software workflow

Based on RISA's online RISAFloor help, checked 2026-11-27. The open version's visible controls and user instructions govern interaction. Consult a linked page when a version-specific detail needs clarification.

## Concrete floor and geometry

RISAFloor ES supports concrete floor slabs supported by columns or walls. In Create New Floor Plan choose Concrete Floor Slab and the assigned design method. Define the drawing/project grid, column and wall properties and positions, slab perimeter and openings, then any beams required by the assignment. Model views and spreadsheets reflect each other under the normal settings. Project grids describe building axes; drawing grids assist placement. Verify the active global axes and exact coordinates, as rotated views can change screen appearance.

Sources: https://help.risa.com/risahelp/risafloor/Content/Floor_Only_Topics/Elevated%20Slabs.htm and https://help.risa.com/risahelp/risafloor/Content/Common_Topics/Graphic%20Editing.htm

## Area loads and combinations

Uniform area-load magnitudes are defined in Spreadsheets > Loads > Area Load Definitions, then assigned graphically with Draw Area Loads. The general load page lists several application methods, but its elevated-slab-specific limitation states that Point to Point Draw of the Area is the only manual assignment option for elevated slab floors. Select the defined load, click Apply, draw the closed boundary using the controls in the current version, then inspect the resulting load. Use Area Load Query to verify load cases at a location. Check overlapping/additive load settings and self-weight to avoid double counting.

Loads belong to cases that feed load categories. In Spreadsheets > Load Combinations inspect each category and factor, ensure the desired combinations have Solve selected, then run Solve. Loads omitted from the combination's categories are omitted from that solution. Use appropriate strength and service combinations.

Sources: https://help.risa.com/risahelp/risafloor/Content/Common_Topics/Loads%20-%20Load%20Types.htm and https://help.risa.com/risahelp/risafloor/Content/Common_Topics/Loads%20-%20Load%20Combinations.htm

## Support lines and reinforcement

For the Design Strips method define slab design rules, draw support lines in both plan directions, generate strips and inspect their coverage and geometry. Verify top and bottom cover, bar sizes and allowed spacing against the assignment and actual crossing-bar layers. The User Defined method instead checks specified uniform reinforcement; RISA states each method ignores the other method's corresponding reinforcement settings. Absence of strip coverage can leave areas without a complete reinforcement design.

Design-strip detail reports identify analysis steel, minimum flexural reinforcement and other checks that govern the provided steel. Construction and Theoretical methods display reinforcement differently; do not interpret a generic theoretical cross-section as a discrete bar schedule. Manual design cuts give analysis information but not design information.

Sources: https://help.risa.com/risahelp/risafloor/Content/Floor_Only_Topics/Elevated%20Slabs%20-%20Design%20Strip%20Modeling.htm and https://help.risa.com/risahelp/risafloor/Content/Floor_Only_Topics/Elevated%20Slabs%20-%20Design%20Strip%20Results.htm

## Results and limitations

Open result spreadsheets through the Results menu and capture the actual combination, units, location, sign and governing values. A punching-shear unity check is a demand/capacity ratio, with its governing load combination. Verify column attachment: RISA says a column node outside the slab is not considered attached for punching checks. Its documentation also says punching for walls, point loads and non-concrete columns is not checked in the described workflow. ACI 318-19 has a conditional minimum reinforcement check at the punching perimeter reported in the column detail report that the elevated slab reinforcement design does not automatically incorporate; check this only where the selected edition and condition apply.

The software checks slab deflection for the entered thickness; it does not automatically redesign thickness for deflection. RISA describes long-term creep/deflection limitations for the Design Strips method. Record the selected analysis/design options and avoid claiming a long-term check unless its actual output supports it. Reconcile the selected software code edition with the course method.

Sources: https://help.risa.com/risahelp/risafloor/Content/Common_Design/Punching%20Shear%20-%20Results.htm ; https://help.risa.com/risahelp/risafloor/Content/Common_Design/Punching%20Shear%20-%20Design.htm ; https://help.risa.com/risahelp/risafloor/Content/Floor_Only_Topics/Elevated%20Slabs%20-%20Design.htm ; https://help.risa.com/risahelp/risafloor/Content/Common_Topics/Results.htm
