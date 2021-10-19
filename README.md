# Firebase-JavaScript

### Koneksi antara Javascript dan Firebase<br/>
```javascript
    <script id="MainScript">
      var firebaseConfig = {
        apiKey: "AIzaSyCOkbZJYFDDPZxoYt4VhkUEUjOaKMcGnLo",
        authDomain: "iotse-b1c10.firebaseapp.com",
        databaseURL: "https://iotse-b1c10-default-rtdb.firebaseio.com",
        projectId: "iotse-b1c10",
        storageBucket: "iotse-b1c10.appspot.com",
        messagingSenderId: "270480060594",
        appId: "1:270480060594:web:6cbccdbb40e653c14e99ab",
      };
      firebase.initializeApp(firebaseConfig);
```

<br/>
### Jika ingin memanggil item/value dari ID html dapat menggunakan potongan program dibawah
<br/>
```javascript
var xxx = document.getElementById("namaid");
```
<br/>
### Retrieve atau mengambil data dari Firebase 
```javascript
var dbRef = firebase.database().ref().child("nama_child").on("value", (snap) => (nama_var_id.innerText = snap.val()));
```
<br/>
### Set atau mengirim data ke Firebase
```javascript
firebase.database().ref("nama_child").set("Value");
```
