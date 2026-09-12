# Projects
This section documents my data science projects, research questions, and data stories I create throughout the semesters.
## Project 1

## MLB Pitch Effectiveness — 2026

**Research Question:**
Which MLB pitch types are most effective at limiting offensive production during the 2026 MLB season?

### Overview

For this project, I analyzed MLB Statcast data from Baseball Savant to investigate how different pitch types performed during the 2026 MLB season-to-date.

The analysis focused on eight major pitch types:

* 4-Seam Fastball
* Sinker
* Slider
* Changeup
* Sweeper
* Cutter
* Curveball
* Split-Finger

### Effectiveness Score

To compare pitch types, I created an Effectiveness Score using six different measures:

* Run value per 100 pitches
* Whiff rate
* wOBA
* Expected batting average (xBA)
* Average exit velocity
* Hard-hit rate

The metrics were standardized using z-scores and combined into one score. A higher score represents better overall effectiveness.

### Results

The changeup had the highest average Effectiveness Score among the eight pitch types analyzed, followed by the split-finger and sweeper. The sinker had the lowest average Effectiveness Score, while the four-seam fastball also ranked below the overall average.

![Average Effectiveness Score by Pitch Type](effectiveness_score.png)

The chart above shows the average Effectiveness Score for each pitch type. Positive scores represent above-average effectiveness, while negative scores represent below-average effectiveness.

The heatmap below shows how each pitch type performed across the individual metrics used to calculate the Effectiveness Score.

![Pitch Type Performance Heatmap](pitch_heatmap.png)


### Data

The data came from MLB Statcast through Baseball Savant and represents the **2026 MLB regular season through September 2, 2026**.

The final analysis included **535 pitcher–pitch type observations** across the eight pitch types.

### Limitations

The 2026 season was still in progress when the data was collected, so the results may change by the end of the season.

The Effectiveness Score is also a descriptive measure created specifically for this project and is not an official MLB statistic. Because the analysis is observational, the results show differences between pitch types but do not prove that a specific pitch type causes better or worse offensive outcomes.

### What I Learned

This project gave me experience collecting and cleaning real-world baseball data, working with pandas, creating visualizations, and combining multiple statistics into a single analytical measure. It also helped me understand some of the challenges involved in using sports data, including missing values, differences in sample sizes, and deciding how to operationalize a broad concept like pitch effectiveness.

