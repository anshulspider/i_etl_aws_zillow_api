# zillow-rapid-api
end-to-end data engineering project 


what's the project about?--

In this project i have created an end-to-end data pipeline , i.e. the data is coming from zillow rapidapi and to the last data reporting for stakeholders.....

Used tools and technologies--
1.airflow
2.aws(ec2,s3,quicksight,lambda,redshift)
3.python
4.sql(basic)

So,
the data is coming from rapidapi and transferring to aws s3 bucket 
I've created 3 s3 buckets
one for transferring raw data from api
second for copy of raw data
third for storing trasformed data

in between these s3 buckets ive programmed lambda function (2 lambda function )
these get trigerred automatically when data gets inside s3

after the last s3 the dataset gets transferred to redshift which is more or less like a 
cloud RDMBS and after that ive finally reported this using quicksight

these tasks were monitored and triggered by airflow throught the systems
airflow is running as standalone in ec2 which is accessed by my local machine by ssh(in vscode)
