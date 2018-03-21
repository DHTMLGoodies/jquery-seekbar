# jquery-seekbar
JQuery seekbar/slider script

# Example of use

#Step 1:
Include files
```html
<script type="text/javascript" src="scripts/seekbar/js/jquery-1.11.2.min.js"></script>
<script type="text/javascript" src="scripts/seekbar/js/seekbar.js"></script>
<link rel="stylesheet" type="text/css" href="scripts/seekbar/css/seekbar.css"/>
```
#Step 2:
Create html:
```html
<div id="seekbar-container-vertical-red" 
style="width:50px;height:300px;float:left;margin-right:20px"></div>
```
#Step 3
Configure the widget
```Javascript
<script type="text/javascript">
     var redSlider = new Seekbar.Seekbar({
           renderTo: "#seekbar-container-vertical-red",
           minValue: 0, maxValue: 255,
           valueListener: function (value) {
               this.value = Math.round(value);
               updateColorPreview();
           },
           thumbColor: '#BBff0000',
           negativeColor: '#ff0000',
           positiveColor: '#CCC',
           value: 0
       });
</script>
```
# Methods
 `redSlider.setValue(number)` , set new value to a Seekbar.
 `redSlider.setEnable(boolean)` , disable/enable a Seekbar.
