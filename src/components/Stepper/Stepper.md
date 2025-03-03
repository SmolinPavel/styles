---
name: Stepper
category: Component
---

## Description

*Stepper* is used to render a wizard-friendly steps row. Each step is a
`<input type="radio">` under the hood, so it can work without JavaScript. The 
*Stepper* occupies `olt-Stepper*` class names and can contain :

- `olt-Stepper-header` - The "step" button
- `olt-Stepper-content` - The content of the step.

The step's content is only visible when the user has clicked on the step itself.

The *Stepper* is transformed to row toggled sections, when a small screen is
being used to render it. You can test the functionality by reducing the screen 
width of this page and take a look at the example below.


```stepper.css hidden
body > div.olt-Frame { min-height: 250px; }
```

```stepper.html
<div class="olt-Stepper">
  <input type="radio" name="steps" id="step-one" checked="checked"/>
  <label for="step-one" class="olt-Stepper-header">Step One</label>
  <div class="olt-Stepper-content">
    <h4 class="olt-Headline olt-Headline--4">Step One Content</h4>
    <p class="olt-Paragraph">Lorem ipsum dolor sit amet, consectetur adipisicinsg elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
  </div>

  <input type="radio" name="steps" id="step-two"/>
  <label for="step-two" class="olt-Stepper-header">Step Two</label>
  <div class="olt-Stepper-content">
    <h4 class="olt-Headline olt-Headline--4">Step Two Content</h4>
    <p class="olt-Paragraph">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
  </div>

  <input type="radio" name="steps" id="step-three"/>
  <label for="step-three" class="olt-Stepper-header">Step Three</label>
  <div class="olt-Stepper-content">
    <h4 class="olt-Headline olt-Headline--4">Step Three Content</h4>
    <p class="olt-Paragraph">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
  </div>

	<input type="radio" name="steps" id="step-four"/>
  <label for="step-four" class="olt-Stepper-header">Step Four</label>
  <div class="olt-Stepper-content">
    <h4 class="olt-Headline olt-Headline--4">Step Four Content</h4>
    <p class="olt-Paragraph">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
  </div>
</div>
```

## Stepper as Navigation

There is also another *Stepper* usecase, when one can use it as a simple
navigation and control the active step via `is-active` state class name.

```navigation.html
<div class="olt-Stepper olt-Stepper--navigation">
  <a class="olt-Stepper-header is-active">Link One</a>
  <a class="olt-Stepper-header">Link Two</a>
  <a class="olt-Stepper-header">Link Three</a>
</div>
```
