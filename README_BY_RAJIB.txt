Original Project
----------------

https://github.com/firebase/quickstart-js/tree/master/messaging

# Frontend Application

nmp start # to start the application


# Backend and serverside implementation

curl -X POST -H "Authorization: key=<YOUR-SERVER-KEY>" -H "Content-Type: application/json" -d '{
  "notification": {
    "title": "Portugal vs. Denmark",
    "body": "5 to 1",
    "icon": "firebase-logo.png",
    "click_action": "http://localhost:8081"
  },
  "to": "<THE-TOKEN-GENERATED-ON-THE-FRONTEND-APPLICATION>"
}' "https://fcm.googleapis.com/fcm/send"


curl -X POST -H "Authorization: key=AAAAQ9K_Jaw:APA91bGTMOmluMxkZw8myG4Vm0F5VMT4H0GLejgVAFEKXnArtE7fKaUnt_dKYXG78O0N4mwhJZ0jTMAhmXVX914ZCPhjwR_MpECvCphCETjhMhwlWqzZPoyNIDdBDcplBWP0eIfpcCiD" -H "Content-Type: application/json" -d '{
  "notification": {
    "title": "Portugal vs. Denmark",
    "body": "5 to 1",
    "icon": "firebase-logo.png",
    "click_action": "http://localhost:8081"
  },
  "to": "f3oWBQh4ors:APA91bGGUTuu2t_TkrGkuvCfnTzGwNsAIiDSNzkxwHnjdkqlxySYS47P8WdsLZBd5OQR4VNHFFAjeiLAKmioLDZS0DFjXx55RipdpiOj2qBNVT7qKVa5Jdj7c8NbeakHFUviIwXIuGeA"
}' "https://fcm.googleapis.com/fcm/send"