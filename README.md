# WebServer-Calculation-Notes
### 
```


(number of CPU cores / Average Page Response Time in seconds) * 60 * User Click Frequency in seconds = Maximum simultaneous users
```
### Formula Calculating the max capacity of your web server
```
Average time for a page request (in seconds) -Chrome Browser->Inspect->Network->Time (response time of the webpage)

Example: 
    Using VPS 2 cpu / .135ms = 14.8 (15) max number of page request per second
Formula:
    Number of CPU cores / Average time for a page request (in seconds) = Max number of Page Requests per second
```
### How many users can I have on my web site simultaneously?
```
Note: 
    Rule of thumb for ecommerce is 1 user per minute (60 seconds).
Given: 
    Avg. Session Duration (00:09:10)
    Page / Session ( 4.82 )

Compute Click frequency of users in seconds 
    -In Google Analytics Audience->Overview 
           Avg. Session Duration( 9min ) * 60 seconds + Avg. Session Duration( 10sec ) = Session Duration ( 550 )
          Session Duration ( 550 )  / Page/Session ( 4.82 ) = 114 sec (approx. once every 2 minutes)          
Example: 
     15 Page request per seconds * 60 seconds * Click Interval in 2 minutes = 1800 Max simultaneous users
     
Formula:
     Number of max requests per second * 60 * Click frequency of users in seconds = Maximum Number of Simultaneous Users
```
### How many users can I have on my VPS?
```

Average PHP request time: 650ms
CPU cores: 2
Click frequency: 45 seconds (normal for e-commerce)

2 cores / 0.65 = 3 pageviews per second * 60 * 0.75 = 135 Max simultaneous users
```
### Reference
```
https://servebolt.com/articles/calculate-how-many-simultaneous-website-visitors/
```
