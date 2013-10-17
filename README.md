# Mobile3-Notes

New Project setup files like .gitgnore and etc files example just copy and paste while creating new Mobile project.


## More Information

Some files in a Mobile project should not be checked into a Git version control repository. You can tell git to ignore certain files by creating a file called **.gitignore** in the top level of your working directory.

## Using the File

Copy the example file **gitignore.example** to the top level of your working directory and rename it *.gitignore* (For both platforms).

Note that git will not ignore a file that was already tracked before a rule was added to this file to ignore it. In such a case the file must be un-tracked, usually with `git rm --cached filename`.


# Mobile Best Practices


The goal of this guide is to present a set of best practices and style prescriptions for Android, Iphone and other mobile platform development. The practices that we follow helps other developers to understand the code much easily , the naming and the coding convensation not only help the developers working in a team but also helpfull for any new person to understand and read the code.

##Few of the naming convenstions that the mobile team follows are : 
* [Naming Projects](#naming-projects)
* [Naming Packages](#naming-packages)
* [Naming Classes](#naming-classes)
* [Naming Methods](#naming-methods)
* [Naming Objects](#naming-Objects)
* [Naming View Files](#naming-view-files)
* [Naming View elements](#naming-view-elements)

###Naming Projects

* The project name should be the name of the application that you are developing.
* Use simple and short name that reflects the use or the purpose of the application.
	
	```Android
		FriendPickerSample
		AndroidTwitterConnect
	```

###Naming Packages

* Usually the number of classes created in an application is quite high which becomes difficult to maintain , so using the packages for the classes performing simillar functions reduces the complexity of the project.
* Naming convenction of the pakages helps to differentiate the classes that are working on functionality like database , web services and adapters .
	
	```Android
		com.webonise.projectname
		com.webonise.projectname.webservice
		com.webonise.projectname.dbhandler	
		com.webonise.projectname.helper
		com.webonise.projectname.adapter	
	```
* Packages name also changes as per requirement of the client.
	
	```Android
		com.headsuprules
		com.headsuprules.adapter
		com.headsuprules.webservice
	```	 
###Naming Classes

* The names should follow the camel case naming convention and should always start with capital letter.
	eg. MainActivity , ImageListAdapter etc.

* The name of a class should reflect the type of class it is extending or implementing.

	* The classes that are extending from `Activity` or `FragmentActivity` should always have *Activity* as a suffix.  
		Few Examples are like this :

	```Android
		MapActivity
		FriendActivity			
	```

	* For the classes that are extending from `Fragment` there names should have `Fragment` as suffix.
	
	```Android
		MapFragment
		FriendFragment			
	```
* For simple classes the names also should be simple to reflect the working of the class.
	eg. Parser , DbHandler , ImageReceiver etc. 

###Naming Methods
* The method name should also follow the camel case naming convention and should always start with small letter.

	```Android
		public void onResultReceive() {
		......
		}
	```

	```Android
		public String getName() {
		.....		
		return name;
		}
	```
* Method name should reflects the functionality of the method.

###Naming Objects

* Object name should also follow the camel case naming convention and should always start with small letter.

* An object name should have a part of the name reflecting the type of object it is.
	Few excmples are like this : 
	
	 ```Android
		TextView textViewHeader;
		TextView textViewTitle;
		
		ImageView imageViewProfile;
		
		Button buttonNext;
		Button buttonPrevious;
	```
###Naming View Files

* View files or the layout files should always have small letters and if the name is large then words saperated by underscore.
	eg. 	image_view_list.xml 
		map_fragment.xml etc.

###Naming View Elements

* Elements names or id should always be in camel case starting with small letter.



