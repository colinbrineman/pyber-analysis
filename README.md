    Deliverable 3: A written report for the PyBer analysis (20 points)
    Deliverable 3 Instructions
    Use your repository README file to write your analysis of how to address any disparities in the ride-sharing data among the city types.

    The analysis should contain the following:

    Overview of the analysis: Explain the purpose of the new analysis.
    Results: Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types.
    Summary: Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.
    Deliverable 3 Requirements
    Structure, Organization, and Formatting (6 points)
    The written analysis has the following structure, organization, and formatting:

    There is a title, and there are multiple sections. (2 pt)
    Each section has a heading and subheading. (2 pt)
    Links to images are working and displayed correctly. (2 pt)
    Analysis (14 points)
    The written analysis has the following:

# Module 5 Challenge: Analyzing and Visualizing Ridesharing Data Using Pandas and Matplotlib
#### Colin Brineman, M.A.

## Overview
The purpose of this project is to analyze and visualize data from a ridesharing company called PyBer. PyBer wishes to understand the differences between its performance in three city types (rural, suburban, or urban), so that they can develop a strategy for improving their position in each geographic market. Using Pandas, I have grouped PyBer data by city type and calculated summary statistics from three metrics (rides, drivers, and fares). Using Matplotlib, I have created a line graph showing PyBer's weekly fares accumulated from January through April 2019, across the three city types.

## Results

#### Fig. 1: PyBer Summary Statistics
![Fig. 1: PyBer Summary Statistics](/analysis/PyBer_DataFrame.png)

Total rides, total drivers & total fares are correlated with density (i.e., each metric is highest in urban areas and lowest in rural areas, with suburban areas in between).

Average fares per ride and average fares per driver are inversely correlated with density (i.e., each metric is highest in rural areas and lowest in urban areas).

Nothing about this is particularly surprising. Considering rural areas:
- fewer people live in rural areas, so there are fewer drivers,
- and people also live further apart, making ride distances longer.
We could expect both of these factors to increase average fares per ride & average fares per driver. Yet, while average fares are higher, PyBer still doesn't get very much revenue from rural areas, because there simply aren't as many customers in those areas.

For urban areas, consider every factor outlined above, but in reverse, and suburban areas split the distance between the two geographies.

#### Fig. 2: Pyber Fares by Month (2019)
![Fig. 2: Pyber Fares by Month (2019)](/analysis/PyBer_fare_summary.png)

A graphical analysis of total fares over a fairly large slice of our data does not provide much additional insight, as compared to the summary statistics cited above. PyBer makes the most money in urban areas, the least in rural areas, and somewhere in between in suburban areas. The relative performance of these geographies may differ over the course of the year, but not in any way which I can clearly tease out. I would suspect what variation exists is more or less indistinguishable from noise.

## Recommendations

Based on the above analysis, I would make the following recommendations to PyBer's CEO:
1. Advertise more in suburban areas which closely adjoin urban areas. The advantages of more urban drivers means that customers shouldn't have too hard of a time getting a ride in the early phases of a suburban push, but the rides would tend to be longer and thus the fares larger, making urban/suburban border areas the sweetspot for expanded market penetration.
2. Identify lucrative rural routes. While PyBer will never do as much business in rural areas as in urban areas, there are clearly rural customers for PyBer's ridesharing service. What PyBer needs to figure out, is who these customers are and where they are going. Since there are fewer drivers in rural areas and wait times must be long, it's a good guess that these are customers who have a strong attachment to PyBer's service. PyBer should identify other rural customers who may be similarly situated.
3. Communicate to urban drivers the opportunities available in other geographies. The average fare per driver is more than 3x as high in suburban areas vs. urban areas — and more than 12x as high in rural areas! There is a demand for PyBer's services in other geographic regions than cities, but if PyBer cannot ensure enough drivers in these areas, then it runs the risk of falling out of use. From a driver's perspective, there is better income to be had in rural and suburban areas. If PyBer can communicate this opportunity to its drivers, then the situations is win–win–win for investors, drivers, and customers alike.