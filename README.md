
## Geospatial Analysis for Agricultural Plots and Machinery Utilization - QGIS Plugin

### Project Overview

This project aims to leverage geospatial data collected from farmers' mobile devices to analyze agricultural plots and machinery utilization. The primary goal is to develop a QGIS plugin that seamlessly integrates the obtained data, including plot boundaries and machinery usage records, to provide valuable insights for informed decision-making in the agriculture sector.

### Project Features

1. **Plot Boundaries Processing:**
   - Implement algorithms to process plot boundaries data, enabling the calculation of total plot area and perimeter for each agricultural plot.
   - Utilize advanced geospatial analysis techniques to accurately determine the centroid of each plot.

2. **Visualization and Mapping:**
   - Visualize the plot boundaries and centroids on the map within the QGIS environment for enhanced understanding.
   - Enable users to interact with the map, displaying relevant information on demand.

3. **Machinery Utilization Analysis:**
   - Integrate machinery usage data obtained from farmers' mobile devices into the plugin.
   - Analyze the duration for which machinery is being used on each plot, facilitating insights into machinery utilization patterns.

4. **Aggregate Usage Data:**
   - Aggregate the machinery usage data to estimate the total machinery usage time for different plots.
   - Provide summary statistics and visualizations for better decision-making regarding machinery allocation and usage optimization.

# Geospatial Data Preparation and Attribute-Based Clustering

## Steps

1. **Data Loading**
   - Load the geospatial dataset into the analysis environment to begin the process.

2. **Excel to CSV Conversion and Integration with NQGIS Mapping Tool**
   - Convert the dataset from Excel format to CSV format for better compatibility.
   - Integrate the CSV dataset with the NQGIS mapping tool to enable visualization and mapping.

3. **Formatting the Date-Time Field**
   - Use the Field Calculator to manipulate the date-time field in the dataset.
   - Apply the to_date(whatsspa) function to convert the date-time data into the desired format for analysis.

4. **Attribute-Based Clustering using stDBSCAN Algorithm**
   - Implement the stDBSCAN clustering algorithm for attribute-based clustering.
   - Specify relevant attributes to identify distinct clusters within the dataset.

5. **Polygon Generation - Minimum Bounding Geometry and Convex Hull**
   - Generate minimum bounding geometry to determine the minimum area polygon for each cluster.
   - Calculate the convex hull to obtain the smallest convex polygon enclosing the cluster points.

6. **Attribute Extraction - Area and Perimeter**
   - Retrieve pre-existing attribute information on area and perimeter from the dataset.
   - Utilize this attribute data without requiring additional calculations.

7. **Centroid Calculation using Vector Geometric Tools**
   - Apply vector geometric tools to determine the centroid for each cluster.
   - Calculate the centroid as a representative point that lies at the center of gravity of the cluster.

### Contribution and Feedback

We welcome contributions to this open-source project. If you find any issues or have suggestions for improvements, please submit them through the GitHub repository's issue tracker.

Let's work together to empower farmers with better geospatial insights for efficient agricultural plot management and machinery utilization!
