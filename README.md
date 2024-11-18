Story: https://public.tableau.com/shared/RC478TN4T?:display_count=n&:origin=viz_share_link
Why Tableau: For public access to the dashbboard and interactive features.

#### Data Collection:
Water Contaminants: Voluntary Remediation Program (Indiana IDEM)
Air Contaminants: Air Quality Data (Indiana IDEM)
School Information: School List (NCES)
Hospital Information: Private School List (NCES)
Geolocation Generation:
Some datasets lacked geolocation information. We used a Python script (Geolocation_Generation.ipynb) to generate latitudes and longitudes for schools and hospitals based on their addresses. We have used the Google Maps API for this purpose.
Time Series Analysis:
We applied the ARIMA model to forecast air contaminants' presence over the next 10 years, providing a predictive view of future air quality trends.

#### Data Cleaning:
Standardized column names for consistency.
Transposed rows to columns for year-wise data representation.
Created a "Units" attribute to assign each chemical its respective measurement unit.

Our Indiana Toxicity Watch Dashboard serves as a powerful tool for residents, policymakers, researchers, and environmental advocates, providing a comprehensive, real-time view of the toxic chemical landscape in Indiana. By integrating multiple datasets—from air and water contaminant levels to proximity data for schools and hospitals—our dashboard provides valuable insights into both environmental and public health risks. Here’s how it is useful and why it is a novel contribution:

1. Holistic View of Pollution & Children Health:
Environmental & Health Integration: Unlike traditional environmental monitoring tools that focus solely on air or water quality, our dashboard connects toxic chemical levels with public health risk factors. It helps users not only track pollutant levels but also understand how those levels impact schools allowing for a more complete picture of the environment's effect on children. It also provides a brief view of the common diseases caused by these contaminants.
Proximity Analysis: By visualizing the proximity of schools and hospitals to pollution sources, we provide insights into how vulnerable populations, particularly children, may be exposed to harmful chemicals. This feature is particularly critical for identifying areas where air quality monitoring stations or water contamination efforts are insufficient.
2. Dynamic Data Exploration:
Time Slider for Interactive Analysis: The year slider allows users to explore pollution trends over time. By animating data from 2001 to 2024, users can visually track how the presence of various chemicals has fluctuated in specific areas, giving them an understanding of the temporal changes in air and water quality.
Chemical Filters: The ability to filter data by specific chemicals allows users to dive deeper into the pollution levels of individual chemicals (e.g., SO2, NO2, PM2.5, Ozone) across different years and counties. This feature is valuable for researchers or policymakers who need to focus on particular substances when developing regulations or public health interventions.
3. Forecasting & Predictive Insights:
ARIMA Forecasting: Our dashboard takes predictive modeling a step further by using the ARIMA (AutoRegressive Integrated Moving Average) model to forecast air contaminants’ presence for the next 10 years. This helps users visualize future trends and anticipate potential risks, empowering policymakers to act proactively in improving air quality.
Long-term View of Pollution Trends: By forecasting pollution levels, our dashboard helps decision-makers prepare for future public health concerns, identifying where investments should be made in environmental monitoring, community awareness, and public health interventions.
4. Novelty in Data Integration & Accessibility:
Comprehensive Data Sources: The dashboard aggregates diverse datasets—from the Indiana IDEM (for both air and water contaminants) to school and hospital locations from NCES—into a single, easy-to-navigate platform. This integration of environmental data with health infrastructure is a unique feature that isn’t typically seen in other environmental monitoring tools, offering a more nuanced understanding of how pollution impacts human health.
Missing Data Visualization: We’ve gone a step further to visualize data gaps, such as areas with insufficient chemical monitoring. This transparency is key for informing users about regions where further environmental monitoring and data collection are needed, encouraging more informed decision-making.
5. Interactive and User-Friendly Experience:
Engaging Visualizations: With intuitive visuals such as choropleth maps, heatmaps, and line charts, users can interactively explore air and water quality data at the county, state, or chemical level. These visuals allow users to see the immediate impact of pollution on specific regions and populations, while also providing the ability to zoom into specific areas for a more detailed analysis.
KPIs for Key Insights: The inclusion of key performance indicators (KPIs)—such as the most contaminated counties or the most common air toxins—helps users quickly understand the most critical issues. These KPIs provide a snapshot of pollution levels and contamination hotspots, making the dashboard not only visually appealing but also functionally efficient.
6. Empowering Citizens & Policymakers:
Public Awareness Tool: Our dashboard is designed to be an educational tool, raising awareness about pollution’s impact on health. By providing easy access to pollution data, citizens, students, and community organizations can become better informed and advocate for cleaner air and water in their neighborhoods.
Policy Decision Support: For policymakers, the forecasting model, pollution incident maps, and proximity heatmaps can be critical in formulating effective environmental regulations. This tool equips government officials with insights to make data-driven decisions on pollution control, site remediation efforts, and public health initiatives.

