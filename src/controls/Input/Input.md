---
name: Input
category: Controls
---

## Description

An *Input* component is always text input field. It occupies the `olt-Input*`
class names and can be used with any `type=` 
[HTML attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input)
that render a box for entering text.

Most common types are :

- `type=text` for text input fields
- `type=password` for password input fields
- `type=email` for email input fields

```input.html
<input type="text" class="olt-Input" placeholder="Username"/>
```

## Modifiers

### Render as block element

By default the *Input* will not change the `display` property of the `input`
tag, which will render the inputs `inline`. There is a `--block` modifier that
can be used if you want to render several inputs one below the other, without
introducing additional markup.

```block.html
<input type="text" class="olt-Input olt-Input--block" placeholder="Username"/>
<input type="email" class="olt-Input olt-Input--block" placeholder="E-mail"/>
<input type="password" class="olt-Input olt-Input--block" placeholder="Password"/>
```

## States

### Disabled state

Any input can be disabled via `disabled` HTML attribute.

```disabled.html
<input type="email" class="olt-Input" disabled placeholder="Disabled input" />
```

### Error state

The input can have an error state with `is-error` state class name.

```error.html
<input type="email" class="olt-Input is-error" value="invalid-mail@" />
```
