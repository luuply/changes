# Changes for 2020-05-24

### Program Ranking Style

Using Bootstrap columns, make the :star: ratings aligned so that they're in their own column, as opposed to depending on the length of the school name. In the image below, the star rankings *should* be in their own column.

![Unaligned stars](https://github.com/luuply/changes/raw/master/20200524/Image%20from%20iOS.png "Unaligned stars")

### Sticky navbar

On mobile, the page navigation for the reviews page is currently only at the top. Use a very skinny navbar at the top and make it sticky, so that users can navigate away from the page without having to scroll all the way to the top.

### Centering Asset on Homepage

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

### Mobile Responsiveness Issue

On mobile, "Choose a sport" isn't visible in any page when it's in the header because of text overflow. The homepage is fine, but everywhere else is not. See:

![Text overflowed from sport select](https://github.com/luuply/changes/raw/master/20200524/Image%20from%20iOS%20(1).png "Text overflowed from sport select")
![Text fine on homepage for sport select](https://github.com/luuply/changes/raw/master/20200524/Image%20from%20iOS%20(2).png "Text fine on homepage for sport select")

### Add Mailing List Embedded Script

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

### Gussy Up the Contact Us Page

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
