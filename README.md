# [iziModal](http://izimodal.dolce.ninja)
[![CDNJS](https://img.shields.io/cdnjs/v/izimodal.svg)](https://cdnjs.com/libraries/izimodal)

Elegant, responsive, flexible and lightweight modal plugin with jQuery.

[**izimodal**.marcelodolce.com](http://izimodal.marcelodolce.com)

![capa](http://i.imgur.com/TPdnES8.png)

[logo]: http://i.imgur.com/hCYIhep.png "Check icon"

[new]: http://i.imgur.com/41zuVDk.png "New label"
[bug]: http://i.imgur.com/92lu4ln.png "Bug label"

Fast | Responsive | Animated | Lightweight | Customizable | History | Group Mode | Retina
:-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: 
![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo] | ![alt text][logo]


- All modern browsers are supported (Tested in Chrome, Firefox, Opera, Safari, IE9+ and Edge).
- Bugs? create an issue [here](https://github.com/dolce/iziModal/issues).

___
### Version Log

- **v1.5.0**
  
  - ![alt text][new] AMD support - *Implemented.*
  - ![alt text][new] closeButton option - *Implemented.*
  - ![alt text][new] appendTo option - *Implemented.*
  - ![alt text][new] Static margin (Top and Bottom options) - *Implemented.*
  - ![alt text][new] Namespace  - *Implemented.*
  - ![alt text][new] Improvements when using Modal in flexbox layouts - *Implemented.*
  - ![alt text][bug] Scroll iframe on iOS - *Fixed.*
  - ![alt text][bug] Some kinds of Data-attr do not work as they should - *Fixed.*
  - ![alt text][bug] Incompatibility with iziToast animations - *Fixed.*
  - ![alt text][bug] Methods setTransitionIn and setTransitionOut - *Fixed.*
  - ![alt text][bug] Modal closes when use shortcut arrows - *Fixed.*
  - ![alt text][bug] Modal loses its classes when closed - *Fixed.*
  - ![alt text][bug] Modal loses option RTL when closed - *Fixed.*
  - ![alt text][bug] Modal loses reference if it does not have an ID - *Fixed.*


- **v1.4.2**
  - ![alt text][new] All the options can now be used through the data-iziModal-optionName attribute - *Implemented.*
  - ![alt text][bug] Inaccurate modal height calculation - *Fixed.*
  - ![alt text][bug] The Light theme was not applied correctly - *Fixed.*

- **v1.4.0/1.4.1**
  - ![alt text][new] RTL support - *Implemented.*
  - ![alt text][new] WAI-ARIA support - *Implemented.*
  - ![alt text][bug] An error occurred if there was a hash did not belong to the modal - *Fixed.*
  - ![alt text][bug] It breaks the layout if "iziModal" class is missing - *Fixed.*
  - ![alt text][bug] The vertical positioning of the modal, sometimes was not applied correctly - *Fixed.*
  - ![alt text][bug] Transitions of modals positioning do not behave correctly - *Fixed.*
  - ![alt text][bug] The modals group navigation did not work correctly If any modal was destroyed - *Fixed.*

- **v1.3.3**
  - ![alt text][new] Text icons support (option, data-attr and set method)  - *Implemented.*
  - ![alt text][bug] History was always active on mobile - *Fixed.*
  - ![alt text][bug] It was not possible to instantiate multiple modals at once - *Fixed.*

- **v1.3.2**
  - ![alt text][new] setGroup to set new group name - *Implemented.*
  - ![alt text][bug] group option work in some cases - *Fixed.*

- **v1.3.1**
  - ![alt text][bug] iframe URL (by event like click) not work with append childs - *Fixed.*
  - ![alt text][bug] Widths with percentage does not work - *Fixed.*

- **v1.3.0**
  - ![alt text][new] History support - *Implemented.*
  - ![alt text][new] Group support (data-iziModal-group) with caption and navigation - *Implemented.*
  - ![alt text][new] Methods next and prev to be used on group mode - *Implemented.*
  - ![alt text][new] Option Loop and data (data-iziModal-loop)  - *Implemented.*
  - ![alt text][new] Option pauseOnHover when you have timeout - *Implemented.*
  - ![alt text][new] Other Transitions and improvements in CSS - *Implemented.*
  - ![alt text][new] Methods setTransitionIn and setTransitionOut - *Implemented.*
  - ![alt text][new] data-iziModal-transitionIn and data-iziModal-transitionOut to triggers and modals - *Implemented.*
  - ![alt text][new] radius Option, zindex Option and method setZindex - *Implemented.*
  - ![alt text][new] Open and Close methods they can be used with different animations - *Implemented.*
  - ![alt text][new] data-iziModal-open="modal-id" - *Implemented.*
  - ![alt text][new] data-iziModal-title, data-iziModal-subtitle and data-iziModal-icon - *Implemented.*
  - ![alt text][new] Callbacks onResize and onFullscreen - *Implemented.*
  - ![alt text][new] Event fullscreen and Global Event iziModal-group-change - *Implemented.*
  - ![alt text][new] autoOpen option with delay - *Implemented.*
  - ![alt text][new] attached option, top or bottom - *Implemented.*
  - ![alt text][bug] return of the methods were always overwritten - *Fixed.*
  - ![alt text][bug] Overflow in fullscreen and other minor fixes in js structure - *Fixed.*


- **v1.2.0**
  - ![alt text][new] Retina display support - *Implemented.*
  - ![alt text][bug] Callbacks had no access to modal functions - *Fixed.*

- **v1.1.0**
  - ![alt text][new] feature to apply fullscreen - *Implemented.*
  - ![alt text][new] timeout feature with progress bar - *Implemented.*

- **v1.0.1**
  - ![alt text][bug] overlayClose only works the first time - *Fixed.*

___
### Use

#### [CDNJS](https://cdnjs.com/libraries/izimodal)
https://cdnjs.com/libraries/izimodal

### Install

#### [npm](https://www.npmjs.com/package/izimodal)
```
npm install izimodal --save
```

#### bower
```
bower install izimodal
```

#### [GEM](https://github.com/elitenomad/izimodal)
```
gem install izimodal
```




___
### Data Attributes

- Add **data-izimodal-open** to any button or link inside or outsite the modal will open it when clicked.
```html
<button data-izimodal-open="modal-id">Open</button>
<!-- Specifying the opening transition -->
<button data-izimodal-open="modal-id" data-izimodal-transitionin="fadeInDown">Open</button>
```

- Add **data-izimodal-close** to any button or link inside the modal will close it when clicked.
```html
<button data-izimodal-close="">Close</button>
<!-- Specifying the closing transition -->
<button data-izimodal-close="" data-izimodal-transitionout="bounceOutDown">Close</button>
```

- Add **data-izimodal-fullscreen** to any button or link inside the modal will expand it when clicked.
```html
<button data-izimodal-fullscreen>Maximize</button>
```


- Closes the current and open the **Next** modal.
```html
<button data-izimodal-next>Next Modal</button>
```
- Closes the current and open the **Previous** modal.
```html
<button data-izimodal-prev>Previous Modal</button>
```

#### Data-attr to Modal

- Add **data-izimodal-group** to div of the modal for build a group with everyone involved.
```html
<div id="modal" class="iziModal" data-izimodal-group="alerts"></div>
```

- Sets **Loop** for the same modals in the group.
```html
<div id="modal" class="iziModal" data-izimodal-loop></div>
```

- Update v1.4.2+

#### ![alt text][new] Now all options can be set via data-attrs.





___
### Default Options

```javascript
$("#modal").iziModal({
    title: '',
    subtitle: '',
    headerColor: '#88A0B9',
    theme: '',  // light
    attached: '', // bottom, top
    appendTo: '.body', or false
    icon: null,
    iconText: null,
    iconColor: '',
    rtl: false,
    width: 600,
    top: null,
    bottom: null,
    padding: 0,
    radius: 3,
    zindex: 999,
    iframe: false,
    iframeHeight: 400,
    iframeURL: null,
    focusInput: true,
    group: '',
    loop: false,
    navigateCaption: true,
    navigateArrows: true, // Boolean, 'closeToModal', 'closeScreenEdge'
    history: true,
    restoreDefaultContent: false,
    autoOpen: 0, // Boolean, Number
    bodyOverflow: false,
    fullscreen: false,
    openFullscreen: false,
    closeOnEscape: true,
    closeButton: true,
    overlay: true,
    overlayClose: true,
    overlayColor: 'rgba(0, 0, 0, 0.4)',
    timeout: false,
    timeoutProgressbar: false,
    pauseOnHover: false,
    timeoutProgressbarColor: 'rgba(255,255,255,0.5)',
    transitionIn: 'comingIn',
    transitionOut: 'comingOut',
    transitionInOverlay: 'fadeIn',
    transitionOutOverlay: 'fadeOut',
    onFullscreen: function(){},
    onResize: function(){},
    onOpening: function(){},
    onOpened: function(){},
    onClosing: function(){},
    onClosed: function(){}
});
```


Argument | Default Value | Description
:---: | :---: | ---
**title** | *''* | Title in modal's header.
**subtitle** | *''* | Caption below modal's title.
**headerColor** | *'#6d7d8d'* | Color to fill the header background, will also be applied to the bottom edge of the modal.
**theme** | *''* | Theme of the modal, can be empty or **light**.
**attached** | *''* | Attach the modal at the **top** or **bottom** of the screen.
**appendTo** | *'.body'* | Where the modal will be placed?
**icon** | *null* | Icon class (font-icon of your choice) that will be displayed in modal header.
**iconText** | *null* | Icon text (font-icon using text) that will be displayed in modal header.
**iconColor** | *''* | Color of the header icon.
**rtl** | *false* | Right To Left option.
**width** | *600* | Fixed width of the modal. You can use %, px, em or cm. If not using a measure unity, PX will be assumed as measurement unit.
**top** | *null* | Top static margin.
**bottom** | *null* | Bottom static margin.
**padding** | *0* | Modal inner margin.
**radius** | *3* | Border-radius that will be applied in modal.
**zindex** | *999* | The z-index CSS attribute of the modal.
**iframe** | *false* | If true, an Iframe will be used inside the modal.
**iframeHeight** | *400* | Fixed height of the iframe.
**iframeURL** | *null* | Address that will open in the iframe inside the modal, if not set, the user can alternatively use the href link responsible for opening it.
**focusInput** | *true* | If set true, whenever you open a modal, the first visible field is active.
**group** | '' | Create a group with same 'group' name, so can navigate between them.
**loop** | *false* | It allows loop with modals of the same group.
**navigateCaption** | *true* | Displays arrows to navigate.
**navigateArrows** | *true* | Change arrows position to navigate between the modals. It can be: 'closeToModal' or 'closeScreenEdge'.
**history** | *true* | Enable browsing history.
**restoreDefaultContent** | *false* | Reset the modal to default to be opened again. 
**autoOpen** | *0 or false* | If true, the modal opens automatically with any user action. Or you can set a delay time (in milliseconds) to open.
**bodyOverflow** | *false* | Forcing overflow hidden in the document when opening the modal, closing the modal, overflow will be restored.
**fullscreen** | *false* | 	Show a button in modal header to expand.
**openFullscreen** | *false* | 	Force to open modal in fullscreen.
**closeOnEscape** | *true* | If set true, you can close the modal only pressing the escape key.
**closeButton** | *true* | Display close button in the header.
**overlay** | *true* | Enable or disable background overlay.
**overlayClose** | *true* | If set true, the modal will be closed clicking outside of it.

**overlayColor** | *'rgba(0,0,0,0.4)'* | Color overlay.
**timeout** | *0 or false* | 	Amount in milliseconds to close the modal or false to disable.
**timeoutProgressbar** | *false* | Enable timeout progress bar.
**timeoutProgressbarColor** | *'rgba(255,255,255,0.5)'* | Progress bar color.
**pauseOnHover** | *false* | Pause the progress bar when mouse cursor hover the modal.
**transitionIn** | *'comingIn'* | Modal opening default transition. Can be: <b>comingIn, bounceInDown, bounceInUp, fadeInDown, fadeInUp, fadeInLeft, fadeInRight, flipInX</b>.
**transitionOut** | *'comingOut'* | Modal closing default transition. Can be: <b>comingOut, bounceOutDown, bounceOutUp, fadeOutDown, fadeOutUp, , fadeOutLeft, fadeOutRight, flipOutX</b>.
**transitionInOverlay** | *'fadeIn'* | Default transition of overlay opening.
**transitionOutOverlay** | *'fadeOut'* | Default transition of overlay closure.
**onFullscreen** | *function() {}*	 | Callback function that will run when the modal enable or disable full screen.
**onResize** | *function() {}*	 | Callback function that will be executed when a resize occurs.
**onOpening** | *function() {}*	 | Callback function that will run when opening the modal.
**onOpened** | *function() {}*	 | Callback function that will run when the modal is open.
**onClosing** | *function() {}*	 | Callback function that will run when closing the modal.
**onClosed** | *function() {}*	 | Callback function that will run when the modal is closed.


___
### Methods

- **Instantiating** - Catching instance of modal
```javascript
var modal = $('#modal').iziModal();
// then you can use:
// modal.iziModal('open');
```

- **Open** - Opens the modal window.
```javascript
$('#modal').iziModal('open');
 
// or with a specific transition of entry.
 
$('#modal').iziModal('open', {
    transition: 'fadeInDown' // Here transitionIn is the same property.
});
 
// or with a specific transition of entry and output.
 
$('#modal').iziModal('open', {
    transitionIn: 'bounceInDown'
    transitionOut: 'bounceOutDown' // TransitionOut will be applied if you have any open modal.
});
```

- **Close** - Closes the modal window.
```javascript
$('#modal').iziModal('close');
 
// or with a specific transition of output.
 
$('#modal').iziModal('close', {
    transition: 'bounceOutDown' // Here transitionOut is the same property.
});
```

- **Toggle** - Change to the opposite of the current state.
```javascript
$('#modal').iziModal('toggle');
```

- **getState** - Returns a current state of the modal.
```javascript
/**
 * @returns {'closed'|'closing'|'opened'|'opening'}
 */
$('#modal').iziModal('getState');
```

- **getGroup** - Returns group information.
```javascript
$('#modal').iziModal('getGroup');
```

- **setGroup** - Set a new group name.
```javascript
$('#modal').iziModal('setGroup', 'alerts');
```

- **Next** - Skip to next modal to the same group.
```javascript
$('#modal').iziModal('next');
 
// or with a specific transition of output.
 
$('#modal').iziModal('next' ,{
    transitionIn: 'bounceInDown'
    transitionOut: 'bounceOutDown'
});
```

- **Prev** - Skip to previous modal to the same group.
```javascript
$('#modal').iziModal('prev');
 
// or with a specific transition of output.
 
$('#modal').iziModal('prev' ,{
    transitionIn: 'bounceInDown'
    transitionOut: 'bounceOutDown'
});
```

- **startLoading** - Start overlay loading within the modal.
```javascript
$('#modal').iziModal('startLoading');
```

- **stopLoading** - Stop overlay loading within the modal.
```javascript
$('#modal').iziModal('stopLoading');
```

- **Destroy** - Destroys the modal instance.
```javascript
$('#modal').iziModal('destroy');
```

- **setHeaderColor** - Apply the background color in modal header.
```javascript
$('#modal').iziModal('setHeaderColor', 'color');
```

- **setTitle** - Change the title of the modal.
```javascript
$('#modal').iziModal('setTitle', 'Title');
```

- **setSubtitle** - Change the subtitle of the modal.
```javascript
$('#modal').iziModal('setSubtitle', 'Subtitle');
```

- **setIcon** - Change the class of icon.
```javascript
$('#modal').iziModal('setIcon', 'icon-home');
```

- **setIconText** - Change the text of font icon.
```javascript
$('#modal').iziModal('setIconText', 'icon');
```

- **setZindex** - Change the z-index CSS attribute of the modal.
```javascript
$('#modal').iziModal('setZindex', 999);
```

- **setTransitionIn** - Change the Modal opening transition.
```javascript
$('#modal').iziModal('setTransitionIn', 'comingIn');
// comingIn, bounceInDown, bounceInUp, fadeInDown, fadeInUp, fadeInLeft, fadeInRight, flipInX
```

- **setTransitionOut** - Change the Modal closing transition.
```javascript
$('#modal').iziModal('setTransitionOut', 'comingOut');
// comingOut, bounceOutDown, bounceOutUp, fadeOutDown, fadeOutUp, , fadeOutLeft, fadeOutRight, flipOutX
```

- **recalculateLayout** - Used to recalculate the placement and dimensions of the modal layout.
```javascript
$('#modal').iziModal('recalculateLayout');
```

___
### Events

- **Opening** - Capture when the modal is opening.
```javascript
$(document).on('opening', '#modal', function (e) {
    //console.log('Modal is opening');
});
```

- **Opened** - Capture when the modal is open.
```javascript
$(document).on('opened', '#modal', function (e) {
    //console.log('Modal is opened');
});
```

- **Closing** - Capture when the modal is closing.
```javascript
$(document).on('closing', '#modal', function (e) {
    //console.log('Modal is closing');
});
```

- **Closed** - Capture when the modal is closed.
```javascript
$(document).on('closed', '#modal', function (e) {
    // console.log('Modal is closed');
});
```

- **Fullscreen** - Capture when the modal enables or disables the full screen.
```javascript
$(document).on('fullscreen', '#modal-default', function (e, modal) {
    if(modal.isFullscreen){
        // Enabled
    } else {
        // Disabled
    }
});
```

- **iziModal-group-change** - Capture when a modal opens and closes within a group.
```javascript
$(document).on('iziModal-group-change', function (e, modal) {
    console.info(modal.in); // Modal that came in.
    console.info(modal.out); // Modal that came out.
});
```
