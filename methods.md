# Defining Methods

Methods allow you to smoothly display code examples in different languages.

{% method %}
## init

Initializes the DSK

{% sample lang="swift" %}
Init the SDK using Swift.

```swift
TracxSDK.shared.init("your app id here")
```

{% sample lang="java" %}
Init the SDK using Java.

```java
TracxSDK.shared.init("your app id here");
```



{% common %}
Whatever language you are using, the result will be the same.

```bash
$ My first method
```
{% endmethod %}

{% method %}
## Login with user

Logs in with given TracxUser.



```swift
TracxUser has the following properties:
firstName : String
lastName
birthdate
clubID
personalID
email
mobilePhoneNumber
homePhoneNumber
address
```



{% sample lang="swift" %}

```swift
let user = TracxUser()
user.firstName = "first name"
user.lastName = "last name"
user.clubId = "12345678"
user.personalID = "0123456789"
user.birthdate = "2017-08-13" //ISO 8601 date format YYYY-MM-DD
user.email = "mail@gmail.com"
user.mobilePhoneNumber = "+9725412345678"
user.homePhoneNumber = "0412345678"
user.address = TracxAddress(country: "Israel", city: "Tel aviv", street: "Allenby", streetNumber: 20, appartmentNumber: 1, mailbox: 1, zipCode: 1234567)

TracxSDK.shared.login(user)
```

{% sample lang="java" %}

```java
TracxUser user = new TracxUser();
user.firstName = "first name";
user.lastName = "last name";
user.clubId = "12345678"
user.personalID = "0123456789"
user.birthdate = "2017-08-13"; //ISO 8601 date format YYYY-MM-DD
user.email = "mail@gmail.com";
user.mobilePhoneNumber = "+9725412345678";
user.homePhoneNumber = "0412345678";
user.address = new TracxAddress("Israel", "Tel aviv", "Allenby", 20, 1, 1, 1234567);

TracxSDK.shared.presentTracxpointActivity();
```



{% common %}
Whatever language you are using, the result will be the same.

```bash
$ My first method
```
{% endmethod %}


{% method %}
## OpenTracxpointTerminal

Launches Tracxpoint QR code reader take or return cart from the terminal

{% sample lang="swift" %}
Presents the Tracxpoint ViewController

```swift
TracxSDK.shared.presentTracxpointViewController()
```

{% sample lang="java" %}
Opens the Tracxpoint Activity

```java
TracxSDK.shared.presentTracxpointActivity();
```



{% common %}
Whatever language you are using, the result will be the same.

```bash
$ My first method
```
{% endmethod %}
