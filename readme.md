# MyChat

## Description 
A Group video calling application using the Agora Web SDK with a Django backend.

##  How to use this source code

#### 1 - Clone repo
```
git clone https://github.com/divanov11/mychat
```

#### 2 - Install requirements
```
cd mychat
pip install -r requirements.txt
```

#### 3 - Update Agora credentals
In order to use this project you will need to replace the agora credentials in `views.py` and `streams.js`.

Create an account at agora.io and create an `app`. Once you create your app, you will want to copy the `appid` & `appCertificate` to update `views.py` and `streams.js`. If you have questions about where to get your app I'd recommend referencing this link `https://youtu.be/HX6AM_1-jNM?t=88`

###### views.py
```
def getToken(request):
    appId = "516a4ce144ed4006b60df99d8dc9ef0b"
    appCertificate = "f3fa1caa56c24e1da703823f3ce632ef"
    ......
```

###### streams.js
```
....
const APP_ID = '516a4ce144ed4006b60df99d8dc9ef0b'
....
```


#### 4 - Start server
```
python manage.py runserver
```


