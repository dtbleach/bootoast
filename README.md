# Bootoast 🔥
## A [*Boot*][0]strap T[*oast*][1]er Plugin
Toast notifications with **Bootstrap 3 or 4** `alert`s.

### [Demo!][3]

### Default Settings

```javascript
bootoast({
    message: 'Helo!',
    type: 'info',
    position: 'bottom-center',
    icon: undefined,
    timeout: false,
    animationDuration: 300,
    dismissible: true
});
```

### Options Settings

To use your own settings, take the default example above and replace with your values. You can also remove the keys you will not change.

Option | Default Value | Descrition
:--- | :--- | :---
`message` | `'Helo!'` | Any, **any**, HTML String!
`type` | `'info'` | A raw string that can be any of Bootstrap 3 alert type classes without the `alert-` preffix. [Available types](#types).
`icon` | based on choosen `type` OR `undefined` | An icon following the standard Bootstrap 3 glyphicons name without the `glyphicon-` preffix. [Icons choosen by type](#icon-defaults).
`position` | `'bottom-center'` | A raw string with two segments of align separated by hypehn follo0wing the pattern: `vertical-horizontal`. [Supported positions](#supported-positions).
`timeout` | `false` | The time in seconds for hide the notification (`.alert` element). If `false` or `0`, the notification will not auto-hide. 
`dismissible` | `true` | Shows or hides the dismiss &times; button. It can be `true` or `false`.
`animationDuration` | `300` | The notification hide animation duration in milliseconds (`ms`).

#### Supported Types

By default, Bootoast supports all [Bootstrap 3 alert types][2]:

* info
* success
* warning
* danger
 
 [See more about Bootsrap `alert`s][2].
 


#### Supported Positions

Supported | Sinonymus
:---: | :---:
`top-center` | `top`
`top-left` | `left-top`
`top-right` | `right-top`
`bottom-center` | `bottom`
`bottom-left` | `left-bottom`
`bottom-right` | `right-bottom`


#### Icon Defaults

By default, if it's not defined, it will turn into an icon choosen by the type:

Bootoast type | Bootstrap icon
:---: | :---:
warning | exclamation-sign
success | ok-sign
danger | remove-sign
info | info-sign

----

Good Luck. :-)


[0]: https://getbootstrap.com/docs/3.3/
[1]: github.com/odahcam/bootoast
[2]: https://getbootstrap.com/docs/3.3/components/#alerts
[3]: https://codepen.io/odahcam/full/oeoYxm
