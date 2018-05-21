# Instagram-Crawler
This project we cover several segments of data collection on Instagram and their presentation 1. Python scrip solution that captures/craws data from Instagram. 2. Enter the collected instagram profile information in the database. 3. View and filter the data on a simple WEB site in Django Framemwork. 4. Practical application

## INSTALLATION REQUIREMENTS
 
* Install Python 3.6.0
* Install the Pip Package, type in the command line:
  
  ***python get-pip.py***
* Install Pip requests (This will install Django and Selenium frames)
  
  ***cd * PATH * / Project*** 
  
  ***pip install -r requirements.txt***
* Install Firefox Client (you can download the famous Mozilla Firefox browser)
* Completed



## SETTING UP THE WEB SYSTEM
* If you want to use the web system, then you need to deploy the entire Django system in the database. We do this with the following code:

  ***cd * PATH * / Project / web. / manage.py makemigrations***

This will perform the migrations from the model. /manage.py migrate Convert migrations from a model to a base

* Default user/admin access : 
 
  * user : admin
  * password : admin
  
* To create a Super Administrator who has all the privileges, type:

  ***./manage.py createsuperuser***

Enter the fields that are required.

* To turn on the server, run the following command and activate the Django Web application at port 8000

  ***./manage.py runserver 8000***
  
  

## INSTRUCTIONS FOR USING THE CRAWL SCRIPT
Using the script to collect data is too simple, here is the full api with which you can serve.

***Warning! Before you start using any kind of service from the crawler, you must configure the authentication instagram user 
that will be used for crawling the data which is visible only for autheticated users***

* Go to Project / script / settings.py
* Change Authentication info 

  ***Default is : username = "kiril_cvetkov" password = "*******"***
* Enter your username and password through which the browser will log in.
 
Once we have configured our sniffer, Below is the full API as well as an example to give a complete picture of how the script can be used

```
crawl.py [-db EXPORT_DB] [-DIR DIRECTORY] [-page PAGE_NAME] [-more MORE_DETAILS] [-num POST_NUMBER]
 
* [-db EXPORT_DB] Whether to save data in a database or only in a file system
* [-DIR DIRECTORY]: Directory where the data will be stored
* [-page PAGE_NAME]: Profile / crawling page
* [-more MORE_DETAILS]: Retrieve more details, such as number of likes, description of pictures within a single photo
```
