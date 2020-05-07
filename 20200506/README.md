# Updates for 2020-05-06

### Buttons on Hover

On homepage, change button text color on hover to black `#000000`

```
<li class="register"><a href="http://dev106.developer24x7.com/cnp910/luuply-registration/">Sign Up</a></li>
```

Change button icon color on hover to black `#000000`

```
<i class="fa fa-search" aria-hidden="true"></i>
```

### Links on Hover

On homepage, this element:

```
<div class="menu-header-menu-container"><ul id="menu-header-menu" class="header-nav"><li id="menu-item-128" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-128"><a href="http://dev106.developer24x7.com/cnp910/review-submission/">Write a Review</a></li>
<li id="menu-item-27" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-27"><a href="http://dev106.developer24x7.com/cnp910/about-us/">About Us</a></li>
<li id="menu-item-28" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-28"><a href="http://dev106.developer24x7.com/cnp910/contact-us/">Contact Us</a></li>
</ul></div>
```

On hover, change the text to underline. For example, when I hover on WRITE A REVIEW, it should change to _WRITE A REVIEW_.

### Search Box

On homepage, this element:

```
<span class="select2-selection select2-selection--single" role="combobox" aria-haspopup="true" aria-expanded="false" tabindex="0" aria-disabled="false" aria-labelledby="select2-sports-container"><span class="select2-selection__rendered" id="select2-sports-container" role="textbox" aria-readonly="true" title="Men’s Lacrosse"><span class="select2-selection__clear" title="Remove all items" data-select2-id="120">×</span>Men’s Lacrosse</span><span class="select2-selection__arrow" role="presentation"><b role="presentation"></b></span></span>
```

While searching, auto-populate the `<span class="select2-selection__clear" title="Remove all items" data-select2-id="120">×</span>` with the filled search query, but the incomplete portion highlighted, like Google.

### Alphabetical Order

On homepage, the select menu for the school search should be in alphabetical order, DESC from A-Z.

```
<span class="select2-selection select2-selection--single" role="combobox" aria-haspopup="true" aria-expanded="true" tabindex="0" aria-disabled="false" aria-labelledby="select2-institute-container" aria-owns="select2-institute-results" aria-activedescendant="select2-institute-result-fd9r-Yale University"><span class="select2-selection__rendered" id="select2-institute-container" role="textbox" aria-readonly="true"><span class="select2-selection__placeholder">Search for a school...</span></span><span class="select2-selection__arrow" role="presentation"><b role="presentation"></b></span></span>
```

### Search Broken [BUG]

On homepage, the select menu is broken when searching. When you type in a letter, say G, the correct school might show up, but it also displays a bunch of schools that don't have the letter "G."

