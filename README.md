
# 2022 T20_World_Cup Analysis -Report



## Problem Statement

In the highly competitive landscape of T20 cricket, selecting the best players and analyzing individual performance are critical for success od the team. However, the process of identifying top-performing players is often subjective and inconsistent. 

This project aims to address these challenges by leveraging key performance indicators (KPIs) to empower anyone to make data-driven decisions for selecting the best 11 players. Additionally, it provides a detailed analysis of individual player performance.


### Steps followed 

- Step 1 : Web Scraping

           a) For collecting real-time data from ESPNcricinfo website, Bright Data tool was used.
           b) Then, identifying and targeting the required data endpoints on ESPNcricinfo.
           c) Implementing Scraping script(javascript) in Interactive Code and Parser code editor.
           d) Collected data was stored in 'json' format.
           e) Four scrapers were made in Bright Data, each for match_summary, batting_summary, bowling_summary, players_summary.
- Step 2 : Data Collection

      The data through four web scrapers were collected in
             match_results: Contains results of matches.
             batting_summary: Summarizes batting performances.
             bowling_summary: Summarizes bowling performances.
             players_summary: Provides detailed player statistics.
      
- Step 3 : Data Transformation and Cleaning

          a) For converting raw JSON data into clean and actionable CSV files, jupyter notebook is used.
          b) After importing pandas and json libraries, the four json files were converted to pandas dataframe for some data cleaning tasks.
          c) A match_ids_dict dictionary was created to link match_results table with batting_summary table, bowling_summary table.
          d) In match_summary dataframe, 'scorecard' column was renamed to 'match_id'.
          e) In batting_summary dataframe, new column named: 'out/not_out' was created based on dismissal column.Afterwards, 'dismissal' column was drop.
          f) Some data cleaning task was also performed in 'batsmanName' column.
          g) Above step was also performed for 'name' column in players dataframe.
          h) The four dataframes were converted into csv formats.

- Step 4 : Before going for data visualization step in Power BI, I created image column in players CSV file to add images of some selected players.
- Step 5 : Then interactive and insightful report was created in Power BI.

         a) A folder containing all csv files were loaded for transforming data in power Bi query editor.
         b) The folder was duplicated three times and names were changed.
         c) In match_summary, conditional column : 'stage' was added.
         d) In bowling_summary, overs column was splitted along delimter: '.'
         e) Then after doing all necessary changes, data was load in Power Bi Desktop.
         f) In players_summary table, 'Custom Batting Order' column was added.
         g) In wc_batting_summary and wc_bowling_summary, 'Boundary Runs' column was added.
         h) In wc_match_summary, 'Team 1 code','Team 2 code' and 'match' column was created.
         i) In model view, wc_batting_summary and wc_bowling_summary table were connected to players_summary table through merging batsmanName and bowlerName in name column of players_summary.
         j) Various New Measures were also created like, Batting Average, Batting S/R, Economy,Wickets and many more.
         h) For effective selection of players, different pages for Power Hitters, Middle Order, Finisher, All Rounder, Specialist Fast Bowler were made.
         i) Players details by match, Finisher/All Rounder details by match,fast bowlers details by match were also created to use them as [tooltip].
  Snap of New Measures
      ![image](https://github.com/user-attachments/assets/88861ba7-b890-4dcb-a69a-f33b0803ca0f)
  





 
 # Report Snapshot (Power BI DESKTOP)
 
![image](https://github.com/user-attachments/assets/96285930-c74e-408b-b2b4-d0c3e033ddbc)



# 2022 T20_World_Cup Analysis -Report.md.txt
Displaying # 2022 T20_World_Cup Analysis -Report-Dashboard.md.txt.

