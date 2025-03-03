---
name: Tooltip
category: Component
---

## Description

*Tooltips* can be added as a wrapper around another component and render a
small bubble on hover containing specific text

The tooltip can also be rendered on the bottom side of the element by adding
`--bottom` modifier.

```tooltip.css hidden
body > div.olt-Frame { padding-top: 30px; padding-bottom: 30px; }
```

```tooltip.html
Lorem ipsum dolor
<span class="olt-Tooltip">
    <span class="olt-u-colorPrimary">dolor</span>
    <div class="olt-Tooltip-content">
        <span>Lorem</span>
    </div>
</span>
sit amet, consectetur
<span class="olt-Tooltip olt-Tooltip--bottom">
    <span class="olt-u-colorPrimary">adipiscing</span>
    <div class="olt-Tooltip-content">
        <span>Ipsum</span>
    </div>
</span>
elit
<span class="olt-Tooltip">
    <span class="olt-u-colorSuccess">dolor</span>
    <div class="olt-Tooltip-content olt-Tooltip-content--success">
        <span>consectetur</span>
    </div>
</span>
```

