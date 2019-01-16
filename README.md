# angular-firebase-service-docs

## API

### logEvent( string eventName, Object params ): Observable\<boolean\>

logEvent to the firebase analytics

```js
...
  constructor(private firebaseAnalytics: FirebaseAnalyticsService) {}
  
  ngOnInit() {
    this.firebaseAnalytics.logEvent( "screen_view", {...params} );
  }
...
```

### setUser( string uuid ): Observable\<boolean\>

set current user to track his activity. 

```js
  ...
    this.firebaseAnalytics.logEvent( Device.uuid );
  ...
```

### setScreen( string screenName ): Observable\<boolean\>

set current screen to check activity

```js
  ...
    this.firebaseAnalytics.setScreen( screenName );
  ...
```
