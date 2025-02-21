# ETL Pipeline for Literary Network Analysis: Character Relationships and Data Visualization

## Project Overview

This project demonstrates the use of an **ETL pipeline** to process and analyze literary data, specifically focusing on character relationships within books. The pipeline uses **Python** and **MongoDB** to extract raw data, transform it into a structured format, and load it into a MongoDB database. The project also visualizes the relationships and patterns between characters and books using various data visualization techniques.

The main objective is to explore connections between characters in literature, identifying influential characters, and uncovering narrative patterns through structured data processing and visualization.

## Key Features

- **ETL Process**:  
  - **Extract**: Raw datasets (Books, Characters, and Edges) are ingested using Python scripts into MongoDB.
  - **Transform**: Data cleaning, filtering, and transformation are performed to ensure high-quality data for analysis.
  - **Load**: The cleaned and transformed data is loaded into MongoDB for querying and analysis.
  
- **Data Visualizations**:  
  The project uses advanced data visualization techniques to present the relationships and trends in the dataset. Key visualizations include:
  - Network graphs to show character relationships
  - Bar charts to highlight the most connected characters and frequent books
  - Heatmaps to display co-occurrence patterns of characters across books
  - Sankey diagrams to trace character-book relationships
  - Interactive dashboards for easier exploration

## Research Questions

- How do relationships between characters and books manifest in the dataset?
- Who are the most influential characters, and what patterns can be inferred from their connections?
- How can advanced visualization techniques enhance the interpretation of complex networks?

## Technologies Used

- **Programming Language**: Python  
  Python was chosen for its rich libraries and ability to process large datasets efficiently.
  
- **Database**: MongoDB  
  MongoDB was used for its ability to handle semi-structured data with flexible schemas, making it ideal for managing the datasets.
  
- **Libraries**:  
  - **Pandas**: Data manipulation and analysis.
  - **NetworkX**: Network analysis and creation of relationship graphs.
  - **Matplotlib** and **Seaborn**: Basic visualizations.
  - **Plotly**: Interactive visualizations.
  
## Project Structure

- `mongo_raw.py`: Script for extracting raw datasets and loading them into MongoDB.
- `mongo_raw_georg.py`: Variant of the above script for different data extraction (if applicable).
- `mongo_raw_varun.py`: Another variant of the extraction script.
- `mongo_retrieval.py`: Python script used for retrieving and filtering data from MongoDB.
- `data_cleaning.py`: Handles data cleaning processes like removing duplicates and handling missing values.
- `data_transformation.py`: Normalizes and transforms the data into a format ready for analysis.
- `visualizations.py`: Contains scripts for generating the visualizations (network graphs, heatmaps, bar charts, etc.).
- `interactive_dashboard.ipynb`: Jupyter notebook for creating an interactive dashboard to explore the relationships.

## Workflow

1. **Data Extraction**:  
   The raw data (Books, Characters, Edges) is loaded into MongoDB using Python scripts. The data is parsed and prepared for further processing.

2. **Data Transformation**:  
   The data undergoes cleaning and transformation:
   - **Cleaning**: Removing duplicates, filling missing values, and ensuring data consistency.
   - **Transformation**: Data normalization to structure it for analysis and querying.

3. **Data Loading**:  
   After transformation, the data is loaded into MongoDB collections for efficient querying and retrieval.

4. **Analysis and Visualization**:  
   The data is analyzed to explore relationships, and various visualizations are generated to represent the findings. These include network graphs, bar charts, heatmaps, and Sankey diagrams.

5. **Interactive Dashboards**:  
   The final step involves building an interactive dashboard that allows both technical and non-technical users to explore the relationships and patterns in the data.

## Results

- **Central Characters**:  
  Network analysis reveals key influencers within the narrative, identified by nodes with high centrality.

- **Clusters**:  
  Community detection algorithms highlight tightly-knit character groups, reflecting subplots and character arcs.

- **Books as Hubs**:  
  Some books act as central hubs for character interactions, marking them as crucial in the dataset.

- **Character Co-occurrence**:  
  Heatmaps show patterns of collaboration and rivalry between characters, providing deeper insight into their relationships.

- **Interactive Feedback**:  
  Users reported that the interactive dashboard allowed for easy exploration and understanding of the relationships, making the analysis accessible to a broader audience.

## Challenges and Solutions

- **Handling Sparsity**:  
  Missing relationships in the dataset were addressed through imputation and filtering, ensuring that the dataset remained complete for analysis.

- **Visualization Scalability**:  
  Large networks were optimized using community-focused views, allowing for better clarity in visualizations.

- **Performance Optimization**:  
  Query optimization and efficient data structures were used to minimize computational overhead and ensure fast data retrieval.

## Conclusion

This project successfully demonstrates the use of Python and MongoDB for managing semi-structured data, creating a flexible ETL pipeline for literary network analysis. The analysis and visualizations provide valuable insights into character relationships and narrative structures, showcasing the power of modern data processing tools in literary studies.
