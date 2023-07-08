# Technical Interface Documentation

Below we have detailed description of backend and frontend of the project.

## Requirements

To successfully run the project, one would need to have the following dependencies installed :

- Python 3.9 (or above)
- flask==2.2.3
- pandas==1.4.3
- scipy==1.9.3
- numpy==1.23.2


## 1. Backend

We have used Flask with Python to implement the interface's backend.

### 1.1 app.py

- This file implements the interface's functionality, using Flask that responds to "POST" requests from a browser. The code is broken down into functions with proper documentation.

- Here are few of the main functions that we have worked on :

    -  `job_data_api()`
        - When skills separated by comma are provided, the top 100 job listings are provided. 
        - This API accepts a POST request with parameter skill (the json format should be {'skills':'python, R'} ).    
        - The API returns the job posting data based on the skills entered.
    -  `wordcloud_api()` 
        - When skills separated by comma are provided, bi-gram word clouds are generated.
        - This API accepts a POST request with parameter skill (the json format should be {'skills':'python, R'} ).    
        - The API returns the word cloud data based on the skills entered.
    -  `class_skill_api()` 
        - When job title is provided, skills percentage required for this job is calculated and plotted in a bar chart.
        - This API accepts a POST request with parameter class (the json format should be {'class':'software_engineer'}).    
        - The API returns the top 10 skills mentioned in the job postings for that job class. 
    -  `download_csv()` 
        - It downloads all the filtered job listing for the comma separated skills provided by the user.
    
 
## 2. Frontend


### 2.1 index.html

- The `index.html` contains three options to choose, namely search by skills, search by job, word cloud.

- When one search type is chosen it will go to that particular page.

### 2.2 skill.html

- The `skill.html` takes in skills as input when provided in comma separated format. When `Get job info` is clicked, we will get 100 job descriptions related to these skills. 

### 2.3 job.html 

- The `job.html` contains a drop down to choose a title from all the parent class(class name). We get all the skills that are related to this job title with percentage expectation. These information are plotted as bar chart.

### 2.4 wordcloud.html

- The `wordcloud.html` takes in skills as input when provided in comma separated format.  When `Get wordcloud` is clicked, bi-gram word clouds are generated based on the job descriptions.


## Docker Commands


- To Build docker image
    - docker build -t hariharavarshan/jobskills:0.0.1.RELEASE .
- To run docker image locally:
    - docker container run -d -p 5000:5000 hariharavarshan/jobskills:0.0.1.RELEASE
- To view the status of the docker image
    - docker container ls
- To save the docker image as tarball
    - docker save jobskills > jobskills.tar
- To stop the docker image running
    - docker container stop 0f8
- To push the docker image to docker.hub
    - docker push hariharavarshan/jobskills:0.0.1.RELEASE

- To pull the docker image from docker.hub
    - docker pull hariharavarshan/jobskills:0.0.1.RELEASE
- To run the pulled docker image locally
    - docker run -d -p 5000:5000 hariharavarshan/jobskills:0.0.1.RELEASE
    
- Then go to browser and open the app
    - localhost:5000
    

