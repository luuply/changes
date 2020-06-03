# Changes for 2020-05-24

### (FIXED) Program Ranking Style

Using Bootstrap columns, make the :star: ratings aligned so that they're in their own column, as opposed to depending on the length of the school name. In the image below, the star rankings *should* be in their own column.

![Unaligned stars](https://github.com/luuply/changes/raw/master/20200524/Image%20from%20iOS.png "Unaligned stars")

### (FIXED) Sticky navbar

On mobile, the page navigation for the reviews page is currently only at the top. Use a very skinny navbar at the top and make it sticky, so that users can navigate away from the page without having to scroll all the way to the top.

### (FIXED) Centering Asset on Homepage

For the titles for Men's and Women's lacrosse under Program Ranking, change these to `text-align: center;` as shown here:

```
<div class="box-section__single" style="
    text-align: center;
"><h4>Men’s Lacrosse</h4><ol><li><a href="http://dev106.developer24x7.com/cnp910/school/brown-university/?sport_name=mens-lacrosse">Brown University</a><p class="home-rate"><span class="ratings dashicons dashicons-star-filled"></span><span class="rate-val">5</span></p></li><li><a href="http://dev106.developer24x7.com/cnp910/school/stanford-university/?sport_name=mens-lacrosse">Stanford University Demo</a><p class="home-rate"><span class="ratings dashicons dashicons-star-filled"></span><span class="rate-val">4.2</span></p></li></ol><a class="" href="http://dev106.developer24x7.com/cnp910/luuply-login/">See full list</a></div>
```

```
<div class="box-section__single" style="
    text-align: center;
"><h4>Women’s Lacrosse</h4><ol><li><a href="http://dev106.developer24x7.com/cnp910/school/stanford-university/?sport_name=womens-lacrosse">Stanford University Demo</a><p class="home-rate"><span class="ratings dashicons dashicons-star-filled"></span><span class="rate-val">4.6</span></p></li></ol><a class="" href="http://dev106.developer24x7.com/cnp910/luuply-login/">See full list</a></div>
```

Update: this has been resolved on mobile only, not on desktop. Please double-check this!

### (FIXED) Mobile Responsiveness Issue

On mobile, "Choose a sport" isn't visible in any page when it's in the header because of text overflow. The homepage is fine, but everywhere else is not. See:

![Text overflowed from sport select](https://github.com/luuply/changes/raw/master/20200524/Image%20from%20iOS%20(1).png "Text overflowed from sport select")
![Text fine on homepage for sport select](https://github.com/luuply/changes/raw/master/20200524/Image%20from%20iOS%20(2).png "Text fine on homepage for sport select")

### (FIXED) Add Mailing List Embedded Script

Add and style this script according to the style of the rest of the site. Do not change the ID or any attributes other than style of the elements.

```
<!-- Begin Mailchimp Signup Form -->
<div id="mc_embed_signup">
<form action="https://luuply.us18.list-manage.com/subscribe/post?u=6269eb225a8672a1ef294cf05&amp;id=ca201131ed" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
    <div id="mc_embed_signup_scroll">
	<h2>Subscribe to Luuply's Newsletter</h2>
<div class="indicates-required"><span class="asterisk">*</span> indicates required</div>
<div class="mc-field-group">
	<label for="mce-EMAIL">Email Address  <span class="asterisk">*</span>
</label>
	<input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL">
</div>
<div class="mc-field-group">
	<label for="mce-FNAME">First Name </label>
	<input type="text" value="" name="FNAME" class="" id="mce-FNAME">
</div>
<div class="mc-field-group">
	<label for="mce-LNAME">Last Name </label>
	<input type="text" value="" name="LNAME" class="" id="mce-LNAME">
</div>
<div class="mc-field-group size1of2">
	<label for="mce-PHONE">Phone Number </label>
	<input type="text" name="PHONE" class="" value="" id="mce-PHONE">
</div>
	<div id="mce-responses" class="clear">
		<div class="response" id="mce-error-response" style="display:none"></div>
		<div class="response" id="mce-success-response" style="display:none"></div>
	</div>    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
    <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_6269eb225a8672a1ef294cf05_ca201131ed" tabindex="-1" value=""></div>
    <div class="clear"><input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button"></div>
    </div>
</form>
</div>

<!--End mc_embed_signup-->
```

### (FIXED) Gussy Up the Contact Us Page

The **Contact Us** page is pretty boring right now. Keep the functionality, but change the HTML to roughly match:

```
<main id="main" class="site-main">
			<div class="container">
		
<article id="post-25" class="common-page post-25 page type-page status-publish hentry">
	<header class="entry-header text-center">
    <h6 style="color: #74dc96;">Got a question?</h6>
		<h1 style="color: #F8F9FA">Contact Luuply</h1>	</header><!-- .entry-header -->
    <div class="container">
        <div class="row">
            <div class="column text-center">
                <p>We're here to help you and answer any questions that you might have.<br>We look forwards to hearing from you!</p>
            </div>
        </div>
    </div>

	
	<div class="entry-content">
		
<div role="form" class="wpcf7" id="wpcf7-f527-p25-o1" lang="en-US" dir="ltr">
<div class="screen-reader-response" role="alert">One or more fields have an error. Please check and try again.<ul><li>The field is required.</li><li>The field is required.</li></ul></div>
<form action="/cnp910/contact-us/#wpcf7-f527-p25-o1" method="post" class="wpcf7-form invalid text-center" novalidate="novalidate" style="background-color: #3e3e3e; border-radius: 10px; padding: 20px;">
<div style="display: none;">
<input type="hidden" name="_wpcf7" value="527">
<input type="hidden" name="_wpcf7_version" value="5.1.7">
<input type="hidden" name="_wpcf7_locale" value="en_US">
<input type="hidden" name="_wpcf7_unit_tag" value="wpcf7-f527-p25-o1">
<input type="hidden" name="_wpcf7_container_post" value="25">
</div>
<p><label> Your Name (required)<br>
    <span class="wpcf7-form-control-wrap your-name"><input type="text" name="your-name" value="" size="40" class="wpcf7-form-control wpcf7-text wpcf7-validates-as-required wpcf7-not-valid" aria-required="true" aria-invalid="true" placeholder="Jane Doe"><span role="alert" class="wpcf7-not-valid-tip">The field is required.</span></span> </label></p>
<p><label> Your Email (required)<br>
    <span class="wpcf7-form-control-wrap your-email"><input type="email" name="your-email" value="" size="40" class="wpcf7-form-control wpcf7-text wpcf7-email wpcf7-validates-as-required wpcf7-validates-as-email wpcf7-not-valid" aria-required="true" aria-invalid="true" placeholder="jane.doe@example.com"><span role="alert" class="wpcf7-not-valid-tip">The field is required.</span></span> </label></p>
<p><label> Subject<br>
    <span class="wpcf7-form-control-wrap your-subject"><input type="text" name="your-subject" value="" size="40" class="wpcf7-form-control wpcf7-text" aria-invalid="false" placeholder="Example: Star Wars Ep. II was the best one."></span> </label></p>
<p><label>Message<br>
    <span class="wpcf7-form-control-wrap your-message"><textarea name="your-message" cols="40" rows="10" class="wpcf7-form-control wpcf7-textarea" aria-invalid="false" placeholder="Ask us a question, drop us a message, or just say hi!"></textarea></span> </label></p>
<p><input type="submit" value="Send" class="wpcf7-form-control wpcf7-submit btn"><span class="ajax-loader"></span></p>
<div class="wpcf7-response-output wpcf7-display-none wpcf7-validation-errors" style="display: block;" role="alert">Please double-check everything above! It looks like we've got a problem!</div></form></div>
	</div><!-- .entry-content -->

	</article><!-- #post-25 -->
			</div>
		</main>
```

In the header's `<h1>` element, remove the `margin-bottom: 40px;` and replace it with `margin-bottom:10px;`. In the header's `<h6>` element, change the `margin-top` to `margin-top: 40px;`. Leave the `margin-bottom: 10px;`.

In the `textarea` with name `your-message`, change the CSS so that `padding-top: 10px;`.

The page should *roughly* look like the following. Please read over the code changes to make sure that they're all compatible, FIRST!

![Contact Us Mockup](https://github.com/luuply/changes/raw/master/20200524/Capture.PNG "Contact Us Mockup")

### (FIXED) Roster Break Down Formatting

Please add an extra space after "TOTAL:" on the school's roster breakdown page.

### (FIXED) Pages With Missing Information

If a page is missing some information, [like this one](http://dev106.developer24x7.com/cnp910/school/arizona-state-university/?sport_name=womens-lacrosse#ChildVerticalTab_12), add a message so that the page isn't blank. Here's some basic HTML to get you started.

```
<p>We're missing some information about this school.</p>
<p>If you know what this missing information should be, you can let us know by <a href="http://dev106.developer24x7.com/cnp910/contact-us/">contacting us</a>.</p>
```

### Login Page Padding

On the Login page, add some padding (between 5px and 10px) to either the checkbox or the label for the checkbox for "Remember Me." 

Add some padding to the "Create an account" link (between 5px and 10px).

The "Lost your password?" and "Create an account" links should darken onhover to indicate that they are being hovered over and that they are active links.

### Login Page SSO Button

On the Login page, for the Facebook SSO button, capitalize **Facebook**. That is, the full element should read:

```
<a class="fb-icon" href="https://www.facebook.com/v2.10/dialog/oauth?client_id=585009812359917&amp;state=aa9dcceee19b44504f948156a6e31a97&amp;response_type=code&amp;sdk=php-sdk-5.7.0&amp;redirect_uri=http%3A%2F%2Fdev106.developer24x7.com%2Fcnp910%2Ffb-process%2F&amp;scope=email"><img src="http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/fb-icon">Sign in with Facebook</a>
```

instead of 

```
<a class="fb-icon" href="https://www.facebook.com/v2.10/dialog/oauth?client_id=585009812359917&amp;state=aa9dcceee19b44504f948156a6e31a97&amp;response_type=code&amp;sdk=php-sdk-5.7.0&amp;redirect_uri=http%3A%2F%2Fdev106.developer24x7.com%2Fcnp910%2Ffb-process%2F&amp;scope=email"><img src="http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/fb-icon">Sign in with facebook</a>
```

### (FIXED) Footers

For the footers on ALL pages, change the color of the copyright `<p>` to `#555`.

Change the social media icons to `fa-facebook`, `fa-twitter`, and `fa-instagram`.

### (FIXED) Share Modal CSS Bug

In the sharing modal, the helptext to "Please enter X or more characters" needs to be adjusted so that it does not overlap the "To email addresses" `span`. 

For the `textarea` (class: `shr-md1-main textarea`) for the "Add a note", add the following CSS:

```
padding-top: 10px;
padding-left: 15px;
```

Change the "Add a note(optional)" into a properly formed and attributed `<label>` (rather than a `<p>`), and adjust the text to "Add a note (optional)".

### (FIXED) Emails

When you share a post by email, please change the wording to:

> Subject: Someone shared a Luuply page with you
>
> User Name shared a page with you from Luuply!
>
> To view the page, go to `<link URL here>`.

If possible, style the email using some HTML.

### (FIXED) Way to Unsave

If a user has saved a particular program, they need to be able to *unsave* it using the same mechanism. For example, if I visit the page for Boston University, which I have saved, if I click on "Saved", it should remove the program's listing from my account.

### Software Manual

We'd like to remind you that we still need a software manual. At the least, it needs to include:

- Installation instructions
- How to add or remove schools
- How to update the logos or information for existing schools
- How to add or remove sports
- How to manually remove reviews and comments that don't meet our community guidelines
- How to manually add or remove accounts
- Basic troubleshooting
- Adding a site-wide alert (say, for cookie notifications, outages, notices, etc.)

### (FIXED BUG) Writing Review Without Logging In

If you write a review without being logged in, it prompts you after hitting "Post" to sign up. If you try to sign up, it hangs.

![Sign Up Hanging](https://github.com/luuply/changes/raw/master/20200524/signuphang.jpg "Sign Up Hanging")

If you click out of the modal without completing the sign up, the button you clicked changes to "posting...", even if you didn't complete the entire sign-up process.

![Posting Image](https://github.com/luuply/changes/raw/master/20200524/postingimage.jpg "Posting Image")

### (FIXED) Add "Next Page" navigation to bottom

Add the button to view the next page of reviews to the bottom of school pages with more than 5 reviews. Currently, you need to scroll all the way back up to go to the next page.

![Navigation At Bottom](https://github.com/luuply/changes/raw/master/20200524/navbottom1.png "Navigation At Bottom")
![Navigation At Bottom](https://github.com/luuply/changes/raw/master/20200524/navbottom2.png "Navigation At Bottom")

### (FIXED) Write Reviews in New Tab

If you click on "Start your review of *school name*", the page opens in the current tab. However, if you click on the star ratings to start the review, it still opens in a new tab.

![Stars](https://github.com/luuply/changes/raw/master/20200524/stars.png "Stars")

### (FIXED) Lost Password

The forgot password process isn't formatted in our colors, and it doesn't work.

![Forgot password](https://github.com/luuply/changes/raw/master/20200524/forgotpassword.png "Forgot password")

### (FIXED) Email Confirmation Style

Please style the PHPMailer script that sends emails to the users for email confirmation as such:

```
<html>
  <head>
    <title>Please confirm your email</title>
    <link href="https://fonts.googleapis.com/css2?family=Hind&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans&display=swap" rel="stylesheet">
  </head>
  <body style="background-color: #F8F9FA;">
    <div style="padding: 10px;margin: 20px;text-align: center;">
      <h1 style="font-family: 'Hind', sans-serif;color: #1FACEA;">Welcome to Luuply!</h1>
      <h2 style="font-family: 'Hind', sans-serif;color: #1FACEA;">Email confirmation</h2>
    </div>
    <div style="padding: 10px;margin: 20px;text-align: center;">
      <p style="font-family: 'Open Sans', sans-serif;color: #000000;">Thank you for registering for a Luuply account!</p>
      <p style="font-family: 'Open Sans', sans-serif;color: #000000;">You or someone else has registered on %ACCTDATE% using the address %EMAIL%.</p>
    </div>
    <div style="padding: 30px;margin: 30px;text-align: center;background-color: #b1b1b1;border-radius: 8px;">
      <p style="font-family: 'Open Sans', sans-serif;color: #000000;">To confirm your email address, please click on this button:</p>
      <button style="background-color: #1FACEA;border: none;border-radius: 8px;color: white;padding: 15px 32px;text-align: center;text-direction: none;display: inline-block;font-size: 16px;" type="button" onclick="location.href='%CONFIRMLINK%'">Confirm My Email</button>
    </div>
    <div style="padding: 10px;margin: 20px;text-align: center;">
      <p style="font-family: 'Open Sans', sans-serif;color: #000000;">If the above link does not work, copy and paste this link into your web browser: <a style="color: #1FACEA'background-color: transparent;text-decoration: none;" href="%CONFIRMLINK%">%CONFIRMLINK%</a></p>
    </div>
    <div style="padding: 10px;margin: 20px;text-align: center;">
      <p style="font-family: 'Open Sans', sans-serif;color: #C3C3C3;">If you believe that this is a mistake, you can just ignore this message and nothing else will happen.
      <br>
      If you have questions or comments, please email us at <a style="color: #1FACEA;background-color: transparent;text-decoration: none;" href="mailto:hello@luuply.com">hello@luuply.com</a>.
      </p>
    </div>
  </body>
</html>
```

Adjust all links as needed.

### (FIXED) Account activated page issue

Adjust the bottom margin and padding of the `<article>` with `id="post-109"`.

Change the heading text to just "**Your email has been confirmed!**". Change the lorem ipsum text to the following:

> Thanks for confirming your email address! We're excited that you're joining us here on Luuply. To get started, you can go [home](https://luuply.com) or just start searching for a school above. If you have questions, please don't hesitate to get in contact with us [here](./contact-us/)!

Remove the "Visit homepage" button.

### (FIXED) Logout issue

Remove the interstitial page when a user not using SSO tries to log out.

![Logout interstitial page](https://github.com/luuply/changes/raw/master/20200524/logoutinterstitial.png "Logout interstitial page")

### (FIXED) Sign up page SSO button

Similar to the login page, please capitalize "Facebook" in the SSO button on the sign up page.

### (FIXED) Erroneous password change emails

When a user signs in using SSO, they might receive a "Password Changed" email that lets them know that their password was changed, even though they had just signed in with SSO. Password change emails ***must*** only be sent if a user does NOT sign in with SSO.

### Recent reviews

Recent reviews nees to have the school and sport included, see image:

![Recent reviews](https://github.com/luuply/changes/raw/master/20200524/recentreviews.png "Recent reviews")

### See more

"Older posts" should say "see more" instead. See image:

![Older posts](https://github.com/luuply/changes/raw/master/20200524/olderposts.png "Older posts")

### Verification Email Page Link

On the confirmation page after you verify your email, the "contact us here" link is formatted with an extra period. Please remove the period at the end of the `<p>`. See image: 

![Extra period](https://github.com/luuply/changes/raw/master/20200524/extraperiod.png "Extra period")

# THANK YOU!
