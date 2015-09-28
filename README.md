# jquery-seekbar
JQuery seekbar/slider script

# Example of use
```html
<div id="seekbar-container-vertical-red" style="width:50px;height:300px;float:left;margin-right:20px"></div>
```

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