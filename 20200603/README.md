# INTERNAL CHANGES LIST

## `<span>` Labels

### Attributes

###### ID: 1
###### Document: `./review-submission/index.php`
###### Severity: Moderate
###### Techs: Internal fix
###### Category: Style
###### Round: 1

### Issue Description

Change the helper text on `<fieldset class="comments-rating">`'s `<span>` to "Awful," "Bad," "Okay," "Good," and "Great." Root object ID is `<form id="review_form">`.

## Remove `<radio>` padding

### Attributes

###### ID: 2
###### Document: `./luuply-registration/index.php`
###### Severity: Low
###### Techs: Internal fix
###### Category: Style
###### Round: 1

### Issue Description

To cause issue, visit document, then select the radio for `<input type="radio" id="parent">`. Remove excessive padding on the nested `<div>` components for the radios. To fix, in the `style.css` document, change attribute `margin-bottom: ;` in CSS class `.luuply-page-registration #frame3 .parent-options .radio` to -10px.
