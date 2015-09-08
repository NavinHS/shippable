# Shippable

## Project Description

This is a simple application where an user can input any github repository link, and the respected output displayed in a table would be total number of open issues in the github repository, total number of open issues that were opened in the last 24 hours, total number of open issues that were opened more than 24 hours ago but less than 7 days ago and number of open issues that were opened more than 7 days ago. 


## Code Description

The URL of the repository is retrieved and validated whether it is a valid github repository.The Github Api returns back only 30 issues per page.Inorder tie view the total number of pages, the response headers are being checked and the total number of pages are being retrieved (i.e the last page number).Ajax request is being sent to all pages to get all the issues in json format.
All reponses are parsed and issues are saved by checking their created_at timestamp. 

## Tests

1)Download the two files index.html and script.js and save both the files in the same direcotry.
2)Run the index.html file.
3)Try any github repository link to view the open issues.

##Future Enhancements

Given more time , we will add some methods for login so that the github api responds with 100 issues per request.Without authentication it provides only 30 issues per request. Result can be optimized more further.


