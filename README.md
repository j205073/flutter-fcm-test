# fcmtest
### Postman payload
url:
https://fcm.googleapis.com/fcm/send \
method:post

```json
{
 "to" : "YOUR DEVICE FCM TOKEN",
 "collapse_key" : "type_a",
 "priority" : "high",
 "notification" : {
     "android_channel_id": "fcm_muster_channel", //自訂channel id
     "sound": "muster",       
     "title": "Test FCM",
     "body" : "Test Notify"
 },
  "data" : {
     "body" : "Sending Notification Body From Data",
     "title": "Notification Title from Data",
     "key_1" : "Value for key_1",
     "key_2" : "Value for key_2"
 }
}
```
sound file path:\android\app\src\main\res\raw\muster.wav

```dart
//device fcm token
 String? token = await messaging.getToken(
    vapidKey:
        'Fcm 後臺設定的網路推播憑證金鑰組',
  );
  ```
  
  fcm console:[https://console.firebase.google.com/](https://console.firebase.google.com/)

![image](https://user-images.githubusercontent.com/17948436/205470425-05ddbdab-8e2c-4960-a38f-a23c82bc0cef.png)
![image](https://user-images.githubusercontent.com/17948436/205470389-1e11e3b0-a45f-42e1-9a7b-17a779c16efb.png)

Getting started

``` terminal
//clean cache
flutter clean

//start project
flutter start

```


j205073/flutter-fcm-test
