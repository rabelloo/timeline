# timeline
CSS pattern design for Timelines

## Usage

```html
<div class="timeline bottom" data-progress="66">
  <ul>
    <li>
      <span class="timespan">
        Optional timespan detail, like "3 hours ago"
      </span>
      <input id="timeline1" readonly>
      <label for="timeline1">
        <i class="icon"></i>
      </label>
      <div>
        Hidden content
      </div>
    </li>
    <li>
      ...
    </li>
    <li>
      ...
    </li>
  </ul>
</div>
```

The `.timeline` element will define styles. It only has one children, a list with every `li` being a **timeline item**.

**The `[data-progress]` attribute will define how much of the `timeline`'s progress bar is filled.**

## Options

| Element | Type | Description |
| --- | --- | --- |
| `.timespan` | Optional | Suggested for lightly indicating time since event's ocurrence. May be used to display other info. |
| `<input>` | Optional | Provides support for keyboard navigation. Use its `[id]` coupled with `<label>`'s `[for]`. |
| `<label>` | Mandatory | `timeline item`'s main display. Suggested use with `.icon`. Its attribute `[for]` is only needed to couple with `<input>`'s `[id]` attribute for keyboard navigation. |
| `.icon` | Optional | Display for `timeline item`'s `icon`. Can be replaced with your markup of choice |
| `<div>` | Optional | Hidden content to fade in on `<label>`'s `hover` or `<input>`'s `focus` |

**Additionaly, you can choose the hidden `<div>`'s position by adding one of the classes `top`, `right`, `bottom` or `left` to the `.timeline` element.**
