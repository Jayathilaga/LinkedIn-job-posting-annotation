
# General annotation rules

- Job description from Linkedin  are extracted using web scrapping tools.
- We have planned to annotate SKILLS which are technology related like Python, Java, Agile, Scrum, etc.
- Any annotation that is related to soft-skills are not taken into consideration like Team building skills, excellent verbal communication required.
- We are considering only few Parent classes of job classes that are present in the Information Technology sector like :
     - Data scientist 
     - Software developer 
     - Data Analyst 
     - Cyber security Analyst 

- This restriction is applied because of the limited domain knowledge from other industries.

- `SKILLS` - Technologies paraphrased from the job description. example: Python, Java, Agile, Scrum, etc.

- `CLASS_NAME` - Ideal job title (not the job title from LinkedIn). example: Data Scientist, Quality Analyst, Front-end developer, etc.

- `EXPERIENCE` - Experience level required for the job. example: Novice, intermediate, Advanced, Expert.


## Data 

All the Job description is scraped and stored in a CSV file. It was cleaned from html tags and prepared for annotation during scraping, i.e. files only contain plain text .

The code that produces the data can be found in :https://github.ubc.ca/MDS-CL-2022-23/LinkedIn_Posting_Markup/blob/master/data/linkedin_data.csv 
