<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link href="https://unpkg.com/ionicons@4.5.10-0/dist/css/ionicons.min.css" rel="stylesheet">
    <link rel="stylesheet" href="font-awesome/css/font-awesome.min.css">
    <link href="https://fonts.googleapis.com/css?family=Roboto:400,700&display=swap" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js" integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"></script>
    <link rel="stylesheet" href="css/style.css">
    <link rel="icon" type="image/x-icon" href="images/favicon.ico">
    <title>Checkout</title>
</head>
<body>
    <header id="header">
        <div class="overlay">
            <nav id="navcart" >
              <div class="container-fluid">
                <div class="row">
                  <div class="col-lg-10 col-md-9 col-sm-12">
                    <h4 style="margin-left: 30px;">Products > Cart > Checkout</h4>
                    <br>
                </div>
                <div class="col-lg-2 col-md-3 col-sm-12">
                  
                    <div class="cart">
                        <button type="button" class="btn btn-secondary" onclick="window.history.back();" style="padding: 10px; text-decoration: none; color: white; margin-left: 30px;">Go Back
                        </button>    
                        <style>
                          @media (max-width:425px) {
                            header {
                              height: 200px;
                            }  
                          }
                        </style>
                    </div>
                  </div>
                </div>
              </div>
            </nav>
          </div>
    </header>
    
    <br>
        
<!------CHOOSE PAYMENT MODE-->
    <div class="payment" id="paymentoptionscontainer">
        
        <div class="row" id="paymentradiorow">
          
                <div class="form-check" style="margin-left: 5vw;">
                  <input class="form-check-input" type="radio" id="creditcardradio" name="gridRadios" value="Three">
                          Pay with Credit /or Debit Card
                          <label class="form-check-label" for="creditcardradio">
                          </label>
                          <br>
                </div>
                <div class="form-check" style="margin-left: 5vw;">    
                    <input class="form-check-input" type="radio" id="gcashradio" name="gridRadios" value="Two">
                            Pay with Gcash or Bank Transfer
                            <label class="form-check-label" for="gcashradio">
                            </label>
                            <br>
                </div>            
                <br>
            </form>
        </div>            
    <div class="container">
      
        <!----START of Credit Card payment row-->
        <div class="row justify-content-center align-items-start g-2">
          <div id="showThree" class="myDiv" style="width: 500px;">
              <center><h4><strong>Pay with Credit /or Debit Card </strong></h4></center>
              <p>The amount below already includes our Home Service fee and Gluta Drip Product of your choice.</p>
              <h5>Amount to Pay:  </h5>
              <h6 style="font-size: 2.5vh; color: black; font-weight: 600;">
                  Grand Total = ₱<span id="demo9" style="font-size: 2.5vh; color: black;">0</span>.00 
              </h6>
              <br>
              <center><button type="button" class="btn btn-secondary" onclick="window.history.back()" >Add / Edit Items in Cart
              </button></center>
              <br><br>
              <p><span style="font-size: larger;"><b>Vanity Princess</b></span> is now in partnership with  <a href="https://www.paypal.com"><img width="64" alt="PayPal logo" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/39/PayPal_logo.svg/64px-PayPal_logo.svg.png"></a>, one of the leaders and most trusted in Credit/Debit Card Payment Gateways.</p>
              <p style="color: red;"><b>Please reconfirm below with <a href="https://www.paypal.com"><img width="64" alt="PayPal logo" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/39/PayPal_logo.svg/64px-PayPal_logo.svg.png"></a> the Quantity and Grand Total Amount to be paid.</b></p>
              <p>Then click <b>Debit or Credit Card</b> if you do not have a Paypal account.</p>
              <hr>
