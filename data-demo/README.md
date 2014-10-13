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
## 5 Build and Run
    
    ionic build
    ionic emulate android
    open platforms/ios/BlueList.xcodeproj


### (Optional) How to recreate demo

    npm install -g ionic cordova gulp
    #App ID: com.ibm.bluemix.bluelist.cordova
    #App Name: BlueList
    #App Project: bluelist-mobiledata-cordova
    #App Template: tabs
    ionic start -a BlueList -i com.ibm.bluemix.bluelist.cordova bluelist-mobiledata-cordova tabs
    cd bluelist-mobiledata-cordova/
    cp -r 
    npm install
    gulp install
    ionic platform ios
    ionic platform android
    cordova plugin add https://hub.jazz.net/git/bluemixmobilesdk/ibmbluemix-cordova
    cordova plugin add https://hub.jazz.net/git/bluemixmobilesdk/ibmdata-cordova
    ionic emulate android -l
    ionic emulate ios -l
