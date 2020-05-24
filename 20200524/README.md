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

