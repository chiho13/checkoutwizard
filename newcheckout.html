<!doctype html>
<html lang="en">
<head>
	<meta charset="utf-8" />

	<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
	<title>Checkout | Style Minions</title>

	<meta content='width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0' name='viewport' />
  <meta name="viewport" content="width=device-width" />

    <!--checkout product --> 

  <link rel="stylesheet" href="http://weloveiconfonts.com/api/?family=entypo">
  <link rel='stylesheet prefetch' href='http://static.bveneman.nl/utf-latest.min.css'>

   <!--base css-->

  <link rel="icon" type="image/png" href="assets/img/favicon.ico">
  <link href="css/bootstrap.css" rel="stylesheet" />
	<link href="css/gsdk-base.css" rel="stylesheet" />
  <link href="css/newcheckout.css" rel="stylesheet" />  
  <!-- <link href="http://netdna.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.css" rel="stylesheet"> -->

  <!--Validator css --> 

<link rel="stylesheet" href="css/bootstrap-formhelpers-min.css" media="screen">
<link rel="stylesheet" href="css/bootstrapValidator-min.css"/>
<link rel="stylesheet" href="css/bootstrap-side-notes.css" />

  <!-- Stripe -->
  <script type="text/javascript" src="https://js.stripe.com/v2/"></script>

  <!--Validator --> 

  <script type="text/javascript" src="js/bootstrapValidator-min.js"></script>
  <script src="js/bootstrap-formhelpers-min.js"></script>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>

   <script type="text/javascript">
  $(document).ready(function() {
    $('#payment-form').bootstrapValidator({
        message: 'This value is not valid',
        feedbackIcons: {
            valid: 'glyphicon glyphicon-ok',
            invalid: 'glyphicon glyphicon-remove',
            validating: 'glyphicon glyphicon-refresh'
        },
    submitHandler: function(validator, form, submitButton) {
                    // createToken returns immediately - the supplied callback submits the form if there are no errors
                    Stripe.card.createToken({
                        number: $('.card-number').val(),
                        cvc: $('.card-cvc').val(),
                        exp_month: $('.card-expiry-month').val(),
                        exp_year: $('.card-expiry-year').val(),
      name: $('.card-holder-name').val(),
      address_line1: $('.address').val(),
      address_city: $('.city').val(),
      address_zip: $('.zip').val(),
      address_state: $('.state').val(),
      address_country: $('.country').val()
                    }, stripeResponseHandler);
                    return false; // submit from callback
        },
        fields: {
            street: {
                validators: {
                    notEmpty: {
                        message: 'The street is required and cannot be empty'
                    },
          stringLength: {
                        min: 6,
                        max: 96,
                        message: 'The street must be more than 6 and less than 96 characters long'
                    }
                }
            },
            city: {
                validators: {
                    notEmpty: {
                        message: 'The city is required and cannot be empty'
                    }
                }
            },
      zip: {
                validators: {
                    notEmpty: {
                        message: 'The zip is required and cannot be empty'
                    },
          stringLength: {
                        min: 3,
                        max: 9,
                        message: 'The zip must be more than 3 and less than 9 characters long'
                    }
                }
            },
            email: {
                validators: {
                    notEmpty: {
                        message: 'The email address is required and can\'t be empty'
                    },
                    emailAddress: {
                        message: 'The input is not a valid email address'
                    },
          stringLength: {
                        min: 6,
                        max: 65,
                        message: 'The email must be more than 6 and less than 65 characters long'
                    }
                }
            },
      cardholdername: {
                validators: {
                    notEmpty: {
                        message: 'The card holder name is required and can\'t be empty'
                    },
          stringLength: {
                        min: 6,
                        max: 70,
                        message: 'The card holder name must be more than 6 and less than 70 characters long'
                    }
                }
            },
      cardnumber: {
    selector: '#cardnumber',
                validators: {
                    notEmpty: {
                        message: 'The credit card number is required and can\'t be empty'
                    },
          creditCard: {
            message: 'The credit card number is invalid'
          },
                }
            },
      expMonth: {
                selector: '[data-stripe="exp-month"]',
                validators: {
                    notEmpty: {
                        message: 'The expiration month is required'
                    },
                    digits: {
                        message: 'The expiration month can contain digits only'
                    },
                    callback: {
                        message: 'Expired',
                        callback: function(value, validator) {
                            value = parseInt(value, 10);
                            var year         = validator.getFieldElements('expYear').val(),
                                currentMonth = new Date().getMonth() + 1,
                                currentYear  = new Date().getFullYear();
                            if (value < 0 || value > 12) {
                                return false;
                            }
                            if (year == '') {
                                return true;
                            }
                            year = parseInt(year, 10);
                            if (year > currentYear || (year == currentYear && value > currentMonth)) {
                                validator.updateStatus('expYear', 'VALID');
                                return true;
                            } else {
                                return false;
                            }
                        }
                    }
                }
            },
            expYear: {
                selector: '[data-stripe="exp-year"]',
                validators: {
                    notEmpty: {
                        message: 'The expiration year is required'
                    },
                    digits: {
                        message: 'The expiration year can contain digits only'
                    },
                    callback: {
                        message: 'Expired',
                        callback: function(value, validator) {
                            value = parseInt(value, 10);
                            var month        = validator.getFieldElements('expMonth').val(),
                                currentMonth = new Date().getMonth() + 1,
                                currentYear  = new Date().getFullYear();
                            if (value < currentYear || value > currentYear + 100) {
                                return false;
                            }
                            if (month == '') {
                                return false;
                            }
                            month = parseInt(month, 10);
                            if (value > currentYear || (value == currentYear && month > currentMonth)) {
                                validator.updateStatus('expMonth', 'VALID');
                                return true;
                            } else {
                                return false;
                            }
                        }
                    }
                }
            },
      cvv: {
    selector: '#cvv',
                validators: {
                    notEmpty: {
                        message: 'The cvv is required and can\'t be empty'
                    },
          cvv: {
                        message: 'The value is not a valid CVV',
                        creditCardField: 'cardnumber'
                    }
                }
            },
        }
    });
});
</script>
<script type="text/javascript">
            // this identifies your website in the createToken call below
            Stripe.setPublishableKey('<Stripe Publishable Key>');
 
            function stripeResponseHandler(status, response) {
                if (response.error) {
                    // re-enable the submit button
                    $('.submit-button').removeAttr("disabled");
          // show hidden div
          document.getElementById('a_x200').style.display = 'block';
                    // show the errors on the form
                    $(".payment-errors").html(response.error.message);
                } else {
                    var form$ = $("#payment-form");
                    // token contains id, last4, and card type
                    var token = response['id'];
                    // insert the token into the form so it gets submitted to the server
                    form$.append("<input type='hidden' name='stripeToken' value='" + token + "' />");
                    // and submit
                    form$.get(0).submit();
                }
            }
 

