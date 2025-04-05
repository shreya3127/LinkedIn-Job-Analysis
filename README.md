Hi :)

This is my end-to-end data project that extracts and analyzes real-world job posting data from LinkedIn to generate key hiring insights and trends. Using a combination of Python (for web scraping and data preparation) and Power BI (for visualization and business intelligence), the dashboard serves as a comprehensive resource for job seekers, recruiters, and HR professionals.

The project reflects real hiring data across Indian cities and job levels, revealing demand patterns, top hiring companies, skill needs, and geographic hiring hotspots.

Finding relevant jobs on platforms like LinkedIn can be overwhelming due to the volume of listings and lack of summarized, structured data. There is no native tool on LinkedIn that helps job seekers or analysts visualize market trends like:
- Which companies are hiring most actively?
- What job levels are in highest demand?
- Which cities offer the most opportunities?
- What industries dominate the hiring landscape?

 This project addresses those gaps by transforming unstructured job listings into actionable insights.

Step-by-Step Breakdown

1. Web Scraping
   - Selenium: Used for automated browser control to simulate logging into LinkedIn and navigating through job search results.
   - BeautifulSoup: Used to extract HTML elements such as job titles, companies, locations, job levels, industry, applicant count, and followers.
   - Pagination Handling: Script loops through multiple job listing pages to collect a wide sample of jobs.
   - Authentication: LinkedIn requires login access, so credentials are securely handled before scraping begins.

Key Scraped Data Fields : Job Title, Company Name, Job Level (Entry, Associate, Executive, etc.), Job Location (City, State), Industry, Number of Applicants, Number of Company Followers


2. Data Cleaning & Transformation
    - Library Used: Pandas
    - Data Quality Handling: Removal of blank, irrelevant, or duplicate records
    - Standardization of city names (e.g., Bengaluru vs. Bangalore)
    - Categorization of job levels and industries
    - Export: Final cleaned dataset exported as LinkedIn_Jobs.csv


3. Dashboard Creation in Power BI

Imported the processed dataset into Power BI and used DAX measures and calculated columns to build insights from the data.

Dashboard Pages & Features:

A. Total Jobs by Level 
- A line chart showing the distribution of jobs across different experience levels.
- A pie chart representing the same data in a percentage format.
- Summary cards: Total Applicants & Total Job Openings
- Filters: Job level, State, City, Company

B. Job Distribution by Geography
- City-Level Tree Map: Cities like Bengaluru, Mumbai, Hyderabad, and Pune stand out as job hubs.
- State Map Visualization: Geolocation data used to map job density state-wise using bubble chart overlays.

C. Company Preferences.
- Company Followers Tree Map: Shows popularity of companies based on their LinkedIn following.
- Jobs by Company bar chart: Top companies currently hiring in different cities and industries.
- Slicers to filter by city, state, industry, and follower count.

D. Role and Industry Analysis.
- Top Job Titles: Analyst, Business Development, Data Analyst, Marketing roles, etc.
- Donut Chart by Industry: Shows IT, Marketing, and Financial services as top hiring sectors.
- KPIs like Total LinkedIn Followers, Job Openings, and Applicant Volume





![image](https://github.com/user-attachments/assets/5accaf58-7ca7-4790-a71b-ff1d632ad0d9)

![image](https://github.com/user-attachments/assets/98f65902-dee9-49f5-b567-a1b2d2cb2a0b)

![image](https://github.com/user-attachments/assets/8b66320f-ea97-4e66-8f89-86d8e31f0d98)

![image](https://github.com/user-attachments/assets/4786bbc5-028c-42f5-adf1-fe4c955075ff)

![image](https://github.com/user-attachments/assets/d2aa55e5-4913-4f27-860d-b7c2d02e6882)


Prerequisites 

- Python 3.x installed on your system
-  Google Chrome browser installed
-  ChromeDriver (version matching your Chrome browser)
-   inkedIn account (valid login credentials.
-    Power BI Desktop installed

Thank you :) 
