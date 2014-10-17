# Demo Bluemix and Cordova using Mobile Data

## Demo Turorial Video: [http://youtu.be/cDM1iWwACCQ](youtu.be/cDM1iWwACCQ)


## 1 Build and Deploy Watson Java Backend
	- [https://github.com/jsloyer/talent-manager-complete]()
   
## 2 Configure Watson Java to access Mobile Data
	- Edit src/com/ibm/personafusion/Config.java

	public static final String MOBILE_DATA_APP_ID = "xxxx";
    public static final String MOBILE_DATA_APP_SECRET ="xxxx";

## 2 Setup Mobile Data Service Backend 
	- Register on [Bluemix.net](http://bluemix.net)
	- Create Backend App with Mobile Cloud Starter boilerplate

## 3 Install Software
	### - Mobile Platforms SDKs (Xcode, Android SDK)

	#### - Node:
 	- [nodejs.org](http://nodejs.org)

	#### - Android SDK Tools:
 
 	- [bit.ly/androidwinsdk](http://bit.ly/androidwinsdk)
 	- [bit.ly/androidmacsdk](http://bit.ly/androidmacsdk)

	#### - Apache Ant:
 	- [http://bit.ly/antbintool](bit.ly/antbintool)

	### - Node, NPM, Git, Ant
	- npm install -g ionic cordova gulp
    
    
## 4 Clone or download the Frontend Mobile code    
    
    git clone http://github.com/csantanapr/aahackathon
    cd aahackathon/data-demo/bluelist-mobiledata-cordova/
    npm install
    gulp install
    
## 5 Setup Frontend with Backend settings    
    
    edit www/bluelist.json with values from your Mobile Cloud on Bluemix.net
    
    {
    "applicationId": "0000111112222",
    "applicationSecret": "111222333",
    "applicationRoute": "something.mybluemix.net"
	}

## 6 Add Cordova Platforms and Plugins
    
    ionic platform [ios | android ]
    or
    cordova platform add [ios | android]
    
    [ionic | cordova] plugin add [com.ibm.mobile.cordova.ibmbluemix | https://hub.jazz.net/git/bluemixmobilesdk/ibmbluemix-cordova]
        
    [ionic | cordova] plugin add [com.ibm.mobile.cordova.ibmdata | https://hub.jazz.net/git/bluemixmobilesdk/ibmdata-cordova]

    
## 7 Build and Run Mobile APp
    
    ionic build
    ionic run android
    open platforms/ios/BlueList.xcodeproj

