## Demo for AA Hackathon Bluemix and Cordova using Cloud Data

### How to run demo

    npm install -g ionic cordova gulp
    git clone http://github.com/csantanapr/aahackathon
    cd ncdevcon/bluelist-mobiledata-cordova
    update www/bluelist.json with values from Bluemix.net
    npm install
    gulp install
    ionic platform ios
    ionic platform android
    ionic emulate android
    ionic emulate ios


### How to recreate demo

    npm install -g ionic cordova gulp
    #App ID: com.ibm.bluemix.bluelist.cordova
    #App Name: BlueList
    #App Project: bluelist-mobiledata-cordova
    #App Template: tabs
    ionic start -a BlueList -i com.ibm.bluemix.bluelist.cordova bluelist-mobiledata-cordova tabs
    cd bluelist-mobiledata-cordova/
    npm install
    gulp install
    ionic platform ios
    ionic platform android
    cordova plugin add https://hub.jazz.net/git/bluemixmobilesdk/ibmbluemix-cordova
    cordova plugin add https://hub.jazz.net/git/bluemixmobilesdk/ibmdata-cordova
    ionic emulate android -l
    ionic emulate ios -l