</script>

</head>
<style>
      /* NOTE: The styles were added inline because Prefixfree needs access to your styles and they must be inlined if they are on local disk! */
      [class*="entypo-"]:before { font-family: 'entypo', sans-serif; }
body {
  background-color: #ecf0f1;
  font: 300 1.25em/1.4 "Lato", sans-serif;
  color: #686868;
}
h1, h2, h3, h4, h5, h6 { font-weight: 400; }
h1, .sub-heading {
  text-align: center;
  margin: .5rem 0 1rem;
}
.sub-heading {
  font-size: .75em;
  font-weight: 300;
}

/**
 * @section: utilities;
 * @see: Justify Grid [http://justifygrid.com/]
 */
._grid {
  text-align: justify !important;
  text-justify: distribute-all-lines;
  font-size: 0 !important;
  text-rendering: optimizespeed;
}
._grid:after {
  content: "";
  display: inline-block;
  width: 100%;
}
._column {
  display: inline-block;
  vertical-align: top;
  font-size: medium;
  text-align: left;
  text-rendering: optimizeLegibility;
}
._btn {
  display: inline-block;
  background-color: #bdc3c7;
  border: none;
  padding: .5em .75em;
  text-align: center;
  font-weight: 300;
}
._btn:hover,
.cart-totals:hover ._btn {
  background-color: #790E7D;
  color: #ecf0f1;
  transition: 0.3s all ease;
}

/**
 * @section: shopping-cart;
 */
.shopping-cart {
  width: 100%;
  max-width: 71rem;
  margin: 0 auto;
}
/**
 * @extends: _grid;
 */
