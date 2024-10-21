## CognoRise-Infotech
DATA ANALYST NAME: EME JOY UCHENNA.
ORGANISATION: CognoRise INFOTECH
POSITION: POWER BI AND TABLEAU INTERN
## TASK 1: TOP SPOTIFY SONGS 2023.
## TOOLS: EXCEL, POWER BI, TABLEAU.
Data Acquisition
-	Platform: Kaggle
-	Format: CSV, converted to Excel for analysis
  ## Data Preparation for Spotify Songs Analysis
  ### USNG TABLEAU
  ## Data Cleaning
- Removed Empty Values, Identified and eliminated any rows with missing data to ensure complete datasets.
  ## Removed Duplicates
-  Scanned and removed duplicate entries to maintain data integrity and accuracy.
- Replaced Errors with Zero: Addressed erroneous data points by replacing them with zeros, preventing calculation issues.
  ##  Data Transformation
- Added Index Column, Introduced a unique identifier for each row, facilitating easier data management and analysis, particularly for finding percentiles, ranks, or organizing data.
- Created 'TREND STATUS' Column; Introduced a new column to indicate if a song was trending or not. This was based on the average stream count calculated as 468.41M streams.
  ## Data Wrangling
- Calculated Average Streams, Computed the average number of streams, setting a benchmark to determine the 'trending' status for each song.
- Organized Data: Renamed column headers and arranged the dataset in a logical and intuitive format, enhancing readability and analytical capabilities.
  ## FORMULAS USED.
   ### DAX Formulas and Their Representations.
  
  1. Sum of Apple Playlists
     - ## SUM('SPOTIFY 2023'[apple playlists])
     - Purpose: Calculates the total number of Apple playlists for songs.
       
  2. Month Name Conversion
     - ## Date.MonthName([released_month] * 29)
     - Purpose: Converts the month number to the month name.

  3. Calculate Average
     - ## AVERAGE(TableName[STREAMS])
     - Purpose: Calculates the average number of streams.

  4. Count of Text Values
     - ## COUNTA(TableName[ColumnName])
     - Purpose: Counts the number of text values in a specified column.

  5. Sum of Numeric Values
     - ## Total Sales = SUM(Sales[SalesAmount])
     - Purpose: Sums up the numeric values in the specified column.
       
  6. Unique Word Count
     - ## COUNTROWS(VALUES(TABLENAME[WORDCOLUMN]))
     - Purpose: Counts the number of unique text values in the specified column.
       
  7. Count of Unique Artists
     - ## COUNTROWS(VALUES('SPOTIFY 2023'[artist(s) name]))
     - Purpose: Counts the number of unique artists.

  8. Sum of Deezer Playlists
     - ## SUM('SPOTIFY 2023'[deezer playlists])
     - Purpose: Calculates the total number of Deezer playlists for songs.

9. Sum of Spotify Playlists
     - ## SUM('SPOTIFY 2023'[spotify playlists])
     - Purpose: Calculates the total number of Spotify playlists for songs.

10. Total Streams
     - ## SUM('SPOTIFY 2023'[streams])
     - Purpose: Calculates the total number of streams.

11. Total Tracks
     - ## COUNTA('SPOTIFY 2023'[track name])
     - Purpose: Counts the total number of tracks.     

## Power BI Setup for Visualization.
1.	Installation: Fresh Power BI installation on a new laptop

### Visualizations.
1.	Total Streams by Track
    Type:  CLUSTERED BAR CHARTS
- #### Purpose: Identify tracks with the highest streams across all apps.
  
2.	MUSIC METRICS; STREAMS VS DANCEABILITY AND BPM
    Type: STACKED COLUMN CHARTS
- #### PURPOSE: TO IDENTIFY TRENDS IN HOW DANCEABILITY AND BPM IMPACT THE STREAMING SUCCESS OF SONGS ON SPOTIFY.
  
3.  MUSIC METRICS; LIVELINESS VS ENERGY
    Type: STACKED COLUMN CHARTS
- #### PURPOSE: TO IDENTIFY TRENDS IN HOW LIVELINESS AND ENERGY IMPACT THE STREAMING SUCCESS OF SONGS ON SPOTIFY.
  
4.  MUSIC METRICS; VALECE INSTRUMENTALNESS AND ACOUSTICNESS.
    Type: STACKED COLUMN CHARTS
