# SuperTravel
# Group name and section: LifeIsHard_T

# Group Members: 
Jiajing Wang (Section 1) jw3687@columbia.edu
Tian Xia (Section 1) tx2181@columbia.edu
Siyao Zhen (Section 1) sz2778@columbbia.edu
Senhao Hu (Section 1)  sh3818@columbia.edu

# Main Idea:
Our initiative was from our daily life. Everytime we plan to travel to different cities or interested places, we are suffered from planning, scheduling, conflicts and negotiating. There would be tons of different web pages to be opened in order to finish our schedules. Thus, we would like to offering travellers easy way to determine where they want to go, live and eat in New York city. 

We built an interface to provide travelling suggestions for tourists in New York City, based on their preferences of the travelling date and attraction categories. After choosing their own destination categories (Museum, Amusement, Galleries, Shopping Center and Tourist Attraction)  and their check-in/check-out date, the next interface will provide them with recommended attractions’ name. By clicking each attraction name, the interface will bring you to another interface with recommended restaurants near that attraction

Our first step was to collect all attraction and restaurant data from Yelp. We web-scrapped the hotel information, such as name, ranking, address etc, from TripAdvisor. For the room type, we assumed a standard room. 

Then, We grab the name, location, phone number, latitude and longitude from yelp for each attraction as well restaurant. We stored all the attractions  as well as the hotels’ information into two csv files using sql and packages, like numpy or pandas. The final csv files are the databases for latter searching. The two datasets are under the name tour.csv and hotel.csv. The interface will only produce 10 recommendations. Each recommendation is selected based on their ratings.  

Finally, we developed a map for each combination of choice. Since our map.html cannot be shown in our interface, we developed a function to get a screenshot of the map on our main interface, after you chose your preference. The map would show all the locations and sites you needed. This map can save us a lot of time when we travel. We can arrange our time and the travelling order of these sites based on the maps developed. 


# Installation Instructions: In this project, we import several python libraries, including:
Requests
Bs4
Beautifulsoup
Pandas
Numpy
re
tkinter
tkinter.scrolledtext
webbrowser
csv
pymysql
folium
Sys

# If you have errors in importing any of the previous packages, please try:
!pip install (packagename) in jupyter notebook

# 2nd choice: run conda install 
The chromedriver is the software that needed to be downloaded outside jupyter notebook
The chromedriver has been added to github

# Run Instructions:
The path.csv needed to be changed.
The path is the executable path of chromedriver you have saved.
The mappath is the file directory of the map been saved from running jupyter notebook (normally it is in the same directory as the jupyter notebook, name is map.html).
The rpath.csv needed to be changed.
The path is the executable path of chromedriver you have saved.
The mappath is the file directory of the restaurant map been saved from running jupyter notebook (normally it is in the same directory as the jupyter notebook, in the name of rmap.html).
Our main file is interface.ipynb, you do not need to run Tools Project.ipynb since all the output from Tools Project file has been saved as several local csv files in the github.
