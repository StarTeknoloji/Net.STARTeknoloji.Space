<!-- Place on one of your landing pages or pre-checkout pages -->
<body>
  <script
    src="https://www.paypal.com/sdk/js?client-id=CLIENT_ID" async>
  </script>
</body>

<div id="paypal-button-container"></div>

<script>
   document.querySelector('#paypal-button-container')
     .style.display = 'none';

   paypal.Buttons().render('#paypal-button-container');

   document.querySelector('#myRadioField')
     .addEventListener('click', function() {
       document.querySelector('#paypal-button-container')
         .style.display = 'block';
     });
</script>
