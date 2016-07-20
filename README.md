# [iziModal](http://izimodal.dolce.ninja)
Elegant, responsive, flexible and lightweight modal plugin with jQuery.

[**izimodal**.marcelodolce.com](http://izimodal.marcelodolce.com)

![capa](http://i.imgur.com/TPdnES8.png)

[logo]: http://i.imgur.com/hCYIhep.png "Check icon"

[new]: http://i.imgur.com/41zuVDk.png "New label"
[bug]: http://i.imgur.com/92lu4ln.png "Bug label"

Fast | Responsive | Animated | Lightweight | Customizable | All modern browsers | Retina Display
:-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :-----:
![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo]


___
### Version Log

- **v1.2.0**
  - ![alt text][new] Retina display support - *Implemented.*
  - ![alt text][bug] Callbacks had no access to modal functions - *Fixed.*

- **v1.1.0**
  - ![alt text][new] feature to apply fullscreen - *Implemented.*
  - ![alt text][new] timeout feature with progress bar - *Implemented.*

- **v1.0.1**
  - ![alt text][bug] *overlayClose* only works the first time - *Fixed.*

___
### Install

#### [npm](https://www.npmjs.com/package/izimodal)
```
npm install izimodal --save
```

#### bower
```
bower install izimodal
```




___
### Data Attributes
- Add *data-izimodal-close* to any button or link inside the modal will close it when clicked.
```html
<button data-izimodal-close>Close</button>
```
- Add *data-izimodal-fullscreen* to any button or link inside the modal will expand it when clicked.
```html
<button data-izimodal-fullscreen>Maximize</button>
```

___
### Default Options

```javascript
$("#modal").iziModal({
    title: '',
    subtitle: '',
    theme: '',
    headerColor: '#88A0B9',
    overlayColor: 'rgba(0, 0, 0, 0.4)',
    iconColor: '',
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
    fullscreen: false,
    openFullscreen: false,
    timeout: false,
    timeoutProgressbar: false,
    timeoutProgressbarColor: 'rgba(255,255,255,0.5)',
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


Argument | Default Value | Description
:---: | :---: | ---
**title** | *""* | Title that appears in the modal header.
**subtitle** | *""* | Caption that appears in the header below the title.
**theme** | *""* | Caption that appears in the header below the title.
**headerColor** | *#6d7d8d* | Color to fill the header background, will also be applied to the bottom edge of the modal.
**iconClass** | *null* | Icon class (font-icon of your choice) that will be displayed in modal header.
**headerColor** | *#6d7d8d*	 | Color to fill the header background, will also be applied to the bottom edge of the modal.
**overlayColor** | *rgba(0,0,0,0.4)* | Color overlay.
**width** | *600* | Fixed width of the modal. You can use %, px, em or cm. If not using an unit of measure. It will be taken over the px unit.
**padding** | *0* | Margin that will be applied to the inside of the modal.
**iframe** | *false* | Set true to apply an iframe inside the modal.
**iframeHeight** | *null* | Fixed height of the iframe.
**iframeURL** | *null* | Address that will open in the iframe inside the modal, if not set, the user can alternatively use the href link responsible for opening it.
**overlayClose** | *true* | If set true, you can close the modal just by clicking on the outer layer of dark modal.
**closeOnEscape** | *true* | If set true, you can close the modal only pressing the escape key.
**bodyOverflow** | *false* | Forcing overflow hidden in the document when opening the modal, closing the modal, overflow will be restored.
**focusInput** | *true* | If set true, whenever you open a modal, the first visible field is active.
**autoOpen** | *false* | 	If set true, the modal opens automatically without any user action.
**fullscreen** | *false* | 	Allow button in header modal to expand.
**openFullscreen** | *false* | 	Force to open modal in fullscreen.
**timeout** | *0 or false* | 	Amount in milliseconds to close the modal or false to disable.
**timeoutProgressbar** | *false* | 	Enable progress bar of timeout.
**timeoutProgressbarColor** | *rgba(255,255,255,0.5)* | 	Progress bar color.
**transitionInModal** | *transitionIn* | Modal opening default transition.
**transitionOutModal** | *transitionOut* | Modal closing default transition.
**transitionInOverlay** | *fadeIn* | Default transition of overlay opening.
**transitionOutOverlay** | *fadeOut* | Default transition of overlay closure.
**onOpening** | *function() {}*	 | Callback function that will run when opening the modal.
**onOpened** | *function() {}*	 | Callback function that will run when the modal is open.
**onClosing** | *function() {}*	 | Callback function that will run when closing the modal.
**onClosed** | *function() {}*	 | Callback function that will run when the modal is closed.


___
### Methods

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
### Events

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
