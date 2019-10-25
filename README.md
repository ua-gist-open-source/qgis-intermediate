# Assignment: Intermediate QGIS Tutorials
## Worth: 30 points
## Due: 7 days

### Deliverable:
Pull request to merge a new branch named `assignment` with `master`. Your branch should contain:

1. `screencap-nyc-boro.png`
2. `screencap-nyc-boro.png`
3. `screencap-lake-depth.png`
4. `screencap_police_hostpot.png`
5. `screencap-shortest-path.png`

## Assignment

### 0. Checkout this assignment and create a new branch named `assignment`.
Perform all your work in the `assignment` branch. When you have completed the assignment, submit a `Pull request` to merge `assignment` -> `master`.
signment

### 1. Follow the tutorial at http://www.qgistutorials.com/en/docs/3/performing_spatial_joins.html

Take a screenshot from your final step (step 19) showing the attribute table with `boroname` attribute and name it `screencap-nyc-boro.png`

### 2. Follow the tutorial at http://www.qgistutorials.com/en/docs/3/sampling_raster_data.html

Deliverable:

Take a screenshot from your final step (step 16) and name it `screencap-tmax_mean_table.png`

### 3. Follow the tutorial at http://www.qgistutorials.com/en/docs/interpolating_point_data.html 

_Note this tutorial is for QGIS 2._

Deliverable:

Take a screenshot of your from your final step (step 20) and name it `screencap-lake-depth.png`.

### 4. Follow the tutorial at http://www.qgistutorials.com/en/docs/3/creating_heatmaps.html but use Tucson police incidents points from the City of Tucson Open GIS Data website.

Use the data http://gisdata.tucsonaz.gov/datasets/tucson-police-incidents-2017-open-data.
Instead of `Crime type`, use the `reportedas` attribute and use the following as a substitute for the weight calculation:
```
CASE
WHEN "reportedas" LIKE 'ARMED%' THEN 10
WHEN "reportedas" LIKE '%FIGHT%' THEN 5
WHEN "reportedas" LIKE 'ASSAULT%' THEN 5
ELSE 1
END
```
Deliverable:

From step 24, create a screenshot showing the clustered crime hot spots in Tucson. Save the screenshot to a file named `screencap_police_hostpot.png` in the `intermediate` branch of this repo.

### 5. Follow the tutorial at http://www.qgistutorials.com/en/docs/3/basic_network_analysis.html

Deliverable:

Take a screenshot of your Qyour GIS Desktop at the final map (step 16) and name it `screencap-shortest-path.png`

