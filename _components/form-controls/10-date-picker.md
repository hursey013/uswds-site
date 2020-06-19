---
title: Date picker
parent: Form controls
order: 10
lead: Date picker helps users select a single date.
---

{% include code/preview.html component="date-picker" %}
{% include code/accordion.html component="date-picker" %}

<div class="usa-accordion usa-accordion--bordered site-accordion-docs">
  <button class="usa-button-unstyled usa-accordion__button"
      aria-expanded="true" aria-controls="date-picker-docs">
    Guidance
  </button>
  <div id="date-picker-docs" aria-hidden="false" class="usa-accordion__content site-component-usage">
    <h4>When to use the date picker component</h4>
    <ul class="usa-content-list">
      <li><strong>Scheduling.</strong> When users are trying to schedule something in the future and would likely benefit from the context of selecting from a calendar.</li>
    </ul>
    <h4>When to consider something else</h4>
    <ul class="usa-content-list">
      <li><strong>Known date.</strong> When you’re asking users for a date they’ll already know, or can look up without using a calendar you can continue to use the <a href="{{ site.baseurl }}/form-controls/#date-input">date input fields</a>.</li>
    </ul>
    <h4>Usability guidance</h4>
    <ul class="usa-content-list">
      <li><strong>Describe date format.</strong> Provide a hint of <code>mm/dd/yyyy</code> to help the user understand the date format in cases where it is being entered manually.</li>
    </ul>
    <h4 class="usa-heading">Accessibility</h4>
    <ul class="usa-content-list">
      <li><strong>Customize accessibly.</strong> If you customize the date picker, ensure it continues to meet the the <a href="{{ site.baseurl }}/form-controls/"> accessibility requirements that apply to all form controls.</a></li>
      <li><strong>Avoid auto-submission.</strong> Don’t use JavaScript to automatically submit the form (or do anything else) when an option is selected. Auto-submission disrupts screen readers because they select each option as they read them.</li>
    </ul>
      <h4 class="usa-heading">Implementation</h4>
<div class="usa-prose site-prose" markdown="1">

{:.usa-content-list}

- **Initialization properties.**  There are properties available that will update the component during initialization. These properties must be set before the component is initialized in order to have an affect.

| property | element | effect |
| --- | --- | --- 
required | input | The combo box component will be required in terms of native form validation.
disabled | input | The combo box component will be disabled / readonly. You can re-enable by executing the `enable` procedure on the component.

{:.usa-content-list}

- **Component properties.**  There are properties available that will alter the component functionality when updated. These properties must be set before the component is initialized in order to have an affect.

| property | element | effect |
| --- | --- | --- 
data-min-date | .usa-date-picker | The date picker will not allow a date selection before this date. Typing in an earlier date will cause native form validation error. A default min date or 1/1/0000 is used as a default.
data-max-date | .usa-date-picker | The date picker will not allow a date selection after this date. Typing in an later date will cause native form validation error. There is no default maximum date.
data-range-date | .usa-date-picker | The date picker will show a range selection from the range date.

{:.usa-content-list}

- **Additional component procedures.**  There are static procedures available that can update the component after initialization. These procedures are in addition to the primary methods referenced in the  <a href="{{ site.baseurl }}/documentation/developers/#js-customization">JS customization</a>

| procedure | parameters | effect |
| --- | --- | ---
enable | .usa-date-picker element | The combo box component will be enabled.
disable | .usa-date-picker element | The combo box component will be disabled / readonly.

</div>
    <h4 class="usa-heading">Package information</h4>
    <ul class="usa-content-list">
      <li>
        <strong>Package usage:</strong> <code>@import form-controls</code>
      </li>
      <li>
        <strong>Requires:</strong> <code>required</code>, <code>global</code>
      </li>
    </ul>
  </div>
</div>