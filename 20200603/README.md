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

## Share on twitter

### Attributes

###### ID: 5
###### Document: `./school/?schoolname/?sport_name=?sport` HTML reference
###### Severity: Low
###### Techs: Internal fix
###### Category: Typographical error
###### Round: 1

#### Type: CI Hot

### Issue Description

Change asset `<a class="js-twitter-share">` to capitalize "Twitter". Do not affect the `<i>` asset.

## Footer Changes

### Attributes

###### ID: 6
###### Document: `.`
###### Severity: Moderate
###### Techs: Internal fix
###### Category: Typographical error
###### Round: 1

#### Type: CI Hot

### Issue Description

In `<footer class="c-footer">`, change `<h5>` "Product" and "Product" to "About" and "Policies", respectively.

## Logout interstitial

### Attributes

###### ID: 6
###### Document: `./wp-login.php`, origin `./profile/` and `.`
###### Severity: Moderate
###### Techs: CN
###### Category: BUG
###### Round: 1

#### Type: Cold

### Issue Description

From either of the origin documents, clicking "Logout" still presents an interstitial page.

### Hotfix

Style the `./wp-login.php` document as other code is being modified prior to removal.