.shopping-cart--list-item {
  border: 1px solid #bdc3c7;
  margin-bottom: 3rem;
  height: 10rem;
  overflow: hidden;
}
.shopping-cart--list-item:hover,
.shopping-cart--list-item:hover * {
  border-color: #790E7D;
  transition: 0.3s all;
}
.shopping-cart--list-item > ._column {
    height: 100%; /* make vertical lines match */
}

/**
 * @section: product-image;
 * @extends: _column;
 */
/*.product-image {
  width: 16.663198%;
  background: url("data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7") no-repeat center / cover transparent;
}*/

/**
 * @section: product-info;
 * @extends: _column;
 */
.product-info {
  width: 67.832119%;
  padding: .5rem;
}
.product-name {
  font: 200 1.4em/1 "Lato", sans-serif;
  letter-spacing: -.025em;
  margin: 0 0 .125em;
  padding:0.5rem;
}
.price {
  line-height: 1;
  text-align: right;
}
.product-single-price {
  margin-top: -1rem;
  font-size: 1.4em;
}

.product-desc {
  padding-left:0.5rem;
}
/**
 * @section: product-modifiers;
 * @extends: _column;
 */
.product-modifiers {
  width: 15.496358%;
  text-align: right;
  border-left: 1px solid #bdc3c7;
}
.product-subtract,
.product-plus,
.product-qty {
  width: 33.330557%;
  background-color: transparent;
  color: #686868;
  text-align: center;
}
.product-qty {
  padding: .35em .75em;
}
.product-remove {
  font-size: .875em;
  margin-top: 2.75rem;
  background-color: #e74c3c;
  color: #ecf0f1;
  width: 100%;
  visibility: hidden;
}
.product-modifiers:hover .product-remove {
  visibility: visible;
  transition: 0.3s all ease;
}
.product-remove:before {
  margin-right: .5em;
}
.product-remove:hover {
  background-color: #c0392b;
}
.product-total-price {
  border-top: 1px solid #bdc3c7;
  color: #95a5a6;
  font-size: 1.25em;
  padding: .5rem;
}
.shopping-cart--list-item:hover .product-total-price {
  background-color: #3498db;
  color: #ecf0f1;
}

/**
 * @section: cart-totals;
 * @extends: _grid;
 */
.cart-totals {
  border-top: 1px solid #bdc3c7;
  margin-bottom: 3rem;
}
.cart-totals ._column {
  width: 19.984013%;
  padding: .6rem;
  line-height: 1.2;
}
.cart-totals ._column:not(:last-of-type) {
  border-right: 1px solid #bdc3c7;
}
.cart-totals ._column:first-of-type {
  padding-left: 23px;
}
.cart-totals-key {
  font-size: 1.125em;
  color: #bdc3c7;
}
.cart-totals ._column:hover .cart-totals-value,
.cart-totals ._column:hover .cart-totals-key {
  color: #333;
}
.cart-totals-value {
  font-size: 1.6em;
}
._column.checkout {
  text-align: right;
  padding: 0;
  margin-top: 1.5em;
  vertical-align: middle;
}
.checkout-btn:before {
  margin-right: .5em;
}
._btn.checkout-btn:hover {
  background-color: #2980b9;
}

/**
 * Animations
 */
.product-remove,
.cart-totals * {
  transition: all .2s ease;
}
.closing {
  transition: all .5s ease;
  transform: translate3d(0, -100%, 0);
  opacity: 0;
}

@media(max-width:1200px){
  .cart-totals-value {
    font-size: 1.4em;
}
}

/**996px change margin **/ 

@media(max-width:991px){
  .cart-totals-value {
    font-size: 1.3em;
}

}

@media(max-width:600px){
  .product-info {
  width: 61.832119%;
}
.product-modifiers {
    width: 21.496358%;
    text-align: right;
    border-left: 1px solid #bdc3c7;
}

.product-qty {
    padding: 0.35em .35em;
}

.product-name {
      font: 200 1.2em/1 "Lato", sans-serif;

}
.cart-totals ._column:first-of-type {
  padding-left: 0 ;
}

.product-desc {
  font-size: 0.9em;
}

.product-single-price {
  margin-top: 0rem;
  font-size: 1.2em;
}

.product-remove span {
  display:none;
}

.entypo-trash {
  padding-left: 16px
}

}

    </style>