<!----TestMode VanityPrincess client id = AbMRn6bYXgi4kj3G6CHkuNuRBvHn6KquOpgPUMF06wo2JBBtTM3TYiVoRNP70743A2dF07bStQktiIEq--->
<!----LiveMode VanityPrincess client id = AUCLSeIyI8k6RdXmkiwx-1Zjq5eR1G7Gpbs_3P9VXf0OayPImojZXcWFVPQtb4hImSi3MUd_iOumgU39--->
<!----Change to Php 50 in line#264 or CHANGE the PRICE in SELECT PRICE ATTRIBUTE-->       
<!----START of Paypal payment----------->
  <div id="smart-button-container">
    <div style="text-align: center;">
      <div style="margin-bottom: 1.25rem;">
        <p>Cindyrella /or Aqua Skin /or Liponex</p>
        <select id="item-options"><option value="Price ea" price="1500">Price ea - 1500 PHP</option></select>
        <select style="visibility: hidden" id="quantitySelect"><option value="1">1</option><option value="2">2</option><option value="3">3</option><option value="4">4</option><option value="5">5</option><option value="6">6</option><option value="7">7</option><option value="8">8</option><option value="9">9</option><option value="10">10</option></select>
      </div>
    <div id="paypal-button-container"></div>
    </div>
  </div>
  <script src="https://www.paypal.com/sdk/js?client-id=AbMRn6bYXgi4kj3G6CHkuNuRBvHn6KquOpgPUMF06wo2JBBtTM3TYiVoRNP70743A2dF07bStQktiIEq&enable-funding=venmo&currency=PHP" data-sdk-integration-source="button-factory"></script>
  <script>
    function initPayPalButton() {
      var shipping = 0;
      var itemOptions = document.querySelector("#smart-button-container #item-options");
      var quantity = parseInt(10);
      var quantitySelect = document.querySelector("#smart-button-container #quantitySelect");
        if (!isNaN(quantity)) {
          quantitySelect.style.visibility = "visible";
        }
      var orderDescription = 'Cindyrella /or Aqua Skin /or Liponex';
        if(orderDescription === '') {
          orderDescription = 'Item';
        }
      paypal.Buttons({
      style: {
      shape: 'pill',
      color: 'gold',
      layout: 'vertical',
      label: 'pay',
    
    },
      createOrder: function(data, actions) {
        var selectedItemDescription = itemOptions.options[itemOptions.selectedIndex].value;
        var selectedItemPrice = parseFloat(itemOptions.options[itemOptions.selectedIndex].getAttribute("price"));
        var tax = (0 === 0 || false) ? 0 : (selectedItemPrice * (parseFloat(0)/100));
          if(quantitySelect.options.length > 0) {
            quantity = parseInt(quantitySelect.options[quantitySelect.selectedIndex].value);
          } else {
            quantity = 1;
          }

        tax *= quantity;
        tax = Math.round(tax * 100) / 100;
        var priceTotal = quantity * selectedItemPrice + parseFloat(shipping) + tax;
        priceTotal = Math.round(priceTotal * 100) / 100;
        var itemTotalValue = Math.round((selectedItemPrice * quantity) * 100) / 100;

        return actions.order.create({
        purchase_units: [{
        description: orderDescription,
        amount: {
        currency_code: 'PHP',
        value: priceTotal,
        breakdown: {
          item_total: {
            currency_code: 'PHP',
            value: itemTotalValue,
          },
            shipping: {
              currency_code: 'PHP',
              value: shipping,
            },
            tax_total: {
              currency_code: 'PHP',
              value: tax,
            }
          }
        },
        items: [{
          name: selectedItemDescription,
          unit_amount: {
            currency_code: 'PHP',
            value: selectedItemPrice,
          },
          quantity: quantity
        }]
      }]
    });
  },
  onApprove: function(data, actions) {
    return actions.order.capture().then(function(orderData) {
      
      // Full available details
      console.log('Capture result', orderData, JSON.stringify(orderData, null, 2));

      // Show a success message within this page, e.g.
      const element = document.getElementById('paypal-button-container');
      //element.innerHTML = '';
      //element.innerHTML = '<h3>Thank you for your payment!</h3>';
      location.replace('thankyoupayment.html');
      localStorage.clear();

      // Or go to another URL:  actions.redirect('thank_you.html');

      });
    },
    onError: function(err) {
      console.log(err);
    },
  }).render('#paypal-button-container');
  }
  initPayPalButton();
  
  </script>
  <br><br><br>
<!----END of Paypal payment-----------> 
              
          </div>
        </div>
<!----END of Credit Card payment row-->
        <br>
