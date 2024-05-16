# COVID-19 Time Series Analysis

## Installation

To run the project, you'll need to have the following Python packages installed. You can install them using the following command:

```bash
pip install scikit-learn pandas numpy statsmodels matplotlib seaborn plotly prophet
```

## About Dataset
<center><img src=https://openwho-public.s3.openhpicloud.de/courses/54f2X1Vho0GytsuIynhQmH/visual_v7.PNG></center>

### Context
The emergence of the novel coronavirus, officially designated as 2019-nCoV, marked a significant turning point in global health. Originating in Wuhan, the capital city of Hubei province in China, the virus presented an unprecedented challenge due to its mysterious nature and rapid spread. Individuals began exhibiting symptoms of pneumonia, characterized by respiratory distress, without a clear cause, and existing vaccines or treatments proved ineffective against the novel pathogen. Alarming reports indicated evidence of human-to-human transmission, raising concerns about the potential for widespread contagion. By mid-January 2020, the transmission rate, reflecting the rate of infection, had surged, triggering heightened alerts across international health organizations. As of January 30, 2020, the situation had escalated dramatically, with approximately 8,243 confirmed cases reported, underscoring the urgency for coordinated global efforts to contain the outbreak and develop effective strategies for prevention and treatment.


### Features
The dataset contains number of Confirmed, Death and Recovered cases every day across the globe.

| Feature        | Description                                                                                                                          |
|----------------|--------------------------------------------------------------------------------------------------------------------------------------|
| Province/State | The name of the province or state where the Covid-19 cases were reported.                                                            |
| Country/Region | The name of the country or region where the Covid-19 cases were reported.                                                            |
| Lat            | The latitude coordinate of the location where the Covid-19 cases were reported.                                                      |
| Long           | The longitude coordinate of the location where the Covid-19 cases were reported.                                                     |
| Date           | The date when the Covid-19 cases were reported.                                                                                      |
| Confirmed      | The number of confirmed Covid-19 cases reported in the specified province/state or country/region.                                   |
| Deaths         | The number of deaths attributed to Covid-19 reported in the specified province/state or country/region.                              |
| Recovered      | The number of recovered Covid-19 cases reported in the specified province/state or country/region.                                   |
| Active         | The number of active Covid-19 cases (confirmed cases minus deaths and recoveries) in the specified province/state or country/region. |
| WHO Region     | The World Health Organization (WHO) region to which the province/state or country/region belongs.                                    |


### Project Target
- Country-wise exploration of the data.
- Analysis of the trends in the active, deaths, confirmed and recovered cases.
- Find the top 20 countries for active, deaths, confirmed and recovered cases.
- Build a time series model to uncover underlying trends and seasonality of the data.
- Forest active, deaths, confirmed and recovered cases for the next 7 days using the model.
- Interpret the findings from the model.

### Algorithms Implemented
- Facebook Prophet

### Inferences
On visual inspection of the plots provided by the Prophet library we make these inferences:
- **Upward Trend:** The upward trend observed in all attributes, including confirmed cases, deaths, active cases, and recovered cases, indicates a continuous rise in the impact of COVID-19 globally. It suggests that the spread of the virus is not slowing down, and the situation is evolving rapidly.
- **Weekly Seasonality:** The presence of a distinct weekly seasonality, resembling a sine wave, with a minima around Monday-Tuesday and a maxima around Friday-Saturday is noteworthy.
<br>

**Thoughts on weekly seasonality:** The observed weekly seasonality in COVID-19 attributes can be rationalized based on human behaviour, societal patterns, and reporting dynamics:
- **Workweek Impact:** The lower counts at the beginning of the week may be influenced by reduced testing, reporting delays, or decreased social activities during the early workweek. Similarly, the higher counts towards the end of the week could be linked to increased testing, more social interactions, and potentially delayed reporting catching up from earlier in the week.
- **Testing Patterns:** Variations in testing availability and practices might contribute to the observed weekly patterns, with increased testing leading to higher reported cases.
- **Reporting Delays:** Delays in data reporting, especially over weekends, might result in a surge of reported cases at the beginning of the new week.
- **Weekend Gatherings:** Social activities, gatherings, or events over the early weekend might contribute to increased exposure and transmission, leading to higher reported cases.
- **Workweek Caution:** Individuals might exhibit more caution and adherence to safety measures early in the workweek, potentially influencing lower reported cases. However, as the week progresses, there appears to be a relaxation in this vigilance, potentially leading to a more casual approach to safety protocols.

## Reference
[COVID-19 Data Repository](https://github.com/CSSEGISandData/COVID-19) by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University: On March 10, 2023, the Johns Hopkins Coronavirus Resource Center ceased its collecting and reporting of global COVID-19 data. For updated cases, deaths, and vaccine data please visit the following sources:<br>

- Global: [World Health Organization (WHO)](https://www.who.int/)
- U.S.: [U.S. Centers for Disease Control and Prevention (CDC)](https://www.cdc.gov/coronavirus/2019-ncov/index.html)
For more information, visit the [Johns Hopkins Coronavirus Resource Center.](https://coronavirus.jhu.edu)

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT) - see the [LICENSE](https://github.com/soumyadeepghoshGG/COVID-19-Time-Series-Analysis/blob/main/License.txt) file for details.

## Contact
For questions or issues, please contact me (Soumyadeep Ghosh) via mail: soumyadeepghosh57@gmail.com