# About Dataset
## Dataset Information
This data is from Open Source Mental Illness (OSMI) using survey data from years 2014, 2016, 2017, 2018 and 2019. Each survey measures and attitudes towards mental health and frequency of mental health disorders in the tech workplace.

The tables have the following schema:
Survey (PRIMARY KEY INT SurveyID, TEXT Description)
Question (PRIMARY KEY QuestionID, TEXT QuestionText)
Answer (PRIMARY/FOREIGN KEY SurveyID, PRIMARY KEY UserID, PRIMARY/FOREIGN KEY QuestionID, TEXT AnswerText)

SuveyID are simply survey year ie 2014, 2016, 2017, 2018, 2019.
The same question can be used for multiple surveys
Answer table is a composite table with multiple primary keys. SurveyID and QuestionID are FOREIGN KEYS.
Some questions can contain multiple answers, thus the same user can appear more than once for that questioned.

## Analysis
In the accompanying code, you can see all the steps I undertook to analyze the data. Ultimately, I focused on providing sociodemographic descriptive statistics, creating indices of openness of employees to share about their mental health and employee supportiveness (and their correlation), as well as sentiment analyses of personal experiences shared by respondents.

## Future Work

- Improve comparison methods by aligning similar survey questions across years.
- Explore additional factors influencing workplace mental health.
- Conduct deeper analysis into the relationship between mental health openness and demographic factors.

## Running the project
To run this program, ensure you have all the libraries downloaded that I listed in the requirements.txt file. After this, have the dataset downloaded in your local directory, and open and run my file.

