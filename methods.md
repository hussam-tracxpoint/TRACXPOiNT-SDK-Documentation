# Defining Methods

Methods allow you to smoothly display code examples in different languages.

{% method %}
## init

Initializes the SDK with your provided unique app id.

{% sample lang="swift" %}
Init the SDK using Swift.

```swift
TracxpointSDK.sharedInstance.initSdk("your app id here")
```

{% sample lang="java" %}
Init the SDK using Java.

```java
TracxpointSDK.sharedInstance.initSdk("your app id here");
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


**TracxUser:**
```
firstName (string)
lastName (string)
birthdate (string) ISO 8601 date format YYYY-MM-DD
clubID (string)   
personalID (string)
email (string)
mobilePhoneNumber (string)
homePhoneNumber (string)
address (TracxAddress)
```
**TracxAddress:**
```
country (string)
city (string)
street (string)
streetNumber (string)
appartmentNumber (string)
mailbox (string)
zipCode (string)
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

TracxpointSDK.sharedInstance.login(user)
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

TracxpointSDK.sharedInstance.presentTracxpointActivity();
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
TracxpointSDK.sharedInstance.presentTracxpointViewController()
```

{% sample lang="java" %}
Opens the Tracxpoint Activity

```java
TracxpointSDK.sharedInstance.presentTracxpointActivity();
```



{% common %}
Whatever language you are using, the result will be the same.

```bash
$ My first method
```
{% endmethod %}
