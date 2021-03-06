Facebook-LikeButton
===================

A small library to make it easier to create Facebook Like buttons and track clicks on them. This library is released under the MIT license. Check out the [demo](http://jonyt.github.com/Facebook-LikeButton/demo.html).

```
var likeCallback = function(response){ // Callback will be invoked when user presses 'Like'
    console.log(response)
};
// Parameters are: URL to like, settings, callback, appId, channel file URL
var fbl = LikeButton.create('http://www.facebook.com', {}, likeCallback, YOUR_APP_ID, PATH_TO_CHANNEL_FILE);           
document.getElementsByTagName('body')[0].appendChild(fbl);
```

OR

```
// Parameters are: URL to like, settings, callback, appId, channel file URL
var fbl = LikeButton.create('http://www.facebook.com');         
document.getElementsByTagName('body')[0].appendChild(fbl);
```

*Note*: available settings are hasFaces (`boolean`), hasSendButton (`boolean`), layout (one of `standard`, `button_count`, `box_count`), verb (`like` or `recommend`) and width (`number`).
