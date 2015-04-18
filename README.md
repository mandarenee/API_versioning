#3 Ways to Version an API:

##1. URL
###Description
Include the version in the URL. eg. http://api.example.com/v1.1.1
###Pros
-Simple for simple API with no interdependencies
-To make a new version, you can copy and paste the version folders
-Direct
-Permalinks are more dependable
###Cons
-Inability to evolve system parts independently
-Changes create a new tree of resources
-Client/Server tight coupling
-Headache for testing
-Unstable for changing elements like caches, spider, and forms

##2. Accept Header
###Description
A vendor can make a customizable Accept Header that includes the version
###Pros
-Many ways to set up
-More freedom in design
-RESTful
###Cons
-Clients can infer version in the path
-One extra step that developers have to deal with in working with the API
-Less explorable

##3. No versioning - just make the changes
###Description
Instead of versioning, make the changes to the exising app's version.
###Pros
-No need to worry about several versions
-Tons easier
-No extra steps
###Cons
-Making changes to the API could break client's apps that are reliant
-Not a sustainable practice
-The app can't always improve itself because of the editing limitations

##Personal Preference to use:
I will try adding the version to the URL. I have a simple app to set up that I don't expect to scale or to add additional versions to. There is a great RailsCast that I would like to follow.

