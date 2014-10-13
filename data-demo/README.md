# Demo Bluemix and Cordova using Cloud Data

## 1 Setup Backend 
- Register on [Bluemix.net](http://bluemix.net)
- Create Backend App with Mobile Cloud Starter boilerplate

## 2 Install Software
- Mobile Platforms SDKs (Xcode, Android SDK)
- Node, NPM, Git, Ant
- npm install -g ionic cordova gulp
    
    
## 3 Get the Frontend code    
    
    git clone http://github.com/csantanapr/aahackathon
    cd aahackathon/data-demo/bluelist-mobiledata-cordova/
    npm install
    gulp install
    
## 4 Setup Frontend with Backend settings    
    
    update www/bluelist.json with values from your Mobile Cloud on Bluemix.net
    
    {
    "applicationId": "0000111112222",
    "applicationSecret": "111222333",
    "applicationRoute": "something.mybluemix.net"
	}

## 5 Add Platforms and Plugins
    
    ionic platform [ios | android ]
    or
    cordova platform add [ios | android]
    
    [ionic | cordova] plugin add [com.ibm.mobile.cordova.ibmbluemix | https://hub.jazz.net/git/bluemixmobilesdk/ibmbluemix-cordova]
        
    [ionic | cordova] plugin add [com.ibm.mobile.cordova.ibmdata | https://hub.jazz.net/git/bluemixmobilesdk/ibmdata-cordova]

    
## 6 Build and Run
    
    ionic build
    ionic run android
    open platforms/ios/BlueList.xcodeproj

