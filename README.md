# Firebase-JavaScript

### Koneksi antara Javascript dan Firebase<br/>
```javascript
    <script id="MainScript">
      var firebaseConfig = {
        apiKey: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
        authDomain: "xxxxxxxxxxxxxxxxxxxxxxx",
        databaseURL: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
        projectId: "xxxxxxxxxx",
        storageBucket: "xxxxxxxxxxxxxxxxxxx",
        messagingSenderId: "xxxxxxxxxxxxx",
        appId: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
      };
      firebase.initializeApp(firebaseConfig);
```
### Jika ingin memanggil item/value dari ID html dapat menggunakan potongan program dibawah<br/>

```javascript
var xxx = document.getElementById("namaid");
```
### Retrieve atau mengambil data dari Firebase<br/>
```javascript
    var dbRef = firebase.database().ref().child("nama_child").on("value", (snap) => (nama_var_id.innerText = snap.val()));
```
### Set atau mengirim data ke Firebase<br/>
```javascript
    firebase.database().ref("nama_child").set("Value");
```
<br />
Enjoy!!!
<br />
<br />
<br />
<br />

###### Author

ASNProject<br />
email: asnproject02@gmail.com