<body>
<div class="image-container set-full-height" style="background-image: url('assets/img/wizard-boat.jpg')">
    

    <!--   Big container   -->
    <div class="container">
        <div class="row">
        <div class="col-sm-8 col-sm-offset-2">

            <!--      Wizard container        -->
            <div class="wizard-container">
                <div class="card wizard-card ct-wizard-azzure" id="wizard">
                    <form action="" method="">
                <!--        You can switch "ct-wizard-azzure"  with one of the next bright colors: "ct-wizard-blue", "ct-wizard-green", "ct-wizard-orange", "ct-wizard-red"             -->

                    	<div class="wizard-header">
                        	<h3>
                        	   CHECKOUT <br>
                        	  
                        	</h3>
                    	</div>
                    	<ul>
                            <li><a href="#orders" data-toggle="tab">Orders</a></li>
                            <li><a href="#shipping" data-toggle="tab">Shipping</a></li>
                            <li><a href="#pay" data-toggle="tab">Pay</a></li>
                        </ul>

                        <div class="tab-content">
                            <div class="tab-pane" id="orders">
                              

                <section class="shopping-cart">
                  <ol class="ui-list shopping-cart--list" id="shopping-cart--list">
                    <script id="shopping-cart--list-item-template" type="text/template">
                      <li class="_grid shopping-cart--list-item">
                        <div class="_column product-image">
                          <img class="product-image--img" src="{{=img}}" alt="Item image" />
                        </div>
                        <div class="_column product-info">
                          <h4 class="product-name">{{=name}}</h4>
                          <p class="product-desc">{{=desc}}</p>
                          <div class="price product-single-price">${{=price}}</div>
                        </div>
                        <div class="_column product-modifiers" data-product-price="{{=price}}">
                          <div class="_grid">
                            <button type="button" class="_btn _column product-subtract">&minus;</button>
                            <div class="_column product-qty">0</div>
                            <button type="button" class="_btn _column product-plus">&plus;</button>
                          </div>
                          <button class="_btn entypo-trash product-remove"><span>Remove</span></button>
                          <div class="price product-total-price">$0.00</div>
                        </div>
                      </li>
                    </script>
                    <script src='http://cdnjs.cloudflare.com/ajax/libs/zepto/1.0/zepto.min.js'></script>

                  <script src="js/newcheckout.js"></script>
                  </ol>

                    <footer class="_grid cart-totals">
                      <div class="_column subtotal" id="subtotalCtr">
                        <div class="cart-totals-key">Total</div>
                        <div class="cart-totals-value">$0.00</div>
                      </div>
                     <!--  <div class="_column shipping" id="shippingCtr">
                        <div class="cart-totals-key">Shipping</div>
                        <div class="cart-totals-value">$0.00</div>
                      </div>
                      <div class="_column taxes" id="taxesCtr">
                        <div class="cart-totals-key">HST</div>
                        <div class="cart-totals-value">$0.00</div>
                      </div>
                      <div class="_column total" id="totalCtr" onload="copyDiv();">
                        <div class="cart-totals-key">Total</div>
                        <div class="cart-totals-value" id="mydiv1">$0.00</div>
                      </div> -->
                    </footer>
                
                  </section>
                </div>


                            <div class="tab-pane" id="shipping">
                                
                                <div class="row">
                                    <div class="col-sm-12">

                                  <h4 class="shippingheader">Shipping Address
                                  <!-- <small>
                                    <button type="button" class ="btn btn-primary btn-sm btn-add" data-toggle="collapse" data-target="#billingaddress" aria-expanded="false" aria-controls="billingaddress">
                                       <span class="fa fa-plus" ></span> Add
                                      </button>
                                    
                                  </small> -->

                                 </h4> 
                                
                                <!-- <div class="collapse" id="billingaddress"> -->
                                   <form>   
                                    <fieldset>


                                    <div class="col-sm-5 col-sm-offset-1">
                                         <div class="form-group">
                                            <label>Full Name</label>
                                            <input type="text" class="form-control" placeholder="">
                                          </div>
                                    </div>  
                                      <div class="col-sm-5">
                                         <div class="form-group">
                                            <label>Email</label>
                                            <input type="email" class="form-control" placeholder="">
                                          </div>
                                    </div>  
                                    <div class="col-sm-2 col-sm-offset-1">
                                         <div class="form-group">
                                            <label>Street No.</label>
                                            <input type="text" class="form-control" placeholder="">
                                          </div>
                                    </div>
                                    <div class="col-sm-5 ">
                                         <div class="form-group">
                                            <label>Street Name</label>
                                            <input type="text" class="form-control" placeholder="">
                                          </div>
                                    </div>
                                    
                                    <div class="col-sm-3 ">
                                         <div class="form-group">
                                            <label>State/Province</label>
                                            <input type="text" class="form-control" placeholder="ON">
                                          </div>
                                    </div>
                                    
                                    <div class="col-sm-4 col-sm-offset-1">
                                         <div class="form-group">
                                            <label>City</label>
                                            <input type="text" class="form-control" placeholder="Toronto">
                                          </div>
                                    </div>
                                    <div class="col-sm-3">
                                         <div class="form-group">
                                            <label>Country</label><br>
                                             <select name="country" class="form-control">
                                                <option value="Canada"> Canada </option>
                                                <option value="Albania"> Albania </option>
                                                <option value="Algeria"> Algeria </option>
                                                <option value="American Samoa"> American Samoa </option>
                                                <option value="Andorra"> Andorra </option>
                                                <option value="Angola"> Angola </option>
                                                <option value="Anguilla"> Anguilla </option>
                                                <option value="Antarctica"> Antarctica </option>
                                                <option value="...">...</option>
                                            </select>
                                          </div>
                                    </div>

                                    <div class="col-sm-3">
                                         <div class="form-group">
                                            <label>Zip Code</label>
                                            <input type="text" class="form-control" placeholder="">
                                          </div>
                                    </div>
                                    </fieldset>
                                    
                               <!--  </div> -->
                                <hr class="breakform">
                                <div class="row">

                                <!-- <h4 class="billingheader" > Billing Address </h4> -->

                                
                                <div id="check-awesome" class="form-group col-sm-12">    
                                     <input type="checkbox" id="check-me" checked>  
                                       
                                     <label for="check-me">
                                         <span class="circle"></span>
                                         <span class="check"></span>
                                         <span class="box"></span>
                                         <p class="billing"> Billing Address is the same as Shipping Address (uncheck if different) </p>
                                     </label>  

                                    </div>

                                    <hr>


                                   <section id="billingaddress">  

                                    <div class="col-sm-2 col-sm-offset-1">
                                         <div class="form-group">
                                            <label>Street No.</label>
                                            <input type="text" class="form-control" placeholder="">
                                          </div>
                                    </div>

                                    <div class="col-sm-5 ">
                                         <div class="form-group">
                                            <label>Street Name</label>
                                            <input type="text" class="form-control" placeholder="">
                                          </div>
                                    </div>
                                    
                                    <div class="col-sm-3 ">
                                         <div class="form-group">
                                            <label>State/Province</label>
                                            <input type="text" class="form-control" placeholder="ON">
                                          </div>
                                    </div>
                                    
                                    <div class="col-sm-4 col-sm-offset-1">
                                         <div class="form-group">
                                            <label>City</label>
                                            <input type="text" class="form-control" placeholder="Toronto">
                                          </div>
                                    </div>
                                    <div class="col-sm-3">
                                         <div class="form-group">
                                            <label>Country</label><br>
                                             <select name="country" class="form-control">
                                                <option value="Canada"> Canada </option>
                                                <option value="Albania"> Albania </option>
                                                <option value="Algeria"> Algeria </option>
                                                <option value="American Samoa"> American Samoa </option>
                                                <option value="Andorra"> Andorra </option>
                                                <option value="Angola"> Angola </option>
                                                <option value="Anguilla"> Anguilla </option>
                                                <option value="Antarctica"> Antarctica </option>
                                                <option value="...">...</option>
                                            </select>
                                          </div>
                                    </div>

                                    <div class="col-sm-3">
                                         <div class="form-group">
                                            <label>Zip/Postal Code</label>
                                            <input type="text" class="form-control" placeholder="">
                                          </div>
                                    </div>
                                    </section>
                                  </form>
                                  </div>
                                        <!-- <div class="col-sm-4 col-sm-offset-2">
                                            <div class="choice" data-toggle="wizard-radio" rel="tooltip" title="Renters you approve will be able to take this boat">
                                                <input type="radio" name="job" value="Design">
                                                <div class="icon">
                                                    <i class="fa fa-life-ring"></i>
                                                </div>
                                                <h6>No Captain</h6>
                                            </div>
                                        </div>
                                        <div class="col-sm-4">
                                            <div class="choice" data-toggle="wizard-radio" rel="tooltip" title="Select this option if you or a certified captain will be included.">
                                                <input type="radio" name="job" value="Code">
                                                <div class="icon">
                                                    <i class="fa fa-male"></i>
                                                </div>
                                                <h6>Includes Captain</h6>
                                            </div>

                                        </div> -->
                                    </div>
                                </div>
                            </div>
                            <div class="tab-pane" id="pay">
                                <!-- <div class="row">
                                    <h4 class="info-text"> Drop us a small description </h4>
                                    <div class="col-sm-6 col-sm-offset-1">
                                         <div class="form-group">
                                            <label>Boat description</label>
                                            <textarea class="form-control" placeholder="" rows="9">

                                            </textarea>
                                          </div>
                                    </div>
                                    <div class="col-sm-4">
                                         <div class="form-group">
                                            <label>Example</label>
                                            <p class="description">"The boat really nice name is recognized as being a really awesome boat. We use it every sunday when we go fishing and we catch a lot. It has some kind of magic shield around it."</p>
                                          </div>
                                    </div>
                                </div> -->
                                <form action="" method="POST" id="payment-form">
                                   <!-- <span class="payment-errors"></span>

                                   <div class="col-sm-2 col-sm-offset-1 form-group">
                                     <label>
                                       <span>Card Number</span>
                                       <input class="form-control" type="text" size="20" data-stripe="number"/>
                                     </label>
                                   </div>

                                   <div class="form-group">
                                     <label>
                                       <span>CVC</span>
                                       <input class="form-control" type="text" size="4" data-stripe="cvc"/>
                                     </label>
                                   </div>

                                   <div class="form-group">
                                     <label>
                                       <span>Expiration (MM/YYYY)</span>
                                       <input type="text" size="2" data-stripe="exp-month"/>
                                     </label>
                                     <span> / </span>
                                     <input type="text" size="4" data-stripe="exp-year"/>
                                   </div> -->

                                   <!-- <div class="col-sm-5 col-sm-offset-1">
                                         <div class="form-group">
                                            <label>Card Number</label>
                                            <input type="text" class="form-control" size="20" data-stripe="number">
                                          </div>
                                    </div>
                                    <div class="row">
                                    <div class="col-sm-2 ">
                                         <div class="form-group">
                                     <label>
                                       <span>CVC</span>
                                       <input class="form-control" type="text" size="4" data-stripe="cvc"/>
                                     </label>
                                   </div>
                                    </div>
                                    </div>
                                    
                                    <div class="col-sm-3 ">
                                         <div class="form-group">
                                           <label>
                                             <span>Expiration (MM/YYYY)</span>
                                             <input type="text" size="2" class="form-control"  data-stripe="exp-month"/>
                                           </label>
                                           <span> / </span>
                                           <input type="text" size="4" class="form-control" data-stripe="exp-year"/>
                                   </div> 
                                    </div> -->

