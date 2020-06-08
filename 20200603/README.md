# INTERNAL CHANGES LIST

***

## `<span>` Labels

### Attributes

###### ID: 1
###### Document: `./review-submission/` CSS
###### Severity: Moderate
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Change the helper text on `<fieldset class="comments-rating">`'s `<span>` to "Awful," "Bad," "Okay," "Good," and "Great." Root object ID is `<form id="review_form">`.

***

## Remove `<radio>` padding

### Attributes

###### ID: 2
###### Document: `./luuply-registration/` CSS
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

To cause issue, visit document, then select the radio for `<input type="radio" id="parent">`. Remove excessive padding on the nested `<div>` components for the radios. Padding on the radios and their labels should match that if you select that you're a current or former collegiate athlete. To fix, in the `style.css` document, change attribute `margin-bottom: ;` in CSS class `.luuply-page-registration #frame3 .parent-options .radio` to -10px.

***

## Add extra icon padding

### Attributes

###### ID: 3
###### Document: `./sport/mens-lacrosse/` CSS
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Add 3px additional `margin-top` and 3px additional `margin-left` to all `<span>` items under class `rate-val` to add additional icon padding.

***

## Note width

### Attributes

###### ID: 4
###### Document: `./school/?schoolname/?sport_name=?sport` CSS reference
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Add the `optionalnote` class to `<textarea name="receiver_note">` and set the CSS `width: 100%;` rather than specifying a maximum width. The `textarea` breaks when the page width is too narrow. Do not affect anything in the modal header, especially the `share_url` item.

***

## Share on twitter

### Attributes

###### ID: 5
###### Document: `./school/?schoolname/?sport_name=?sport` HTML reference
###### Severity: Low
###### Techs: CN
###### Category: Typographical error
###### Round: 1

#### Type: CI Hot

### Issue Description

Change asset `<a class="js-twitter-share">` to capitalize "Twitter". Do not affect the `<i>` asset.

***

## Footer Changes

### Attributes

###### ID: 6
###### Document: `.`
###### Severity: Moderate
###### Techs: CN
###### Category: Typographical error
###### Round: 1

#### Type: CI Hot

### Issue Description

In `<footer class="c-footer">`, change `<h5>` "Product" and "Product" to "About" and "Policies", respectively.

***

## Logout interstitial

### Attributes

###### ID: 7
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

***

## Open Sans Library

### Attributes

###### ID: 8
###### Document: `.`
###### Severity: Critical
###### Techs: CN
###### Category: BUG
###### Round: 1

#### Type: CI Hot

### Issue Description

In the CSS `.product-footer-sec h5 {}`, change `font-family` to include a backup family (sans-serif). Include the font class from Google Fonts in the `head`.

***

## Luuply is a platform for

### Attributes

###### ID: 9
###### Document: `.`
###### Severity: Low
###### Techs: CN
###### Category: Typographical error
###### Round: 1

#### Type: CI Hot

### Issue Description

In the `<p>` for `c-aboutus__repeat-single`, capitalize the first and second "To" under "Luuply is a platform for:".

***

## Inconsistent Style On Profile Page

### Attributes

###### ID: 10
###### Document: `./profile`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Under Your Reviews `<div>`, change the whole class to include `padding-b-30` so that the bottom `<hr>` appears the same distance from the text as "Saved Schools" and "Notifications". Change `border-0` to `margin-b-40`.

***

## Padding in search bar

### Attributes

###### ID: 11
###### Document: `./profile`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: Cold

### Issue Description

Vertically align the "Choose a sport" and "Search for a school..." placeholder texts in the search bar within their `<div>`. The baseline is too low.

***

## Capitalize error

### Attributes

###### ID: 12
###### Document: `./profile`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Capitalize "profile" in Change Profile Picture when updating the profile.

***

## Placeholder text in profile change

### Attributes

###### ID: 13
###### Document: `./profile`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Show some placeholder text under "Saved Schools" if the user doesn't have anything saved.

***

## Search results `<h1>`

###### ID: 14
###### Document: `./school/?schoolname/?sport_name=?sport` JS reference
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: Cold

### Issue Description

When searching, if you don't select anything for school, then a comma shows up without anything to preface it. If only one search query provided, remove the comma. Style "mens-lacrosse" to "Men's Lacrosse".

***

## Remove `border-bottom` and shrink the padding

###### ID: 15
###### Document: `./review-submission/`
###### Severity: Moderate
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

