# Annotation Plan

## Annotation Type

We will annotating in two different ways. 

First, we classify the job postings into bigger parent classes based on the title. For example, the job titles `senior data scientist` and `junior data scientist` belong to the parent class `data scientist`.

Second, we will be tagging all the skills/tools mentioned in the job listing such as `Python`, `SQL`, `AWS`, `PyTorch`, etc.


## Details

Input : A `csv` file containing multiple columns (`job title`, `job description`, etc). Each row is one job listing.

We will first be classifying job postings based on their title. For example, these may be like : 

1. `Data Scientist`

2. `Data Analyst`

3. `Software Developer`

4. `Quality Assurance Engineer`

5. `Full Stack Developer`


On top of this, we will tag all the skills/tools mentioned in each job listing. For example, they will look like :

`Python`, `Pandas`, `PowerBI`, `Tableau`, `AWS`, `Docker`, `Node`, `React`, etc.


## Annotation tool

We will be using tools like `GATE` and `labelstudio` for annotation.


## Annotators

The members of the group (Hari, Jaskirat, Jaya, Sai) will be the annotators. We will divide the dataset equally amongst ourselves to perform annotation. Then, each member will verify the annotations done by all the other group members.

## Amount of Data

We plan to annotate around 400-500 job listings in the upcoming week. Since there are four of us, each of us will be annotating 100-125 job listings. The estimated time for each annotation is around 3-5 minutes. We will also be reviewing each others annotations.

## Quality of Annotations

We took a few steps we are planning to take to ensure that the annotations are of good quality:

1. We plan to make a document stating which parent class each job title should belong to.

2. In case of conflicts, we plan on taking a vote and go ahead with the majority.