- #### PURPOSE: TO IDENTIFY TRENDS IN HOW  VALECE INSTRUMENTALNESS AND ACOUSTICNESS IMPACT THE STREAMING SUCCESS OF SONGS ON SPOTIFY.

5.  5 MOST STREAMED ARTIST.
    Type: CLUSTERED BAR CHARTS
- #### PURPOSE: HELPS TO SPOT PATTERNS IN LISTENER PREFERENCES, SUCH AS WHAT TYPE OF MUSIC OR WHICH GENRES ARE CURRENTLY POPULAR OR DECLINING.

6.  5 LEAST STREAMED ARTIST.
    Type: CLUSTERED BAR CHARTS
- #### PURPOSE: HELPS TO SPOT PATTERNS IN LISTENER PREFERENCES, SUCH AS WHAT TYPE OF MUSIC OR WHICH GENRES ARE CURRENTLY POPULAR OR DECLINING.

7.  5 TOPPING ARTIST ANALYSIS.
   Type: STACKED COLUMN CHART
- #### PURPOSE: TO IDENTIFY AND COMPARE STREAMING TRENDS AND PATTERNS ACROSS DIFFERENT PLATFORMS FOR THE TOP 5 MOST-STREAMED ARTISTS.

8.  5 UNDERPERFORMING ARTIST ANALYSIS.
   Type: STACKED COLUMN CHART
- #### PURPOSE: TO IDENTIFY AND COMPARE STREAMING TRENDS AND PATTERNS ACROSS DIFFERENT PLATFORMS FOR THE 5 UNDERPERFORMING ARTIST.

9.  YEARLY STREAM TRENDS BY ARTIST.
    Type: CLUSTERED BAR CHART, SLICER FOR YEAR
  - #### PURPOSE: TO ANALYZE YEARLY STREAMING TRENDS FOR ARTISTS, IDENTIFYING PATTERNS AND CHANGES IN POPULARITY OVER TIME.

    OTHER VISUALIZATIONS INCLUDE:
10. TOTAL ARTIST = 197
    TYPE: CARD
11. TOTAL STREAMS = 273,000,000,000 (BILLION)
    TYPE: CARD
12. TOTAL TRACKS = 256
    TYPE: CARD
13. SPOTIFY PLAYLIST = 3,000,000 (MILLION)
    TYPE: CARD
14. DEEZER PLAYLIST = 276,000 (THOUSAND)
    TYPE: CARD
15. APPLE PLAYLIST = 32,000 (THOUSAND)
    TYPE: CARD
16. SHAZAM PLAYLIST = 0 (NOT PROVIDED IN THE DATA SET)

### OTHER ANALYSIS AND VISUALIZATIONS THAT CAN BE CARRIED OUT.

1. Total Streams by Track and App
   Type: Stacked Bar Chart
   Purpose: See where streams are coming from.
   
2.	Artist Popularity
   Type: Bar Chart or Pie Chart
   Purpose: Show which artist has the most streams and their sources
  	
3.	Danceability vs. Streams
  Type: Scatter Plot
  Purpose: Correlate danceability with streaming numbers

4.	BPM Analysis:
  Type: Histogram
	Purpose: Distribution of BPM across the dataset

5. Trending vs. Non-Trending Visibility:
  Type: Bar Chart, Radar Chart
	Purpose: App visibility of trending and non-trending songs

6. Top 20 Track Names and Visibility:
   Type: Bar Chart
   Purpose: Visibility of top tracks across musical apps
   
7.	Artist Count vs. Trending Status:
   Type: Bar Chart
   Purpose: Compare single artists versus collaborations
  	
8.	Yearly Comparison of Artist Streams:
    Type: Slicer for Year, Bar Chart for Streams
    Purpose: Show artist trends over the years.

   # THEME AND STYLE
   - I used the iconic Spotify theme with its well-known colors: green, white, and black. This choice ensures a cohesive and visually appealing design, reflecting the brand’s identity perfectly.
     
•	Color Theme

 Spotify Green: Hex #1DB954, RGB (29, 185, 84), #016E51 RGB (255, 255, 255), #19423F,  RGB (255, 255, 255), #59A472  RGB (255, 255, 255).
 White: HEX: #FFFFFF RGB: (255, 255, 255)
 Black HEX: #000000 (RGB: 0, 0, 0)

•	Fonts:
o	Circular for Spotify elements
o	Aerial Black for headings (35pt and 12pt)
