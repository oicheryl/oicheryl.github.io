---
layout: page
title: Sponsor one month of Cloud Native London
description: "Sponsor one month of Cloud Native London credit or debit card."
---

<!-- Load Stripe.js on your website. -->
<script src="https://js.stripe.com/v3"></script>

{% if jekyll.environment == "production" %}
{% include stripe1mon.html %}
{% else %}
{% include stripe-test.html %}
{% endif %}