<fieldset>
    <legend style="text-indent: 10px">Card Details</legend> 
    
    <!-- Card Holder Name -->
    <div class="form-group">
      <label class="col-sm-4 control-label"  for="textinput">Card Holder's Name</label>
      <div class="col-sm-6">
        <input type="text" name="cardholdername" maxlength="70" placeholder="Card Holder Name" class="card-holder-name stripeform form-control">
      </div>
    </div>
    
    <!-- Card Number -->
    <div class="form-group">
      <label class="col-sm-4 control-label" for="textinput">Card Number</label>
      <div class="col-sm-6">
        <input type="text" id="cardnumber" maxlength="19" placeholder="Card Number" class="card-number stripeform form-control">
      </div>
    </div>
    
    <!-- Expiry-->
    <div class="form-group">
      <label class="col-sm-4 control-label" for="textinput">Card Expiry Date</label>
      <div class="col-sm-6">
        <div class="form-inline">
          <select name="select2" data-stripe="exp-month" class="card-expiry-month stripe-sensitive stripeform required form-control">
            <option value="01" selected="selected">01</option>
            <option value="02">02</option>
            <option value="03">03</option>
            <option value="04">04</option>
            <option value="05">05</option>
            <option value="06">06</option>
            <option value="07">07</option>
            <option value="08">08</option>
            <option value="09">09</option>
            <option value="10">10</option>
            <option value="11">11</option>
            <option value="12">12</option>
          </select>
          <span> / </span>
          <select name="select2" data-stripe="exp-year" class="card-expiry-year stripe-sensitive stripeform required form-control">
          </select>
          <script type="text/javascript">
            var select = $(".card-expiry-year"),
            year = new Date().getFullYear();
 
            for (var i = 0; i < 10; i++) {
                select.append($("<option value='"+(i + year)+"' "+(i === 0 ? "selected" : "")+">"+(i + year)+"</option>"))
            }
        </script> 
        </div>
      </div>
    </div>
    
    <!-- CVV -->
    <div class="form-group">
      <label class="col-sm-4 control-label" for="textinput">CVV/CVV2</label>
      <div class="col-sm-3">
        <input type="text" id="cvv" placeholder="CVV" maxlength="4" class="card-cvc form-control">
      </div>
    </div>


    
    <!-- Important notice -->
   
   
    <!--   <div class="panel-body">
        <p>Your card will be charged after submit.</p>
  
      </div> -->
 
    
    <!-- Submit -->
    <!-- <div class="control-group">
      <div class="controls">
        <center>
          <button class="btn btn-success" type="submit">Pay Now</button>
        </center>
      </div>
    </div> -->
  </fieldset>

                                  <!--  <button type="submit">Submit Payment</button> -->