In the `form.review-form.comments-rating {}` CSS class, remove the `border-bottom` and change `margin-bottom` to 15px. Remove the `padding-bottom` attribute.

***

## Coaches page

###### ID: 16
###### Document: a school page
###### Severity: Low
###### Techs: Internal
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Replace HC and AC with "Head Coach" and "Assistant Coach".

***

## School detail style

###### ID: 17
###### Document: a school page
###### Severity: Low
###### Techs: Internal
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Remove the dash `-` before the tallies.

***

## Contact style

###### ID: 18
###### Document: `./contact-us/`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Remove the `<h6>` at the top of the page altogether. Do not affect the `<h1>` asset.

After submission, remove the `wpcf7-mail-sent-ok` border `2px solid green`. Change the text to something more suitable.

***

## Margins on headers

###### ID: 19
###### Document: `./contact-us/`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Change the spacing `margin-bottom` from 40px to 10px on `article.contact-us h1 {}` for the `<h1>` asset.

***

## Capitalize facebook

###### ID: 20
###### Document: `./review-submission/`
###### Severity: High
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: Cold

### Issue Description

When clicking to post review when not signed in, change the text in the modal that pops up for `id=fbLink"` to capitalize "Facebook."

***

## Center continue button

###### ID: 21
###### Document: `./review-submission/`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: Cold

### Issue Description

Center button with `name="next"` after clicking to post review when not signed in.

***

## Center and reformat login button if not signed in

###### ID: 22
###### Document: `./review-submission/`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: Cold

### Issue Description

When not signed in, merge the Already in Luuply `<p>` and the login button into one `<a>` and center.

***

## Remove Lorem ipsum text

###### ID: 23
###### Document: `./review-submission/`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

Remove the Lorem ipsum text when signing up through the review submission page.

***

## Login Labels

###### ID: 24
###### Document: `./luuply-login/`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

In the form with `id="loginform"`, in the `<label for="user_login">` and `<label for="user_pass">`, add the CSS style attribute `visibility: hidden;` to hide the labels.

***

## Login Fields

###### ID: 25
###### Document: `./luuply-login/`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

In the form with `id="loginform"`, in the HTML for `<input name="log">` and `<input name="pwd">`, add the HTML attribute `placeholder="Email Address"` and `placeholder="Password"`, respectively.

***

## Verified user style change

###### ID: 26
###### Document: `./luuply-registration/`
###### Severity: Low
###### Techs: CN
###### Category: Style
###### Round: 1

#### Type: CI Hot

### Issue Description

If a user selects that they are a current or former collegiate athlete, change the wording of the subsequent question to "Do you want to be a verified user?" Add an `<a>` for "verified user" that opens a modal. Add the following HTML to that page to create that modal.

```
<div class="modal-content">
  <div class="modal-header">
    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
      <span aria-hidden="true">×</span>
    </button>
  </div>
  <div class="modal-body">
    <h1>What is a verified user?</h1>
    <p>A verified badge shows up as a blue checkmark next to your reviews and on your profile. It means that Luuply has verified that you are who you say that you are, and provides additional assurance to readers that your review can be trusted as authentic and representative.</p>
    <ul>
      <li>Verified accounts don't get extra features on Luuply. They aren't indicative of endorsement by Luuply, and they don't represent awards or milestones.</li>
      <li>We reserve the right to revoke verification or terminate accounts that violate our Code of Conduct or Terms of Service.
    </ul>
  </div>
</div>
```

***

## jQuery version change

###### ID: 27
###### Document: `.`
###### Severity: High
###### Techs: CN
###### Category: Dependency
###### Round: 1

#### Type: Cold

### Issue Description

Upgrade jQuery version from 2.12.4 to 3.5 or later.

***

***

## Theme color in head

###### ID: 28
###### Document: `.`
###### Severity: Low
###### Techs: CN
###### Category: Frontend
###### Round: 1

#### Type: Cold

### Issue Description

In the `<head>`, add the following line:

```
<meta name="theme-color" content="#3c3c3c">
```

***

***

# Images

We encourage you to view these images to aid in your fixes.

![](https://github.com/luuply/changes/raw/master/20200603/new_.footers.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_contact-us.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_luuply-login.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_luuply-registration.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_luuply-registration_verify.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_profile-EDIT.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_profile.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_review-submission-signup-modal.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_review-submission.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_schoolpage.PNG)
![](https://github.com/luuply/changes/raw/master/20200603/new_test_results.PNG)
