# music-entertainment-analytics

## Folder Structure

- **`docs/`**  
  - **`images/`**  
    - `erd_music_entertainment.png`  
      A visual Entity-Relationship Diagram showing table relationships (Agents, Entertainers, Customers, etc.).  
  - `Technical Report.pdf`  
  - `music_entertainment_presentation.pdf`  
  - `EDA.pdf`  
  - `Time Series.pdf`

- **`sql/`**  
  - `entertainment_schema.sql`  
    SQL script to create the tables (Agents, Entertainers, Customers, Engagements, ztblDays/Months/Weeks) matching the ERD.

- **`notebooks/`**  
  - `Null_Values.ipynb`  


## How to Reproduce

1. **Review the ERD**  
   - Open `docs/images/erd_music_entertainment.png` to see the complete schema and foreign‐key relationships.  
2. **Run the Schema SQL**  
   - From inside your SQL client (e.g., psql), load `sql/entertainment_schema.sql` to create all tables including Agents, Entertainers, Customers, Engagements, Entertainer_Styles, Musical_Styles, etc.  
3. **Load data & explore**  
   - Use your own sample data or the data dumps (if included under `data/`) to populate the tables.  
4. **Execute queries**  
   - Follow the guidance in `docs/EDA.pdf` for your exploratory queries.  
   - Run the time‐series queries in `docs/Time Series.pdf`.  
   - Check missing values with `notebooks/Null_Values.ipynb`.  