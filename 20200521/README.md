# Updates for 2020-05-06

### Contact Us Page

Text input box text-color needs to be set to `#FFFFFF` or `#F8F9FA`. Currently, text is virtually unreadable.

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

You can find that image [here](https://github.com/luuply/changes/raw/master/20200521/default_profile-01.png).

#### Radios are missing linked labels

Please double-check the `for` attribute on all of the `label` elements under the gender and status and whether any JavaScript is interfering with the proper `for` attribute passing. Currently, users must click on the radio itself, rather than being able to click on the radio's label.

### School review page

On a school's reviews page, replies that came from the original author on a review should show up as "Author" rather than "Anonymous." If a user is logged in and they are viewing their review, rather than showing "Anonymous," it should "Your Review" in `#74DC96`.

#### Modal to log in

If a user is not logged in and they click on a button that requires authentication (say, "Save"), change the text to "Please login first" instead of "Please login first to upvote or downvote."

### Review submission page

On any page to submit a review, instead of `(*)` for required blanks, use `*` only. Put the asterisk before the label (i.e. `* Choose Sport`)

Capitalize `Click here.` under the review box:

> Not sure where to start? Click here.

Instead of "Not sure where to start? click here.

### (BUG) Page should not open in a new tab

Retrace:

1. Go to Bellarmine University
2. Click Write a Review
3. See issue

The review authorship page should not open in a new tab.

### Software Manual
