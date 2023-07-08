# LinkedIn-job-posting-annotation

PEER REVIEW INSTRUCTIONS
SETUP
1.	To download the LinkedIn Job Skill app image file, you need to download jobskills.tar and launch the Docker app.
2.	After downloading jobskills.tar, please open your terminal and navigate to the directory containing the file is located and provide the following command
a.	docker load -i jobskills.tar
3.	Then to run the app remotely follow the command below,
a.	docker run -d -p 5000:5000 hariharavarshan/jobskills:0.0.1.RELEASE
To open the app navigate to your browser and open http://localhost:5000/.
FEATURES
Please find the following instructions to understand our interface and the functionality of our application:
 
1.	Search by skills:
a.	When skills separated by comma are provided, the top 100 job listings are provided. 
b.	eg: python, r    
c.	The API returns the job posting data based on the skills entered.
d.	Download CSV: The user can also look into the job description using a download button the interface. The user can use the LinkedIn link to go their specific job posting to understand how the annotations are done.
 
2.	Search by job:
a.	When job title is provided, skills percentage required for this job is calculated and plotted in a bar chart.
b.	It has dropdown of different job titles extracted from LinkedIn.    
c.	The API returns the top 10 skills mentioned in the job postings for that job class.

 
3.	Word cloud:
a.	 Users can understand, if a technology is having overlap with multiple job titles by using the word cloud technique.
b.	By searching the required technologies, we can understand, which are the job title that the user can apply for.
 
