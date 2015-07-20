# jQuery.vitrine.js
a jQuery plugin used for display items in a vitrine effect

like this:

![](http://vkki.qiniudn.com/vitrine.gif)

# Usage

Import the ```vitrine.js``` file after the jQuery lib:

```html
<script src="jquery.min.js"></script>
<script src="jquery.vitrine.js"></script>
```

Arrange DOM like this:

```html
<div id="vitrine">
    <div data-desc="不丹"><img src="1.png"></div>
    <div data-desc="贵州"><img src="2.png"></div>
    <div data-desc="重庆"><img src="3.png"></div>
    <div data-desc="尼泊尔"><img src="4.png"></div>
    <div data-desc="四川"><img src="5.png"></div>
    <div data-desc="西藏"><img src="6.png"></div>
    <div data-desc="云南"><img src="7.png"></div>
</div>
```

Use ```data-desc``` attribute to describe items.

Then use this code to call vitrine:

```$('#vitrine').vitrine({title:'已开启区域',color:'#fff'});} ```

# Options: default value

#### start: null

Set which item will be displayed at the center after initialization, starts with 0.
When set to null, the plugin will use the item in the middle as center item.

#### narrow: false

Set whether use narrow mode or not: in narrow mode only 3 item will be displayed at same time, and 5 otherwise.
The plugin will use narrow mode automatically when the quantity of item in DOM is less than 5.

#### speed: 400

Set the animation duration in millisecond.

#### loop: false

Allow loop.

#### title: ''

Set the title of vitrine, in the demo above, it's '已开启区域'.

#### color: '#000'

Set the color of title and item decription.
