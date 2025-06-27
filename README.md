# FUTURE_DS_02
PROJECT TITLE: Marketing Campaign Click-Through Rate (CTR) Analysis Dashboard
Overview:
This Power BI dashboard provides a comprehensive analysis of marketing campaign performance, with a specific focus on understanding Click-Through Rate (CTR) across various demographic segments and interest groups. The dashboard aims to offer actionable insights into which audience segments respond most effectively to marketing efforts, enabling data-driven optimization strategies.
Problem Addressed:
Marketing campaigns often generate vast amounts of data. Without proper analysis, it's challenging to identify high-performing segments or areas needing improvement. This project addresses the need for a clear, interactive visualization tool to pinpoint key drivers of CTR and inform future campaign targeting.
Key Features & Visualizations:
 * Click-Through Rate (CTR) Calculation:
   * A custom measure for CTR was created: CTR = DIVIDE(SUM(Clicks), SUM(Impressions)). This ensures accurate calculation of engagement for all analyses.
 * CTR by Gender:
   * A column chart visualizes CTR performance segmented by gender (Male/Female). This chart was specifically engineered to correctly display "M" and "F" categories on the X-axis, resolving an initial display anomaly where numerical representations appeared.
 * CTR by Age Group:
   * A column chart illustrates CTR trends across various age groups. Similar to the gender analysis, this chart was configured to accurately represent age ranges (e.g., "30-34", "45-49") on the X-axis, ensuring clear categorical representation.
 * CTR by Interest Categories (Interest 1, Interest 2, Interest 3):
   * Three separate column charts provide insights into CTR for distinct interest categories (interest1, interest2, interest3).
   * Initial challenges with automatic numerical summarization of interest values on the Y-axis were overcome by explicitly setting the default summarization behavior of these fields to "Don't summarize" in the Power BI data model. This ensured that individual interest values are displayed as distinct categories on the X-axis, with their corresponding CTRs on the Y-axis.
Technical Implementation:
 * Data Import & Transformation: Data was imported into Power BI Desktop. Initial transformations were performed to ensure data quality and correct typing of columns (e.g., gender as Text, age as Text categories).
 * Measure Creation: DAX (Data Analysis Expressions) was used to create the CTR measure.
 * Visual Configuration: Extensive configuration of chart properties, including X-axis and Y-axis settings, was performed to ensure correct visual representation of categorical data and prevent unintended numerical aggregation on the axes. The "Don't summarize" feature was critical for accurate display of categorical fields.
How to Use:
To explore this dashboard, download the marketing campaign dashboard.pbix file and open it using Power BI Desktop. The interactive charts allow for quick visual analysis of campaign performance across key demographics and interests.
Technologies Used:
 * Microsoft Power BI Desktop
