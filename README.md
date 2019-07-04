# AWS S3 SELECT :

### How to query AWS S3 bucket using AWS S3 Select ?

### AWS S3 Bucket :
Amazon Simple Storage Service (S3) stores data for millions of applications used by market leaders in every industry. 

With S3, I can store as many objects as I want and individual objects can be as large as 5 terabytes. Data in object storage have traditionally been accessed as a whole entities, meaning when you ask for a 5 gigabyte object you get all 5 gigabytes. It’s the nature of object storage.

### S3 Select enables applications to retrieve only a subset of data from an object by using simple SQL expressions.

By using S3 Select to retrieve only the data needed by your application, you can achieve drastic performance increases – in many cases you can get as much as a 400% improvement.


### DEMO

select count(*) from s3object s\
select * from s3object s limit 10\
select * from s3object s where s.reqId='1000'\
select * from s3object s where s.reqMethod='GET'\
select * from s3object s where s.resStatusCode='401'\
select * from s3object s where s.resStatusCode='200'\
select * from s3object s where s.accept='application/json'\

