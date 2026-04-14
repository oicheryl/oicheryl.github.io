---
layout: page
title: Choose payment method
description: "Pay Cloud Native London by bank transfer or card."
---

<!-- Load Stripe.js on your website. -->
<script src="https://js.stripe.com/v3"></script>

### Pay by credit card

{% if jekyll.environment == "production" %}
{% include stripe.html %}
{% else %}
{% include stripe-test.html %}
{% endif %}


### Pay by bank transfer

<script type="text/javascript" src="https://form.jotform.com/jsform/261034786613054"></script>

### Direct debit (monthly sponsorship)

<button class="gocardless" onclick="location.href='https://pay.gocardless.com/AL0005Y5QAX5A6'" type="button">Monthly subscription - Direct debit</button> {% if jekyll.environment == "production" %}
{% include stripe-monthly.html %}
{% else %}
{% include stripe-monthly-test.html %}
{% endif %}

