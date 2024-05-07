---
layout: post
title:  "Final Project Presentation"
---
#### Group Member: You Peng, Veeresh Kande, Mengke Wu, Prathyush Bhamidipati

# Introduction

**Name:** Enrollment Database

**Source:** New York State Education Department (NYSED)

**Overview:** 4 datasets inside the package, each focuses on an aspect of the enrollment and can be joined by corresponding keys

**Time:** 2021 to 2023

**Details:**

- `BEDS Day Enrollment.csv` - enrollment numbers by grades in each school for 3 years;
- `BOCES and N:RC.csv` - category and location information for each school for 3 years;
- `Demographic Factors.csv` - demographic information for each school for 3 years;
- `Institution Grouping.csv` - group information for each school;

**Goal:** This data amalysis aims to examine trends or differences in enrollment, demographic factors, and school distributions within New York State (NYS) schools over the three-year period from 2021 to 2023. This analysis will provide valuable information for education policymakers, school administrators, researchers, and analysts interested in understanding dynamics of school enrollment and its implications for educational planning and resource allocation.

## Plot Topic 1 - Enrollments

The first topic in the analysis is the information on the enrollment number in NYS.

### 1.1 General Enrollment

<iframe src="https://youpeng0630.github.io/445final/image/Sum_of_Enrollment.jpg" width="100%" height="450"></iframe>


The plot shows the enrollment trend by year, with the x-axis indicating the year while the y-axis is the sum of enrollment. From the plot we can see, the total number of enrolled students has shown a consistent decrease from 2021 to 2023.

<iframe src="https://youpeng0630.github.io/445final/image/Enrollment_by_Grade.jpg" width="135%" height="450"></iframe>


If we divide the enrollment by grades, we can see that the enrollments varies by grade across the 3 years, with Grade 9 consistently reaching the peak in enrolling students. Meanwhile, the enrollments from Grade 1 to Grade 9 are overall increase then decrease from Grade 9 to Grade 12 in all 3 years.

### 1.2 Enrollment by NYS County across Years**

<iframe src="https://youpeng0630.github.io/445final/enrollment_trends_by_grade.html" width="140%" height="480"></iframe>

This plot shows the nrollment information by NYS counties and by year. The x-axis is each grade while the y-axis is the enrollment of that grade. The dropdown menu in the bottom left corner enables us to select certain county in certain year to see the enrollment of each grade in that year. If hovering on the bar, details such as county name, year, grade, and sum of students will display.

If diving deeper into different NYS counties, the trend of enrollment is mostly align with the general trend showed in section 1.1 but some conflicted patterns occur. For example, Allegany enrolled the most student in Grade 1 in 2022, and the Grade 9 enrollments in Hamilton across all the 3 years are not the most and even the least in 2022 

## Plot Topic 2 - Demographics of Enrolled Students

Among the enrolled students, demographics should be an important part to explore, especially the gender and race distribution.

### 2.1 Gender Dsitribution

<iframe src="https://youpeng0630.github.io/445final/gender.html" width="90%" height="500"></iframe>

From this plot, we can seek insights into the distribution of genders by year from 2021 to 2023. The x-axis of this bar chart is the gender type while the y-axis is the percentage of that gender. The dropdown menu in the bottom left corner enables us to select certain year to see the percentage distribution of enrolled students with different genders in that year. If hovering on the bar, detailed percentage data will show. By switching among years, we can also explore the changes or trends across different years of the gender distribution.

From the plot we can see, the gender distribution has remained relatively stable across the 3 years, with the percentage of females (~ 48.5%) consistently lower than males (~ 51.5%), which indicates a slight inbalance.

### 2.2 Race Dsitribution

**2.2.1 General Race Dsitribution by Year**

<iframe src="https://youpeng0630.github.io/445final/race.html" width="100%" height="650"></iframe>

From this plot, we can seek insights into the distribution of races by year from 2021 to 2023. Similar to the gender distribution plot in section 1.1, the x-axis of this bar chart is the race type while the y-axis is the percentage of that race. This plot also includes a dropdown menu, as well as the hover details, that enables the selection of certain year to see the detailed race distribution in that year.

The percentages of each race have also remained relatively stable across the 3 years, with white students always comprising the largest percentage (~ 46.5%) followed by Hispanic or Latino (~ 26.0%), Black or African American (~ 16.0%), Asian or Native Hawaiian/Other Pacific Islander (~ 7.0%), Multiracial (~ 3.0%), and American Indian or Alaska Native (~ 1%).

**2.2.2 Race Dsitribution by New York State Counties**

<iframe src="https://youpeng0630.github.io/445final/log_NUM_BLACK.html" width="100%" height="600"></iframe>
<iframe src="https://youpeng0630.github.io/445final/log_NUM_ASIAN.html" width="100%" height="600"></iframe>
<iframe src="https://youpeng0630.github.io/445final/log_NUM_WHITE.html" width="100%" height="600"></iframe>

The series of plots geographically shows the distribution across counties of students from 3 races: White, Asian, and Black. The color bar on the right illustrates a density of students, with a higher position in the bar (brighter yellow) indicating higher density and a lower position in the bar (darker purple) indicating lower density.

Zooming on each county, first, we can interpret from the color bar that, the general pattern for race distribution corresponds to the one in section 2.2.1 that White students reach the yellow color in the bar, indicating more students; while Asian and Black students are displayed by the middle or low colors, indicating a lower quantity of students.

Then, from the geographical color patterns, if hovering we can discover some detailed information. For example, Hamilton consistently has the lowest student amounts across the 3 races since it has the darkest color in all 3 maps. Conversely, the New York City area always shows the brightest color across 3 maps, indicating it has the most amount of students from all 3 races.

