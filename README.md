# WebServer-Calculation-Notes
### 
```


(number of CPU cores / Average Page Response Time in seconds) * 60 * User Click Frequency in seconds = Maximum simultaneous users
```
### Calculating the max capacity of your web server
```


Number of CPU cores / Average time for a page request (in seconds) = Max number of Page Requests per second
```
### How many users can I have on my web site simultaneously?
```
Note: Rule of thumb for ecommerce is 1 user per minute.


Number of max requests per second * 60 * Click frequency of users in seconds = Maximum Number of Simultaneous Users
```
### How many users can I have on my VPS?
```

Average PHP request time: 650ms
CPU cores: 2
Click frequency: 45 seconds (normal for e-commerce)

2 cores / 0.65 = 3 pageviews per second * 60 * 0.75 = 135 Max simultaneous users
```
