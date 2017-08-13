# Defining Methods

Methods allow you to smoothly display code examples in different languages.

{% method %}
## init

Initializes the DSK

{% sample lang="swift" %}
Init the SDK using Swift.

```swift
TracxSDK.init("your app id here")
```

{% sample lang="java" %}
Init the SDK using Java.

```java
TracxSDK.init("your app id here");
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
