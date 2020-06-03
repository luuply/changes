# INTERNAL CHANGES LIST

## `<span>` Labels

### Attributes

###### ID: 1
###### Document: `./review-submission/index.php` CSS
###### Severity: Moderate
###### Techs: Internal fix
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Change the helper text on `<fieldset class="comments-rating">`'s `<span>` to "Awful," "Bad," "Okay," "Good," and "Great." Root object ID is `<form id="review_form">`.

## Remove `<radio>` padding

### Attributes

###### ID: 2
###### Document: `./luuply-registration/index.php` CSS
###### Severity: Low
###### Techs: Internal fix
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

To cause issue, visit document, then select the radio for `<input type="radio" id="parent">`. Remove excessive padding on the nested `<div>` components for the radios. To fix, in the `style.css` document, change attribute `margin-bottom: ;` in CSS class `.luuply-page-registration #frame3 .parent-options .radio` to -10px.

## Add extra icon padding

### Attributes

###### ID: 3
###### Document: `./sport/mens-lacrosse/index.php` CSS
###### Severity: Low
###### Techs: Internal fix
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Add 3px additional `margin-top` and 3px additional `margin-left` to all `<span>` items under class `rate-val` to add additional icon padding.

## Note width

### Attributes

###### ID: 4
###### Document: `./school/?schoolname/?sport_name=?sport` CSS reference
###### Severity: Low
###### Techs: Internal fix
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Add the `optionalnote` class to `<textarea name="receiver_note">` and set the CSS `width: 100%;`. Do not affect anything in the modal header, especially the `share_url` item.
