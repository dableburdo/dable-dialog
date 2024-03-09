# dable-dialog

# Install
```
npm install dable-dialog
```

# Sample
```html
<setting>
    <tag load="dable-dialog">Dialog</tag>
</setting>

<script run=after>
dlg.visible(true);
</script>

<script run=init>
let btn_evt = (b1,b2,b3) => {
    console.log(b1.text().text());
    dlg.visible(false);
}
</script>

<Dialog name=dlg size=(3rem,3rem) button-event=@btn_evt>
    <title>"Dialog"</title>
    <button>OK</button>
    <button>Cancel</button>
</Dialog>
```

# Parameter

| Short<br>Form | Parameter Name | Type | Description |
|:-------------:|:---------------|:-----|:------------|
| ◯  | title | mixed | string: title text |
| | | | dable-text: title text component |
| | | dict | text config |
| | button | mixed | string: button text |
| | | | dable-button: dialog button component |
| | | dict | button config  |
| | buttonEvent | function | button event |
| | | mixed | event parameter |
| | closeComp | component | dialog close component |
| | frame | dable-frame | dialog frame component |
| | mainColor | mixed | string: color name, #hex |
| | | | array: [red, green, blue, (alpha)] |
| | | option | style option |
| | accentColor | mixed | string: color name, #hex |
| | | | array: [red, green, blue, (alpha)] |
| | | option | style option |
| | height | string (size) | dialog height |
| | | | undefined: call as getter |
| | | dict | set size option |
| | headerHeight | string(size) | header height |
| | | | undefined: call as getter |
| | | dict | set size option |
| | width | string (size) | dialog width |
| | | | undefined: call as getter |