<!----START of Gcash payment row-->
        <div class="row justify-content-center align-items-start g-2">
            <div id="showTwo" class="myDiv" style="width: 500px;">
                <center><h4><strong>Pay with Gcash</strong></h4></center>
                <p>The amount below already includes our Home Service fee and Gluta Drip Product of your choice</p>
                <h5>Amount to Pay:  </h5>
                <h6 style="font-size: 2.5vh; color: black; font-weight: 600;">
                    Grand Total = ₱<span id="demo8" style="font-size: 2.5vh; color: black;">0</span>.00 
                </h6>
                <br>
                <center><button type="button" class="btn btn-secondary" onclick="window.history.back()" >Add / Edit Items in Cart
                </button></center>
                <br>
                <hr>
                <p>You may scan our QR code below to proceed with your payment using <span><a href="https://www.gcash.com/"><img src="images/gcashlogo img.jpg" alt="GcashLogo" style="width: 90px;"></a></span></p>
                <p>Alternatively, you may also pay using the details below:</p>
                <ul>
                  <li><b>Gcash Number: 09153542074</b></li>
                  <li><b>Owner: Joseph Eslais</b></li>
                </ul>
                <p style="color: red;">Please do not forget to <b>Save/Download</b> or take a <b>Screenshot</b> image of your payment, and save to your device.</p>
                <br>
                <div class="row">
                  <!---<center><a href="images/vanityprincessQRcode img.jpg" download>Download QR Code to your Device</a></center>--->
                  <!---<br><br>--->
                  <img src="images/vanityprincessQRcode img.png" alt="GcashQRcodeVanityPrincess">
                </div>
                <br>

                <p>Please send the image of your payment to our Facebook Messenger or Viber account, and we will assist in <b>Booking your Appointment.</b></p>
                
                <center><a href="https://www.facebook.com/messages/t/113646558287367"><img src="images/fblogo img.png" alt="" width="50"></a>
                <a href="viber://chat?number=639854670003"><img src="images/viberlogo img.png" alt=""></a></center>
                <br><br>
                <center><button type="button" class="btn btn-secondary" onclick="gcashDone()">DONE</button></center>  
                
            </div>
        </div>
        <!----END of Gcash payment row-->
    </div>
    </div>
        
    <br><br>
  
<!------END CHOOSE PAYMENT MODE-->


        
    <script src="js/main.js"></script>
    <script src="https://unpkg.com/ionicons@4.5.10-0/dist/ionicons.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>

    
<!------JS for GRAND TOTAL AMOUNT TO PAY-->
    <script>
      let cart = localStorage.getItem("totalCost");
      cart = parseInt(cart).toLocaleString();
      let n = cart.valueOf();
      document.getElementById('demo9').innerHTML = n;
      document.getElementById('demo8').innerHTML = n;
      if (!isNan(n)) {
        n.style.visibility = "hidden";
      }
    </script>
    
    <script>
      //if((n) != 'NaN') {
          //n.style.visibility = "hidden";
        //}

        //if (!isNaN(n)) {
        //n.style.visibility = "hidden";}
            //else {
            //document.getElementById('demo').innerHTML = n;
            //document.getElementById('demo8').innerHTML = n;
            //document.getElementById('demo9').innerHTML = n;
          //}
    </script>

<!------JS for CHOOSE PAYMENT MODE-->
    <script>
        $(document).ready(function(){
            $('input[type="radio"]').click(function(){
                var demovalue = $(this).val(); 
                $("div.myDiv").hide();
                $("#show"+demovalue).show();
            });
        });
    </script>
    
    <script>
      function showElement() {
        element = document.querySelector('.payment');
        element.style.visibility = 'visible';
      }
    </script>

    <script>
      function gcashDone() {
        alert('Thank you for your Gcash payment. If you have not been able to Book An Appointment yet, please contact us through our communication channels or send an inquiry on our Contact page.');
        location.replace('index.html');
        localStorage.clear();
        }
    </script>


<!---Mayen's TestCreditCard#	4032038743689097	06/24	828 	any address any phone number any email-->       
<!---Mayen's testmodeClientID sbI = AT3voGiPt1PXeuq5-UqLqFd_qz8-0bFRgBJ8HHFNp1utWpLK2q9WsjUeFRotM-kwhCknsxK2HdN0Ov1b-->
<!----Mayen's live ClientID = AdDk8qOSvh8UtvzdhF26tF8Lc_W67H6wF5FkzDpNUEzM3JKQ78cyerONEfV1TIDQ1qHyzrNwBIJQm4ZJ---->

</body>
</html>
