# CIS-2818-Project3-CryptoPrices
PROJECT #2: CRYPTOCURRENCY PRICES


INSTRUCTIONS
For this assignment, you will create an app to display the information about various cryptocurrencies, along with their prices.
Make sure to use Kotlin, not Java.
The Coincap API doesn’t require a key, but uses a REST API and returns JSON format data about a multitude of different cryptocurrencies. Information and live data can be viewed at coincap.io. However, the API that returns the JSON data is at https://api.coincap.io/v2/assets.
Go to this URL, and you can look through the JSON to become familiar with its format. Inside the root object, there is a property named data, which is an array of objects, each containing information about a single cryptocurrency. There are 100 cryptocurrencies in total available with live data through this API.
You should use the Volley HTTP library for Android to download the data from the Coincap API. You should maintain this data appropriately in memory so that the user can select which cryptocurrency they want to view information about. You should use a drop-down menu (In Android, these are Spinners) whose options represent each of the available cryptocurrencies. Each of the cryptocurrency names should be the only thing displayed in the drop-down menu.
Once the user selects an option from the drop-down menu, the information displayed next to the drop down should be updated.
The information displayed should include the following:
•
The name of the cryptocurrency in a TextView at the top
•
The crypto symbol (e.g., ETH, USDT, BNB)
•
The supply (rounded to the nearest integer)
•
The price in USD rounded to two decimal places
•
The percent change in the last 24 hours (also, to 2 decimal places)

The app should be appropriate styled to look professional. The displayed information should be in its own section, also styled appropriately so as to look professional. You should consider leveraging Fragments in order to display all the information.


![image](https://github.com/user-attachments/assets/6b0eb95b-0767-4fc6-ad91-c3b66a940cc7)

The “magic” is of course in how you locally store the information and work with it in memory after you receive it from the API.
Make sure to add the dependency for Volley to build.gradle, and also the INTERNET permission to AndroidManifest.xml. Otherwise your application will not be able to access the REST API.
//build.gradle:
dependencies{
//...
implementation 'com.android.volley:volley:1.0.0'
}
//Android Manifest:


DELIVERABLES
Please do the following:
•
Create (if you haven’t already) a folder named project3 with all of your code, properly organized
•
Screenshots of your app running appropriately
REFERENCES
•
Volley on Github
o
https://google.github.io/volley/
•
How to use Volley on Android in Kotlin by DBTechProjects
o
https://www.youtube.com/watch?v=Om08VYwatn8
•
What is a REST API? by IBM Technology (YouTube)
o
https://www.youtube.com/watch?v=lsMQRaeKNDk
•
Learn JSON in 10 Minutes by Web Dev Simplified (YouTube)
o
https://www.youtube.com/watch?v=iiADhChRriM


