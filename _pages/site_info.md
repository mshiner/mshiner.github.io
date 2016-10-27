I decided to start this Jekyll build because of my dissatisfaction with Wordpress.

We were using it with various plugins and the site became a bit of a management hassle.

Originally the site was conceived as a place where rides starting in Brent Knoll and the surrounding area can be
posted centrally without the email round robin. Then things got out of hand.

This particular file is written in Markdown, but it has no YAML front matter so is ignored by the build. It is included in the site index so you can write your home page without any html tags.

{% include calendar-subscribe.html %}

To include a frame of the next ride....

## Next ride

{% include nextride.html %}

You can, if you wish, add raw html to, for example, display and iFrame....


### BKVelo on Strava


{% raw %}
<iframe frameborder="no" width="310" height="160" frameborder="0" allowtransparency="true" scrolling="no" src="https://www.strava.com/clubs/125486/latest-rides/78867fa14f1d2f7799cfe79e53d1969d89e59d29?show_rides=false"></iframe>
{% endraw %}


Or a map....

### How to get to Sweet's Tea Rooms

<div>
<iframe width="310" height="255" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="https://maps.google.com/maps?q=Sweetscafewesthaysomerset&amp;ie=UTF8&amp;&amp;output=embed"></iframe>
</div>


Or a twitter timeline....

<div>
  <a class="twitter-timeline"
  href="https://twitter.com/bkvelo"
  width="310"
  height="300"
  data-tweet-limit="3">
  Tweets by bkvelo
  </a>
  <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
</div>
