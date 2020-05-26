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