#### Conclusion:
In summary, our Indiana Toxicity Watch Dashboard stands out for its comprehensive data integration, interactive user experience, and predictive insights. It brings together environmental and health data in a way that allows users to not only explore historical and current pollution levels but also forecast future trends, understand the geographic spread of contaminants, and visualize the impact of pollution on sensitive populations like children. By combining scientific rigor with an engaging, accessible interface, this dashboard empowers Indiana's residents and leaders to make informed decisions to safeguard the health of their communities and the environment for years to come.

#### Future Work & Challenges
- Expand Data Sources & Coverage: The dashboard could benefit from monitoring a broader range of chemicals, such as emerging pollutants like microplastics or pharmaceutical residues, which are becoming significant public health concerns. Additionally, integrating more health data—such as asthma rates, respiratory issues, and cancer statistics—would provide a deeper connection between environmental factors and public health outcomes.
- Real-Time Data Integration: Adding real-time air quality data from sensors and government sources would allow the dashboard to offer up-to-date insights on pollution levels. This could help users make immediate, informed decisions. Also, continuous updates on cleanup progress at contamination sites would improve the dashboard's relevance and offer users a more dynamic view of environmental remediation efforts.
Community Engagement & Crowdsourced Data: Introducing a crowdsourced reporting feature would empower local communities to report pollution incidents or sightings, enriching the database with real-time, on-the-ground information. This could help identify pollution sources that aren't captured by formal monitoring stations, leading to a more comprehensive dataset. Collaborative projects could also engage local communities in tracking and combating pollution.

#### Challenges
One of the biggest challenges is ensuring data accuracy and completeness, especially given the gaps in historical pollution data. Many areas may not have consistent monitoring stations, which can leave data gaps in certain regions. Overcoming these gaps, either through enhanced data collection or more robust predictive modeling, will be essential.

Another challenge lies in scaling the dashboard to handle larger datasets and integrate new data sources seamlessly. As more data gets added—such as real-time pollution levels or health data—the dashboard must be able to handle larger volumes of information without compromising performance.

Lastly, while the dashboard provides valuable insights, ensuring that users fully understand and act on this information requires effective communication. Presenting complex environmental and health data in a way that is both accessible and actionable will be key to maximizing its impact.



#### Data Collection:
Water Contaminants: Voluntary Remediation Program (Indiana IDEM)
Air Contaminants: Air Quality Data (Indiana IDEM)
School Information: School List (NCES)
Hospital Information: Private School List (NCES)
Geolocation Generation:
Some datasets lacked geolocation information. We used a Python script (Geolocation_Generation.ipynb) to generate latitudes and longitudes for schools and hospitals based on their addresses, leveraging the Google Maps API for this purpose.
Time Series Analysis:
We applied the ARIMA model to forecast the presence of air contaminants over the next 10 years, providing a predictive view of future air quality trends.

#### Data Cleaning:
Standardized column names for consistency.
Transposed rows to columns for year-wise data representation.
Created a "Units" attribute to assign each chemical its respective measurement unit.

#### Dashboard Features & Utility
Our Indiana Toxicity Watch Dashboard serves as a powerful tool for residents, policymakers, researchers, and environmental advocates, providing a comprehensive, real-time view of the toxic chemical landscape in Indiana. By integrating multiple datasets—from air and water contaminant levels to proximity data for schools and hospitals—our dashboard provides valuable insights into both environmental and public health risks. Here’s how it is useful and why it is a novel contribution:

1. Holistic View of Pollution & Children’s Health:
Environmental & Health Integration: Unlike traditional environmental monitoring tools that focus solely on air or water quality, our dashboard connects toxic chemical levels with public health risk factors. It helps users not only track pollutant levels but also understand how those levels impact schools, providing a complete picture of the environment's effect on children.
Proximity Analysis: By visualizing the proximity of schools and hospitals to pollution sources, we provide insights into how vulnerable populations, particularly children, may be exposed to harmful chemicals. This feature is critical for identifying areas where air quality monitoring stations or water contamination efforts are insufficient.
2. Dynamic Data Exploration:
Time Slider for Interactive Analysis: The year slider allows users to explore pollution trends over time. By animating data from 2001 to 2024, users can visually track how the presence of various chemicals has fluctuated in specific areas, giving them an understanding of temporal changes in air and water quality.
Chemical Filters: The ability to filter data by specific chemicals allows users to dive deeper into the pollution levels of individual chemicals (e.g., SO2, NO2, PM2.5, Ozone) across different years and counties. This feature is valuable for researchers or policymakers who need to focus on particular substances when developing regulations or public health interventions.
3. Forecasting & Predictive Insights:
ARIMA Forecasting: Our dashboard uses the ARIMA (AutoRegressive Integrated Moving Average) model to forecast air contaminants’ presence for the next 10 years. This helps users visualize future trends and anticipate potential risks, empowering policymakers to act proactively to improve air quality.
Long-term View of Pollution Trends: By forecasting pollution levels, our dashboard helps decision-makers prepare for future public health concerns, identifying where investments should be made in environmental monitoring, community awareness, and public health interventions.
4. Novelty in Data Integration & Accessibility:
Comprehensive Data Sources: The dashboard aggregates diverse datasets—from the Indiana IDEM (for both air and water contaminants) to school and hospital locations from NCES—into a single, easy-to-navigate platform. This integration of environmental data with health infrastructure is a unique feature that isn’t typically seen in other environmental monitoring tools, offering a more nuanced understanding of how pollution impacts human health.
Missing Data Visualization: We’ve gone a step further to visualize data gaps, such as areas with insufficient chemical monitoring. This transparency is key for informing users about regions where further environmental monitoring and data collection are needed, encouraging more informed decision-making.
5. Interactive and User-Friendly Experience:
Engaging Visualizations: With intuitive visuals such as choropleth maps, heatmaps, and line charts, users can interactively explore air and water quality data at the county, state, or chemical level. These visuals allow users to see the immediate impact of pollution on specific regions and populations, while also providing the ability to zoom into specific areas for a more detailed analysis.
KPIs for Key Insights: The inclusion of key performance indicators (KPIs)—such as the most contaminated counties or the most common air toxins—helps users quickly understand the most critical issues. These KPIs provide a snapshot of pollution levels and contamination hotspots, making the dashboard not only visually appealing but also functionally efficient.
6. Empowering Citizens & Policymakers:
Public Awareness Tool: Our dashboard is designed to be an educational tool, raising awareness about pollution’s impact on health. By providing easy access to pollution data, citizens, students, and community organizations can become better informed and advocate for cleaner air and water in their neighborhoods.
Policy Decision Support: For policymakers, the forecasting model, pollution incident maps, and proximity heatmaps can be critical in formulating effective environmental regulations. This tool equips government officials with insights to make data-driven decisions on pollution control, site remediation efforts, and public health initiatives.
Conclusion:
In summary, the Indiana Toxicity Watch Dashboard stands out for its comprehensive data integration, interactive user experience, and predictive insights. It brings together environmental and health data in a way that allows users to explore historical and current pollution levels, forecast future trends, understand the geographic spread of contaminants, and visualize the impact of pollution on sensitive populations like children. By combining scientific rigor with an engaging, accessible interface, this dashboard empowers Indiana's residents and leaders to make informed decisions to safeguard the health of their communities and the environment for years to come.

#### Future Work
Expand Data Sources & Coverage: The dashboard could benefit from monitoring a broader range of chemicals, such as emerging pollutants like microplastics or pharmaceutical residues, which are becoming significant public health concerns. Additionally, integrating more health data—such as asthma rates, respiratory issues, and cancer statistics—would provide a deeper connection between environmental factors and public health outcomes.
Real-Time Data Integration: Adding real-time air quality data from sensors and government sources would allow the dashboard to offer up-to-date insights on pollution levels. This could help users make immediate, informed decisions. Also, continuous updates on cleanup progress at contamination sites would improve the dashboard's relevance and offer users a more dynamic view of environmental remediation efforts.
Community Engagement & Crowdsourced Data: Introducing a crowdsourced reporting feature would empower local communities to report pollution incidents or sightings, enriching the database with real-time, on-the-ground information. This could help identify pollution sources that aren't captured by formal monitoring stations, leading to a more comprehensive dataset.

#### Challenges
Data Accuracy & Completeness: One of the biggest challenges is ensuring data accuracy and completeness, especially given the gaps in historical pollution data. Many areas may not have consistent monitoring stations, which can leave data gaps in certain regions. Overcoming these gaps, either through enhanced data collection or more robust predictive modeling, will be essential.
Scaling the Dashboard: Another challenge lies in scaling the dashboard to handle larger datasets and integrate new data sources seamlessly. As more data gets added—such as real-time pollution levels or health data—the dashboard must be able to handle larger volumes of information without compromising performance.
Effective Communication: While the dashboard provides valuable insights, ensuring that users fully understand and act on this information requires effective communication. Presenting complex environmental and health data in a way that is both accessible and actionable will be key to maximizing its impact.
