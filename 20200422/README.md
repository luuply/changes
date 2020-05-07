# Notes for 2020-04-22

## Background image needs changed

In this code block on the homepage (banner-image.jpg needs changed):

```
<header class="c-header" style="background-image: url(http://dev106.developer24x7.com/cnp910/wp-content/uploads/2020/03/banner-image.jpg)">
        <div class="c-header__top">
            <div class="container">
                <div class="row">
                    <div class="col-md-6 col-sm-6">
                        <div class="menu-header-menu-container"><ul id="menu-header-menu" class="header-nav"><li id="menu-item-128" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-128"><a href="http://dev106.developer24x7.com/cnp910/review-submission/">Write a Review</a></li>
<li id="menu-item-27" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-27"><a href="http://dev106.developer24x7.com/cnp910/about-us/">About Us</a></li>
<li id="menu-item-28" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-28"><a href="http://dev106.developer24x7.com/cnp910/contact-us/">Contact Us</a></li>
</ul></div>                    </div>

                    <div class="col-md-6 col-sm-6">
                        
                            <ul class="header-nav login-nv pull-right">
                                <li><a href="http://dev106.developer24x7.com/cnp910/luuply-login">Login</a></li>           
                                <li class="register"><a href="http://dev106.developer24x7.com/cnp910/luuply-registration/">Sign Up</a></li>
                            </ul>

                                            </div>
                </div>
            </div>
        </div>

        <div class="c-header__main">
            <div class="container">
                <div class="row">
                    <div class="col-12 site-top-inner">
                        <figure><img src="http://dev106.developer24x7.com/cnp910/wp-content/uploads/2020/03/home-logo.png" alt=""></figure>
                    </div>
                </div>
            </div>
        </div>

        <!-----------------------------------Start Front Page Search Section-------------------------->

        <div class="c-header__search">
            <div class="container">
                <div class="row">

                    	
				<form method="get" id="advanced-searchform" role="search" action="http://dev106.developer24x7.com/cnp910" data-select2-id="advanced-searchform">

				    <div class="col-md-4 col-xs-4 custom-select2 remove-space">
					    <select name="sport_name" id="sports" class="sports form-control select2-hidden-accessible" data-select2-id="sports" tabindex="-1" aria-hidden="true">
					    	<option data-select2-id="2"></option>
					    	<option value="mens-lacrosse" data-select2-id="5">Men’s Lacrosse</option><option value="womens-lacrosse" data-select2-id="6">Women’s Lacrosse</option>					    </select><span class="select2 select2-container select2-container--default select2-container--below" dir="ltr" data-select2-id="1" style="width: 379px;"><span class="selection"><span class="select2-selection select2-selection--single" role="combobox" aria-haspopup="true" aria-expanded="false" tabindex="0" aria-disabled="false" aria-labelledby="select2-sports-container"><span class="select2-selection__rendered" id="select2-sports-container" role="textbox" aria-readonly="true"><span class="select2-selection__placeholder">Choose a sport</span></span><span class="select2-selection__arrow" role="presentation"><b role="presentation"></b></span></span></span><span class="dropdown-wrapper" aria-hidden="true"></span></span>
					</div>
				    <div class="col-md-7 col-xs-7 remove-space">
					    <input type="text" name="s" id="institute" class="institute form-control" placeholder="Search for a school...">
					</div>
				     <div class="col-md-1 col-xs-1 remove-space">
		                       <button type="submit" class="btn-submit"><i class="fa fa-search" aria-hidden="true"></i></button>
		              </div>
				</form>
	                   
                </div>
            </div>
        </div>

        <!-----------------------------------End Front Page Search Section-------------------------->

    </header>
```
## List Element in Navbar

