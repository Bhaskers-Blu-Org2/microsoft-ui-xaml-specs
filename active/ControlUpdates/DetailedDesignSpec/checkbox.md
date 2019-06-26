# Checkbox detailed design spec / redline

## The anatomy of checkbox
![anatomy](https://github.com/microsoft/microsoft-ui-xaml-specs/blob/user/chigy/ControlUpdates/active/ControlUpdates/DetailedDesignSpec/Images/Anatomy.png)
### Basic checkbox UI elements
Checkbox has the following UI elements that determines visuals:
1. The box fill
2. The box border
3. The glyph
4. The fill
5. Text

* The box border - 1px border (if we implement #835. Otherwise 2px). Rounded corner following #524 design.
* The glyph - 16px
* The fill - 8x8px
* Text - 14px (standard text size)

### Checkbox colors
Following colors are used to denote the state of the checkbox:
1. Fill color of the box
2. Foreground color of the border
3. Foreground color of the glyph
4. The fill color
5. Foreground color for the text

### Basic checkbox styles
Checkbox has mainly 3 styles:
1. Outline unselected
2. Fill selected
3. Fill unselected
Using these three basic styles on different controls based on typical use of the control, we create coherent experience for application surfaces.

![styles](https://github.com/microsoft/microsoft-ui-xaml-specs/blob/user/chigy/ControlUpdates/active/ControlUpdates/DetailedDesignSpec/Images/BaseDesign.png)

### Default color values

| State | 1. Outline unseledted | 2. Fill selected | 3. Fill unselected |
| :---------- | :------- | :------- | :------- |
| Rest | ||||
| Hover | ||||
| Pressed | ||||
| Disabled | ||||

## Controls that use Checkbox and style it uses

| Control | Unseledted | Selected |
| :---------- | :------- | :------- |
| CheckBox | Outline | Fill |
| ListItem | Outline | Fill |
| TreeView | Outline | Fill |
| GridView | Fill | Fill |
| RadioButton* | Outline | Fill |

*Even though RadioButton is not a checkbox, it needs to be following the system pattern to be coherent.