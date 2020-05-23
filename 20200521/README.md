# Updates for 2020-05-06

### Verified Users Clarification

I think that we've been having some communication issues in determining exactly what a verified user is, compared to email verification. The two terms are not the same, and there's some confusion surrounding exactly what verification is and why it's important.
Email validation occurs for *ALL* users. It's just there to make sure that bots and illegitimate users aren't signing up and filling our databases with tons of fake accounts.
Account verification occurs for *SELECT* users: only users who have **both** identified as a current or former collegiate athlete AND have opted into account verification. It's there to make sure that athletes who say that they go to a certain school actually do go to that school and that they actually play in the athletics program there. Its purpose is to prevent an athlete from trash-talking or leaving bad reviews on schools that they just don't like, but aren't qualified to review (since they never attended that school).
I've linked a short video [here](https://drive.google.com/file/d/1uB_0Q3f0P9znUB1Jvx3rqfLB3EIjiShC/view?usp=sharing
) that explains exactly what I'm talking about.

### (Fixed) Contact Us Page

Text input box text-color needs to be set to `#F8F9FA`. Currently, text is virtually unreadable.

### (Fixed) Footer

In the footers for all pages, replace the **Sample Page** with the **About Us** page.

Replace the Facebook icon with the Instagram icon (`fa-instagram`). Replace the LinkedIn icon with 

### (Fixed) Terms and Conditions Page

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

### (Fixed) User Profile Page

#### Default Profile Picture

Currently, the default profile picture cannot be found (so alt-text is being displayed instead). Please use this image for the default profile picture:

![default profile picture](https://github.com/luuply/changes/raw/master/20200521/default_profile-01.png "Default Profile Picture")

You can find that image [here](https://github.com/luuply/changes/raw/master/20200521/default_profile-01.png).

The blue checkmark icon is currently set as the default profile picture for "About Yourself" in WordPress Admin, causing any and all users to be marked as verified.

#### (Fixed) Radios are missing linked labels

Please double-check the `for` attribute on all of the `label` elements under the gender and status and whether any JavaScript is interfering with the proper `for` attribute passing. Currently, users must click on the radio itself, rather than being able to click on the radio's label.

### (ALMOST Fixed) School review page

On a school's reviews page, replies that came from the original author on a review should show up as "Author" rather than "Anonymous." If a user is logged in and they are viewing their review, rather than showing "Anonymous," **it should show "Your Review" in `#74DC96`**.

#### (Fixed) Modal to log in

If a user is not logged in and they click on a button that requires authentication (say, "Save"), change the text to "Please login first" instead of "Please login first to upvote or downvote."

### (Fixed) Review submission page

On any page to submit a review, instead of `(*)` for required blanks, use `*` only. Put the asterisk before the label (i.e. `* Choose Sport`)

Capitalize `Click here.` under the review box:

> Not sure where to start? Click here.

Instead of "Not sure where to start? click here.

### (Fixed BUG) Page should not open in a new tab

Retrace:

1. Go to Bellarmine University
2. Click Write a Review
3. See issue

The review authorship page should not open in a new tab.

### School saving

On a school's page, save the _program_, not the _school_. For example, if I save the men's lacrosse page, I want to only save men's lacrosse program, not the school's entire athletic program. You should also be able to remove a saved program as well.

#### (BUG) Hyperlinks are broken

When a school is saved, the link that should be added to the user's profile has no hyperlink back to the school's review page (like the links for notifications and your reviews).

### Hiding Reviews

There is currently no way to hide the replies to a review or a comment after opening them, so once you open the replies, you have to refresh the page to hide those replies again.

![Hide replies not available](https://github.com/luuply/changes/raw/master/20200521/Image%20from%20iOS%20(1).png "Hide replies not available")

### (Fixed BUG) View Replies not showing up on mobile

The "View Replies" button is not showing up on mobile devices for reviews that have replies.

![View 2 replies not showing up](https://github.com/luuply/changes/raw/master/20200521/Image%20from%20iOS.png "View 2 replies not showing up")

### Software Manual

We'd like to remind you that we still need a software manual. At the least, it needs to include:

- Installation instructions
- How to add or remove schools
- How to update the logos or information for existing schools
- How to add or remove sports
- How to manually remove reviews and comments that don't meet our community guidelines
- How to manually add or remove accounts
- Basic troubleshooting