The list elements should all be level (that is, write a review, about us, and contact us's navbar should be level with the login and sign up buttons)

```
<div class="row">
                    <div class="col-md-6 col-sm-6">
                        <div class="menu-header-menu-container"><ul id="menu-header-menu" class="header-nav"><li id="menu-item-128" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-128"><a href="http://dev106.developer24x7.com/cnp910/review-submission/">Write a Review</a></li>
<li id="menu-item-27" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-27"><a href="http://dev106.developer24x7.com/cnp910/about-us/">About Us</a></li>
<li id="menu-item-28" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-28"><a href="http://dev106.developer24x7.com/cnp910/contact-us/">Contact Us</a></li>
</ul></div>                    </div>

                    <div class="col-md-6 col-sm-6">
                        
                            <ul class="header-nav login-nv pull-right">
                                <li><a href="http://dev106.developer24x7.com/cnp910/luuply-login">Login</a></li>           
                                <li class="register"><a href="http://dev106.developer24x7.com/cnp910/luuply-registration/">Sign Up</a></li>
                            </ul>

                                            </div>
                </div>
```

## Buttons

Button colors should darken slightly on hover, rather than glow.

Remove search bubble (just comment it out, in case we want to implement it later), i.e.,

```
<li class="register"><a href="http://dev106.developer24x7.com/cnp910/luuply-registration/">Sign Up</a></li>
```

or 

```
<button type="submit" class="btn-submit"><i class="fa fa-search" aria-hidden="true"></i></button>
```

## Search bar

In the

```
<input type="text" name="s" id="institute" class="institute form-control" placeholder="Search...">
```

element, start populating results as soon as the user starts typing (like Google AutoFill or Yelp).

Change the text input placeholder to "Search for a school..."

The select's options:

```
<select name="sport_name" id="sports" class="sports form-control select2-hidden-accessible" data-select2-id="sports" tabindex="-1" aria-hidden="true">
					    	<option data-select2-id="2"></option>
					    	<option value="mens-lacrosse" data-select2-id="5">Men’s Lacrosse</option><option value="womens-lacrosse" data-select2-id="6">Women’s Lacrosse</option>					    </select>
```

should be colored differently on hover.

## Homepage Ranking

The ranking on the front page

```
<div class="box-section__single"><h4>Men’s Lacrosse</h4><ol><li>Stanford University- Demo<span></span></li><li>University of Oxford -Demo<span></span></li></ol><a href="http://dev106.developer24x7.com/cnp910/sport/mens-lacrosse/">See Full List</a></div>
```

should be the top five schools.

## Style

### Heading Element Colors

Please style the homepage's heading elements like so:

![alt text](https://github.com/luuply/changes/blob/master/UpdatedStyle.png "Updated Homepage Style")

### Background Color

Change the whole background color (background-color: ;) to #1d1d1e

## Ranking Lists

On click "See Full List" from the home page, if the user is not signed in or signed up, prompt user to sign up. If they are signed in, navigate to `/cnp910/sport/mens-lacrosse/` or `/cnp910/sport/womens-lacrosse/`, show all of the school rankings (not just five). The grey for the entire background should be #1d1d1e and the divs should be #0e0e0e

On `/cnp910/sport/mens-lacrosse/` and `/cnp910/sport/womens-lacrosse/`, the `rankdiv` needs rounded corners (the same as the homepage). The grey should be the background, and the div should be a darker grey (the same as the current background color for Stanford).

## More style

On the homepage (back to /cnp910), remove the entire section:

```
<section class="o-block__connect digital-sec background-darkGray text-center">
		        <div class="container">
		        									    										            <h2 class="">Make your voice heard.</h2>
									            <p>It's time to bring more transparency to the collegiate recruiting system.<br>
Get ready to join the community of people who want to make the system transparent and open for all.</p>
									      		            <figure>
		                <span class="floating floatingbg1bg1"><img src="http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/floating-bg1.png" alt="floating"></span>
		                <span class="floating floatingbg1bg2"><img src="http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/floating-bg2.png" alt="floating"></span>
		                <i class="devices"><img src="http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/conneting-devices.png" alt="conneting-devices"></i>
		                <span class="floating floatingbg1bg3"><img src="http://dev106.developer24x7.com/cnp910/wp-content/themes/luuply/images/floating-bg3.png" alt="floating"></span>
		            </figure>
		        </div>
   	 		</section>
```

## Some JavaScript to do some auto-updating

In this element:

```
<div class="c-aboutus__box">
		                        					                            <h5> Michigan- Demo </h5>
				                            <blockquote>
				                                <h4> </h4>
				                                <p style=""><span class="ratings dashicons dashicons-star-filled"></span><span class="ratings dashicons dashicons-star-filled"></span><span class="ratings dashicons dashicons-star-filled"></span><span class="ratings dashicons dashicons-star-filled"></span><span class="ratings dashicons dashicons-star-empty"></span></p>
				                                <p class="user-quote">orem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been theLorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the.5.1... <a href="http://dev106.developer24x7.com/cnp910/school/michigan/">See more</a></p>
				                            </blockquote>

			                       
		                        </div>
```

Please have it constantly update with new reviews, and specify in an h6 whether it's men's or women's lacrosse (or just the associated sport).

## Button style

For the buttons <a href="http://dev106.developer24x7.com/cnp910/about-us/" class="btn btn-normal btn-normal--arrow">About Us</a>, please change the style of this to not glow, but instead be darker on hover (like the search and sign up from above).

## CSS H1 style change

In your CSS, please change the h1 to color: #1FACEA;.

## Footer

Change `<p class="footer-title">All rights reserved. © Atleta 2020</p>` to `<p class="footer-title">All rights reserved. © Luuply 2020</p>`

## Sign Up page changes

ON `/cnp910/luuply-registration/`

- Please add the "for=" and the element ID for all radios.
- Decrease the letter-spacing: 2px; to 0px (no letter spacing) on the h2 elements.
- Under the SSO buttons, add a <hr> with a "OR" centered - see attached image:

![SSO button style](https://github.com/luuply/changes/blob/master/SSOSignup.png "SSO button style")

- Remove the fieldset border on frame1, frame2, and frame3.

## Search page and results page search bar style

After a search, make the search bar

```
<div class="row">
                            	
				<form method="get" id="advanced-searchform" role="search" action="http://dev106.developer24x7.com/cnp910">

				    <div class="col-md-4 col-xs-4 custom-select2 remove-space">
					    <select name="sport_name" id="sports" class="sports form-control select2-hidden-accessible" data-select2-id="sports" tabindex="-1" aria-hidden="true">
					    	<option data-select2-id="2"></option>
					    	<option value="mens-lacrosse">Men’s Lacrosse</option><option value="womens-lacrosse">Women’s Lacrosse</option>					    </select><span class="select2 select2-container select2-container--default" dir="ltr" data-select2-id="1" style="width: 189px;"><span class="selection"><span class="select2-selection select2-selection--single" role="combobox" aria-haspopup="true" aria-expanded="false" tabindex="0" aria-disabled="false" aria-labelledby="select2-sports-container"><span class="select2-selection__rendered" id="select2-sports-container" role="textbox" aria-readonly="true"><span class="select2-selection__placeholder">Choose a sport</span></span><span class="select2-selection__arrow" role="presentation"><b role="presentation"></b></span></span></span><span class="dropdown-wrapper" aria-hidden="true"></span></span>
					</div>
				    <div class="col-md-7 col-xs-7 remove-space">
					    <input type="text" name="s" id="institute" class="institute form-control" placeholder="Search...">
					</div>
				     <div class="col-md-1 col-xs-1 remove-space">
		                       <button type="submit" class="btn-submit"><i class="fa fa-search" aria-hidden="true"></i></button>
		              </div>
				</form>
	                        </div>
```
as white #FFFFFF instead.

## School page

On the search results page, remove the conference (i.e., Ivy League), only display the school name.

On a school's page, change the text styling to the attached image:

![School page style](https://github.com/luuply/changes/blob/master/schoolpagestyle.png "School page style")

In this element:

```
<div class="review-mid-sec text-center">
                            <p class="stars">
                            	<span class="ratings dashicons dashicons-star-filled"></span>
                            	<span class="ratings dashicons dashicons-star-filled"></span>
                            	<span class="ratings dashicons dashicons-star-filled"></span>
                            	<span class="ratings dashicons dashicons-star-filled"></span>
                            	<span class="ratings dashicons dashicons-star-filled"></span>
                            </p>
                            <p>Start your review of <strong>Harvard University- Ivy League</strong></p>
                        </div>
```

Change the icons so that they fill and style when hovered over, and add some help text for each rating (meh, like it, hate it, etc.)

