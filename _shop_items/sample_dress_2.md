---
layout: default
slug: samplePracticeDress2
name: Sample practice dress 2
description: Sample text about practice dress. Dresses come in all sizes!
price: "200.00"
collection: dancewear
button_id: NV5784KBL6YJ4
img_src: /images/insta-min.jpg
---
<img class="img-fluid rounded" src="{{ page.img_src }}"/>
<div class="shop-item-header">
  <div class="shop-item-name">{{ page.name }}</div>
  <div>${{ page.price }}</div>
</div>
<p class="shop-item-description">{{ page.description }}</p>
<form  target="paypal" action="https://www.paypal.com/cgi-bin/webscr" method="post">
  <input type="hidden" name="cmd" value="_s-xclick">
  <input type="hidden" name="hosted_button_id" value="{{ page.button_id }}">
  <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_cart_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
  <img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
</form>