![Dropdown Bug Image](https://github.com/luuply/changes/raw/master/20200506/dropdownbug.PNG "Dropdown Bug Image")

### Add the ratings to the program ranking

On homepage, under program ranking, show the ranking, school name, and the rating, not just the ranking and school name.

```
<div class="box-section__single"><h4>Men’s Lacrosse</h4><ol><li><a href="http://dev106.developer24x7.com/cnp910/school/stanford-university/?sport_name=mens-lacrosse">Stanford University Demo</a></li></ol><a class="" href="http://dev106.developer24x7.com/cnp910/luuply-login/">Login to see full list</a></div>
<div class="box-section__single"><h4>Women’s Lacrosse</h4><ol><li><a href="http://dev106.developer24x7.com/cnp910/school/stanford-university/?sport_name=womens-lacrosse">Stanford University Demo</a></li></ol><a class="" href="http://dev106.developer24x7.com/cnp910/luuply-login/">Login to see full list</a></div>
```

### Change button label

On homepage, under program ranking, change `<a class="" href="http://dev106.developer24x7.com/cnp910/luuply-login/">Login to see full list</a>` to `<a class="" href="http://dev106.developer24x7.com/cnp910/luuply-login/">See full list</a>` for both men's and women's lacrosse.

### Button style

In these elements:

```
<a href="http://dev106.developer24x7.com/cnp910/about-us/" class="btn btn-normal btn-normal--arrow">About Us</a>
```

AND

```
<a href="#" class="btn btn-normal btn-normal--arrow">Register Now</a>
```

Change the text style to bold and the text color to black `#000000`.

### Register Now Button Broken [BUG]

In the register now button at the bottom of the page:

```
<a href="#" class="btn btn-normal btn-normal--arrow">Register Now</a>
```

The href still hasn't been assigned a non-default value. Please fix.

### Feature request

If the user is logged in, then don't display this Bootstrap container:

```
<div class="container">
		            <h1>How does Luuply work?</h1>
		            <div class="c-howdoes__steps">
		                <div class="row">

		                										          <div class="col-md-4">
							                      	<div class="c-howdoes__steps-single" style="background-image: url(http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/black-box.png);">
							                            <div class="c-howdoes-top">
							                                <img src="http://dev106.developer24x7.com/cnp910/wp-content/uploads/2020/03/icon1-1.png">
							                            </div>
							                            <div class="c-howdoes-bottom display-flex">
							                                <h4>Athletes score &amp; leave Their feedback</h4>
							                            </div>
							                        </div>

							                        <div class="step-area">
							                            <p class="step-count">
							                                Step<span>01</span>
							                            </p>
							                        </div>
							                    </div>
									         									          <div class="col-md-4">
							                      	<div class="c-howdoes__steps-single" style="background-image: url(http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/black-box.png);">
							                            <div class="c-howdoes-top">
							                                <img src="http://dev106.developer24x7.com/cnp910/wp-content/uploads/2020/03/icon2-1.png">
							                            </div>
							                            <div class="c-howdoes-bottom display-flex">
							                                <h4>Users read these reviews</h4>
							                            </div>
							                        </div>

							                        <div class="step-area">
							                            <p class="step-count">
							                                Step<span>02</span>
							                            </p>
							                        </div>
							                    </div>
									         									          <div class="col-md-4">
							                      	<div class="c-howdoes__steps-single" style="background-image: url(http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/black-box.png);">
							                            <div class="c-howdoes-top">
							                                <img src="http://dev106.developer24x7.com/cnp910/wp-content/uploads/2020/03/icon3-1.png">
							                            </div>
							                            <div class="c-howdoes-bottom display-flex">
							                                <h4>Up and down vote</h4>
							                            </div>
							                        </div>

							                        <div class="step-area">
							                            <p class="step-count">
							                                Step<span>03</span>
							                            </p>
							                        </div>
							                    </div>

		                </div>
		            </div>
		            <a href="#" class="btn btn-normal btn-normal--arrow">Register Now</a>
		        </div>
```

### Contact Us Page

On the [Contact Us Page](http://dev106.developer24x7.com/cnp910/contact-us/), insert a generic contact us page that sends responses to [hello@luuply.com](mailto:hello@luuply.com).

### Button margin is incorrect

When the search bar is in the Bootstrap header, the bottom of the search button has a little bit of white showing. Please adjust the margins on this asset.

```
<div class="col-md-1 col-xs-1 remove-space">
		                       <button type="submit" class="btn-submit"><i class="fa fa-search" aria-hidden="true"></i></button>
		              </div>
```

### Add a share button

On a school's page, add a button in here:

```
<div class="rank-review-btn">
                        <a class="btn-gray review-btn" href="http://dev106.developer24x7.com/cnp910/review-submission/?id=381" target="_blank">
                        	<i class="fa fa-star"></i> Write a Review</a>

                         				<a class="btn-gray save-school" href="#">
				                         	<i class="">
				                         		<img src="http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/save-icon.png" alt="save-images">
				                         	</i>
                         					<span>Save</span>
                         				</a>

                         	                    </div>
```

Add a button to share the results of this page:

Destinations:

- Facebook
- Twitter
- By URL
- By email

If user is not logged in, design per model:

![Unauthorized Model Image](https://github.com/luuply/changes/raw/master/20200506/unauthsharemodel.PNG "Unauthorized Model Image")

If user is logged in, design per model:

![Authorized Model Image](https://github.com/luuply/changes/raw/master/20200506/authsharemod.JPG "Authorized Model Image")

### Capitalization

In the roster display on a school page, correct:

```
<ul class="roster-container-by-class"><li><strong>Freshmen</strong> - 19</li><li><strong>Sophomores</strong> - 17</li><li><strong>Juniors</strong> - 9</li><li><strong>seniors</strong> - 7</li></ul>
```

TO

```
<ul class="roster-container-by-class"><li><strong>Freshmen</strong> - 19</li><li><strong>Sophomores</strong> - 17</li><li><strong>Juniors</strong> - 9</li><li><strong>Seniors</strong> - 7</li></ul>
```

### Sign In Page

#### Remove a field

If possible, remove the Username field:

```
<input type="text" name="user[username]" id="username" value="" placeholder="Username" required="">
```

#### SSO authentication

When an user uses SSO to create an account, they should NOT see any login or personal details - those should come from SSO. They should ONLY see profile details.

#### Under profile details

If the user clicks current or former collegiate athlete, present a select menu to ask if they wish to verify their account. If yes, then prompt user to sign in using Facebook SSO ONLY. Verified accounts must be created with Facebook SSO.

### Email verification [BUG]

Email verification is broken. Verification emails take far too long to send, if they arrive at all.

### Homepage and profile page

If a current or former collegiate athlete is not verified, display a banner notification asking if they would like to verify their account.
