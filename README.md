# [iziModal](http://izimodal.dolce.ninja)
Elegant, complete and lightweight modal plugin with jQuery

[**izimodal**.marcelodolce.com](http://izimodal.marcelodolce.com)




[logo]: http://i.imgur.com/hCYIhep.png "Check icon"



Fast | Responsive | Animated | Lightweight | Customizable | All modern browsers
:---: | :---: | :---: | :---: | :---: | :---:
![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo]





___
#### Default Options

```javascript
$("#modal").iziModal({
    title: "",
    subtitle: "",
    theme: "",
    headerColor: "#88A0B9",
    overlayColor: "rgba(0, 0, 0, 0.4)",
    iconColor: "",
    iconClass: null,
    width: 600,
    padding: 0,
    iframe: false,
    iframeHeight: 400,
    iframeURL: null,
    overlayClose: true,
    closeOnEscape: true,
    bodyOverflow: false,
    focusInput: true,
    autoOpen: false,
    transitionInModal: 'transitionIn',
    transitionOutModal: 'transitionOut',
    transitionInOverlay: 'fadeIn',
    transitionOutOverlay: 'fadeOut',
    onOpening: function() {},
    onOpened: function() {},
    onClosing: function() {},
    onClosed: function() {}
});
```

___
#### Methods

- *Instantiating*
```javascript
$('#modal').iziModal();
```

- *Open*
```javascript
$('#modal').iziModal('open');
```

- *Close*
```javascript
$('#modal').iziModal('close');
```

- *getState*
```javascript
/**
 * @returns {'closed'|'closing'|'opened'|'opening'}
 */
$('#modal').iziModal('getState');
```

- *startLoading*
```javascript
$('#modal').iziModal('startLoading');
```

- *stopLoading*
```javascript
$('#modal').iziModal('stopLoading');
```

- *Destroy*
```javascript
$('#modal').iziModal('destroy');
```

- *setHeaderColor*
```javascript
$('#modal').iziModal('setHeaderColor', 'color');
```

- *setTitle*
```javascript
$('#modal').iziModal('setTitle', 'Title');
```

- *setSubtitle*
```javascript
$('#modal').iziModal('setSubtitle', 'Subtitle');
```

- *setIconClass*
```javascript
$('#modal').iziModal('setIconClass', 'iconClass');
```

- *recalculateLayout*
```javascript
$('#modal').iziModal('recalculateLayout');
```

___
#### Events

- *Opening*
```javascript
$(document).on('opening', '#modal', function (e) {
    //console.log('Modal is opening');
});
```

- *Opened*
```javascript
$(document).on('opened', '#modal', function (e) {
    //console.log('Modal is opened');
});
```

- *Closing*
```javascript
$(document).on('closing', '#modal', function (e) {
    //console.log('Modal is closing');
});
```

- *Closed*
```javascript
$(document).on('closed', '#modal', function (e) {
    // console.log('Modal is closed');
});
```
