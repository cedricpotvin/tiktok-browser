# TikTok Browser Tracking Template For Google Tag Manager
This template helps you to setup the TikTok tracking pixel on your website using Google Tag Manager.

<H2>Getting Started</h2>
<p>Paste the pixel code at the top of the <b>header section</b> on your website.</p>
<pre> <script>
!function (w, d, t) {
  w.TiktokAnalyticsObject=t;var ttq=w[t]=w[t]||[];ttq.methods=["page","track","identify","instances","debug","on","off","once","ready","alias","group","enableCookie","disableCookie"],ttq.setAndDefer=function(t,e){t[e]=function(){t.push([e].concat(Array.prototype.slice.call(arguments,0)))}};for(var i=0;i<ttq.methods.length;i++)ttq.setAndDefer(ttq,ttq.methods[i]);ttq.instance=function(t){for(var e=ttq._i[t]||[],n=0;n<ttq.methods.length;n++)ttq.setAndDefer(e,ttq.methods[n]);return e},ttq.load=function(e,n){var i="https://analytics.tiktok.com/i18n/pixel/events.js";ttq._i=ttq._i||{},ttq._i[e]=[],ttq._i[e]._u=i,ttq._t=ttq._t||{},ttq._t[e]=+new Date,ttq._o=ttq._o||{},ttq._o[e]=n||{};var o=document.createElement("script");o.type="text/javascript",o.async=!0,o.src=i+"?sdkid="+e+"&lib="+t;var a=document.getElementsByTagName("script")[0];a.parentNode.insertBefore(o,a)};
  ttq.load('[YOUR PIXEL ID WILL BE LOCATED HERE]');
  ttq.page();
}(window, document, 'ttq');
</script>
</pre>
<p>You should replace <code>[YOUR PIXEL ID WILL BE LOCATED HERE]</code> with the pixel ID that TikTok provided you you.</p>

<P> <b>Please note:</b> you can also install this code using a Custom HTML tag inside Google Tag manager</p>

![image](https://user-images.githubusercontent.com/60415400/195393343-471ee1ac-49eb-492d-a363-514f65cc4aa1.png)

<h3>Use The Template</h3>
<p>1. Upload the template.tpl file to your web container by navigating to the "Templates" tab inside Google Tag manager.<br>
  2. Create a new tag and select the the <b>TikTok Pixel</b> template.<br>
  3. Insert your Pixel ID.<br>
  4. Select the event you want to send from the following options:<br>
  <code>Add Payment Info</code> <code>Add to Cart</code> <code>Add to Wishlist</code> <code>Click Button</code> <code>Complete Payment</code> <code>Complete Registration</code> <code>Contact</code> <code>Download</code> <code>Initiate Checkout</code> <code>Place an Order</code> <code>Search</code> <code>Submit Form</code> <code>Subscribe</code> <code>View Content</code>.</br>
  5. You can add event parameters. Please follow TikToks documentation: https://ads.tiktok.com/help/article?aid=10028.<br>
  6. If you're also doing server tracking you will need to add an event ID for each of your events.<br> 