</form> 
                  <br>
                   
                    <footer class="_grid cart-totals">
                      <div class="_column subtotal" id="clonetotalCtr">
                        <div class="cart-totals-key">Total</div>
                        <div class="cart-totals-value">$0.00</div>
                      </div>
                      <span class="stripe-logo"><img src="icons/outline.png"></span> 
                    </footer>
                    
                            </div>
                            
                        </div>

                        <div class="wizard-footer">
                            	<div class="pull-right">
                                    <input type='button' class='btn btn-next btn-fill btn-info btn-wd btn-sm' name='next' value='Next' />
                                    <input type='submit' class='btn btn-finish btn-fill btn-info btn-wd btn-sm' name='finish' value='Pay' />

                                </div>
                                <div class="pull-left">
                                    <input type='button' class='btn btn-previous btn-fill btn-default btn-wd btn-sm' name='previous' value='Previous' />
                                </div>
                                <!--  <div class="pull-left" style="margin-left:20px">
                                  <a href="testslider.html" type="button" class="btn btn-primary btn-sm btn-block">
                                   <span class="glyphicon glyphicon-chevron-left"></span> <span class=" exploreicon fa fa-globe" ></span> <span class="explore" > Continue Exploring </span>
                                  </a>
                                </div> -->
                                <div class="clearfix"></div>
                               
                        </div>
                    </form>
                </div>
            </div> <!-- wizard container -->
        </div>
        </div> <!-- row -->
    </div> <!--  big container -->

    <div class="footer">
        <div class="container">
            
        </div>
    </div>


