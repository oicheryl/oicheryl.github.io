<!-- Create a button that your customers click to complete their purchase. Customize the styling to suit your branding. -->
<button class="stripe" id="checkout-button-sku_FcKSyxgCZkGGfx" role="link">
  1 month
</button> 

<div id="error-message"></div>

<script>
  var stripe = Stripe('pk_live_gRovPiGzsmDnzUPZlDt4mR6U00q124AvQ7');

  var checkoutButton = document.getElementById('checkout-button-sku_FcKSyxgCZkGGfx');
  checkoutButton.addEventListener('click', function () {
    // When the customer clicks on the button, redirect
    // them to Checkout.
    stripe.redirectToCheckout({
      items: [{sku: 'sku_FcKSyxgCZkGGfx', quantity: 1}],

      // Do not rely on the redirect to the successUrl for fulfilling
      // purchases, customers may not always reach the success_url after
      // a successful payment.
      // Instead use one of the strategies described in
      // https://stripe.com/docs/payments/checkout/fulfillment
      successUrl: 'https://www.oicheryl.com/cloudnativelondon/success',
      cancelUrl: 'https://www.oicheryl.com/cloudnativelondon/pay',
    })
    .then(function (result) {
      if (result.error) {
        // If `redirectToCheckout` fails due to a browser or network
        // error, display the localized error message to your customer.
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
</script>
