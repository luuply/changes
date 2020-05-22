# Updates for 2020-05-06

### Contact Us Page

Text input box text-color needs to be set to `#FFFFFF` or `#F8f9fa`. Currently, text is virtually unreadable.

### Footer

In the footers for all pages, replace the **Sample Page** with the **About Us** page.

Replace the Facebook icon with the Instagram icon (`fa-instagram`). Replace the LinkedIn icon with 

### Terms and Conditions Page

Replace:

```
<a href="https://vulpix.luuply.com/do/edit/StandardsPractices/PhotoDNA?topicparent=StandardsPractices.TOCEULA;nowysiwyg=0">PhotoDNA</a>
```

with:

```
PhotoDNA
```

There is a hotlink there that's not supposed to be there.

Replace all `â€™` with `'` (single quotes). There was an encoding issue when these files were originally sent to you.

### User Profile Page

#### Default Profile Picture

Currently, the default profile picture cannot be found (so alt-text is being displayed instead). Please use this image for the default profile picture:

![default profile picture](https://github.com/luuply/changes/raw/master/20200521/default_profile-01.png "Default Profile Picture")

You can find that image at [here](https://github.com/luuply/changes/raw/master/20200521/default_profile-01.png).

#### Radios are missing linked labels

Please double-check the `for` attribute on all of the `label` elements under the gender and status and whether any JavaScript is interfering with the proper `for` attribute passing. Currently, users must click on the radio itself, rather than being able to click on the radio's label.

### Review submission page

On any page to submit a review, instead of `(*)` for required blanks, use `*` only.

Capitalize `Click here.` under the review box:

> Not sure where to start? Click here.

Instead of "Not sure where to start? click here.

### Software Manual