</div>

</body>
<!-- 
 <script type="text/javascript">
    function copyDiv(){
      var firstDivContent = document.getElementById('mydiv1');
      var secondDivContent = document.getElementById('mydiv2');
      secondDivContent.innerHTML = firstDivContent.innerHTML;
    }
  </script>
   -->
  <script> 
  // $(document).on('ready') {
   var $conditionalInput = $('#billingaddress');
    var $checkme = $('input[id="check-me"]');

      $conditionalInput.hide();
      $checkme.on('click', function(){
          if ( !$(this).is(':checked') ) {
              $conditionalInput.show();
          }else {
              $conditionalInput.hide();
            }
      });
    
   </script>


  <!--Update Total in pay tab --> 



   <!-- Stripe javascript --> 

  <!--JS libaries --> 

    <script src="js/jquery-1.10.2.js" type="text/javascript"></script>
	<script src="js/bootstrap.min.js" type="text/javascript"></script>

	<!--   plugins 	 -->
	<script src="js/jquery.bootstrap.wizard.js" type="text/javascript"></script>

    <!--  More information about jquery.validate here: http://jqueryvalidation.org/	 -->
	<script src="js/jquery.validate.min.js"></script>

	<!--  methods for manipulating the wizard and the validation -->
	<script src="js/wizard.js"></script>
   <!--checkout products js -->
  

</html>
