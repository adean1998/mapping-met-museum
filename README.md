# Mapping the Met

# Project Description
This project seeks to highlight biases and patterns in the Metropolitan Museum of Art's collecting practices by mapping the locations of their "Highlights" works. The Met "Highlights" are objects that museum staff have presumably categorized as high-quality or culturally significant. This type of subjective classification is prone to bias on the part of those selecting these works, and by mapping their locations of origins, we can determine if biases are present and if they are location- or culture-based. 
# Rationale Statement
Museums' collecting and curation practices are inherently biased, especially at large museums with objects from a range of cultures. In the United States, museums often prioritize the display and study of works from white, Western societies. Through data visualization, this project attempts to determine whether the objects that the Met considers significant are mostly from these cultures, or if any other patterns emerge from the data.
# Workflow
This project uses the Metropolitan Museum of Art's API to map works' locations/cultures of origin via Plotly. First, all of the works that are classified as highlights must be compiled into a csv file that lists basic information about them as well as their locations of origin. Next, the data will be entered into Plotly to create a map of the works' locations of origin. Finally, this information will be entered into a github site which will function as a platform to display and discuss findings. 

# Further Uses
The code used in this project might be repurposed to determine other trends in the Met's collecting practices, such as the gender of the artists, the cultural classifications, or the number of objects in each department.

# Files List
- **METcountries.ipynb**:
A python notebook with all of the code for creating a dataframe with Highlights from the Met API
- **mappingthemetMAP.csv**: A CSV file with all the Highlights in a dataframe, edited for clarity and compatibility with Google MyMaps
- **Department CSVs**: CSVs with all artworks sorted by department