## Plot Topic 3 - School Distribution

In addition to students, we also investigated the information about the schools themselves.

### 3.1 School Dsitribution by Need/Resource Category

First, we explored the distribution of schools falled into different need to resource capacity by years. The need/resource capacity index is a measure of a district's ability to meet the needs of its students with local resources, pointing to the ratio of the estimated poverty percentage to the Combined Wealth Ratio. The detailed category descriptions are below:

- **High N/RC: New York City** - New York City
- **High N/RC: Large City Districts** - Buffalo, Rochester, Syracuse, Yonkers
- **High N/RC: Urban-Suburban Districts** - All districts at or above the 70th percentile (1.1835) that have: (1) at least 100 students per square mile; or (2) an enrollment greater than 2,500 and more than 50 students
per square mile.
- **High N/RC: Rural Districts** - All districts at or above the 70th percentile (1.1835) that have: (1) fewer than 50 students per square mile; or (2) fewer than 100 students per square mile and an enrollment
of less than 2,500.
- **Average N/RC Districts** - All districts between the 20th (0.770) and 70th (1.1835) percentile on the index.
- **Low N/RC Districts** - All districts below the 20th percentile (0.770) on the index.
- **Charter Schools** - Charter Schools

<iframe src="https://youpeng0630.github.io/445final/image/Sum_of_Enrollment.jpg" width="110%" height="450"></iframe>
The plot shows the school counts by year in each need/resource category, with the x-axis indicating the category while the y-axis the school counts. From the plot we can see that the school counts by need/resource category across the 3 years are nearly the same. Among them, NYS has the largest number of Public Schools (~ 1600), followed by Average Need Districts (~ 1350), Low Need Districts (~ 600), and High Need/Resource Rural Districts (~ 350).

**3.1.1 Gender Dsitribution by Need/Resource Category**


<iframe src="https://youpeng0630.github.io/445final/image/Gender_by_NRC.jpg" width="150%" height="450"></iframe>


Directing back to gender and diving into the need/resource categories, we can see that the gender distribution by category shows a similar pattern across the 3 years within each school category. Across the 7 categories, male enrolled students are mostly higher than that of female students, except for Charter Schools, where the percentage of males is slightly lower than females.



<iframe src="https://youpeng0630.github.io/445final/image/Gender_by_NRC_2023.jpg" width="140%" height="450"></iframe>

In the detailed figure onlye for year 2023, the gender distribution by need/resource category is similar to the overall 3-year trend. Moreover, as can be seen in this magnified coordinate, the gender gap (males > females) is largest in NYC Public Schools, while the opposite is true (males < females) only in Charter Schools.

### 3.2 School Distribution by NYS Counties**

This section explores the distribution of schools across various NYS counties. From pre-examination, the school counts for each county are quite similar across the 3 years, so we just take 2023 as the example to demostrate as plots.

<iframe src="https://youpeng0630.github.io/445final/school_count.html" width="160%" height="500"></iframe>

The plot above presents the overall distribution of schools by each counties in NYS. The x-axis is the list of NYS counties in alphabetical order and the y-axis is the school count. The default display of all bars are fade out. By clicking on 1 certain bar representing a county's school count, the selected bar will be highlighted as blue and the exact amount of schools in that county will show. This interaction gives more details for the school distribution across NYS counties in 2023.

We can see that the counties at NYS that have the most schools in 2023 are Kings (555), Bronx (442), and Queens (371).

<iframe src="https://youpeng0630.github.io/445final/youpeng.html" width="150%" height="600"></iframe>

More specifically, beyond presenting the school counts across counties for the year 2023. An additional feature, an interactive slider, is embedded in the plot above.  Each county is distinguished by a unique color for the purpose of better visual differentiations. If dragging to create a rectangular on the slider that covers a certain range of school numbers, only counties have schools within that range will be displayed on the plot. This selection tool enable us to discover the concentration of educational institutions in different areas of the city at a glance.



<button onclick="loadData1()">Reload BEDS Day Enrollment.csv</button>
<button onclick="loadData2()">Reload BOCES_and_N_RC.csv</button>
<button onclick="loadData3()">Reload Institution_Grouping.csv</button>
<button onclick="loadData4()">Reload Demographic_Factors.csv</button>

<div id="display"></div>

<script>
async function loadData1() {
    await fetchData('https://youpeng0630.github.io/445final/BEDS_Day_Enrollment.csv');
}

async function loadData2() {
    await fetchData('https://youpeng0630.github.io/445final/BOCES_and_N_RC.csv');  // Modify URL for your second CSV
}

async function loadData3() {
    await fetchData('https://youpeng0630.github.io/445final/Institution_Grouping.csv');  // Modify URL for your third CSV
}

async function loadData4() {
    await fetchData('https://youpeng0630.github.io/445final/Demographic_Factors.csv');  // Modify URL for your fourth CSV
}

async function fetchData(url) {
    const response = await fetch(url);
    const data = await response.text();
    const rows = data.split('\n').map(row => row.split(','));
    displayData(rows);
}

function displayData(rows) {
    const container = document.getElementById('display');
    container.innerHTML = '<table>' + rows.map(row => `<tr>${row.map(cell => `<td>${cell}</td>`).join('')}</tr>`).join('') + '</table>';
}
</script>

<style>
table, td, th {
    border: 1px solid black;
    border-collapse: collapse;
    padding: 5px;
    text-align: left;
}
</style>


`Link for show ipynotebook analysis in git hub`
<a href="https://github.com/YouPeng0630/445final/blob/main/IS445_project.ipynb" class="btn">Analysis Notebook</a>


[jekyll-docs]: https://jekyllrb.com/docs/home


---