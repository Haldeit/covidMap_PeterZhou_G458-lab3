# # *Civid-19 Thematic maps*
                - Peter Haoyang Zhou


### This projects contains two thematic maps that shows the intensity of the Covid-19 outbreak that took place in 2020 across the United States
### The first thematic map is a proportional symbol map. This map shows the absolute, total cases in each county with interactive bubbles that contains the state, county, and the number of total recorded cases. Here's a snapshot:
![](./img/map1.png)

### The second thematic map is a choropleth map. This map fills the county polygon with color based on the intensity. The intensity is defined as rate, or the number of cases per 1000 residents. This compares the number of cases in respect to the population. For example, Los Angles may have the highest total number of cases, in respect to its population however it is not near the highest, which is in Colorado.
![](./img/map2.png)

### Both maps starts with **map.on('load')** which loads the data(**map.source**) into the map as well as giving it a name that we will be referencing later. We then specify the number interval spec where we would like to make different color visualizations on our maps. For example, cases vs rates. For the proportional symbol map, we specify the radii to the corresponding interval as we implement the layer in **map.addLayer**. For the choropleth map we simply skip the radii part and replace it as type "fill". **map.on('click')** allow us to customize our interactive panel, where each state, county, and case/rate will be shown. On top of all of these, we have css style in the *style* section.
