# Neighborhood Map Project


Included is a list of great restaurants around central park 
The app allows you to filter the list down, and in return displays the locations on the map along with some additional info pulled from Foursquare where available (such as websites and phone numbers, although none of the places listed require a reservation.)

Open index.html to run the web application

The "initialLocation" is a list of all the restaurants' basic location info (name, lattitude longitude)

As for the model:
I use "Location" object.
1. It will get all basic info(include tel, address website) from Foursquare's API
2. It will change all the info into a unified format
3. Using ko.computed to determine whether to show the restaurant on the map
4. Add "click" event on the "maker" to show basic info

As for the viewmodel:
1. It will create the map on screen
2. Will make the "Location" Object and put them into a "ko.observableArray"
3. The searchItem is a "ko.observable" to hold the searchItem
4. "this.filteredList" is "ko.computed" function which will determine whether to show the restaurant on the map

