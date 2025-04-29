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

> **Payee name:** Cloud Native London Ltd  
> **Sort code:** 60-83-71  
> **Account number:** 57049586  
> **IBAN:** GB33SRLG60837157049586  
> **SWIFT/BIC:** SRLGGB2L  
> **Reference:** On invoice   

### Direct debit (monthly sponsorship)

<button class="gocardless" onclick="location.href='https://pay.gocardless.com/AL0005Y5QAX5A6'" type="button">Monthly subscription - Direct debit</button> {% if jekyll.environment == "production" %}
{% include stripe-monthly.html %}
{% else %}
{% include stripe-monthly-test.html %}
{% endif %}

