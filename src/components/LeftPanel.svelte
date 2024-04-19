<!-- LeftPanel.svelte -->
<script>
</script>

<div class="container">
  <h1 class="mt-4 title-text">Unlock Your Reading</h1>
  <p class="checkout-text">Express Checkout</p>
  <div class="payment-buttons row align-items-end justify-content-between">
    <div class="col-md-4 mb-2">
      <button class="btn btn-primary btn-block paypal">
        <img
          src="/images/paypal-logo.svg"
          alt="Paypal"
          class="logo"
          style="width: auto; height: 20px;"
        />
      </button>
    </div>
    <div class="col-md-4 mb-2">
      <button class="btn btn-primary btn-block apple-pay">
        <img
          src="/images/apple-pay-logo.svg"
          alt="Apple Pay"
          class="logo"
          style="width: auto; height: 20px;"
        />
      </button>
    </div>
    <div class="col-md-4 mb-2">
      <button class="btn btn-primary btn-block google-pay">
        <img
          src="/images/google-pay-logo.svg"
          alt="Google Pay"
          class="logo"
          style="width: auto; height: 20px;"
        />
      </button>
    </div>
  </div>
  <p class="or-pay-text">Or Pay With Card</p>
  <div class="card card-payment-form">
    <div class="card-body">
      <div class="input-group mb-2">
        <input type="text" class="form-control" placeholder="Card Number" />
        <div class="input-group-append">
          <button class="btn btn-outline-secondary visa-card" type="button"
          ></button>
          <button
            class="btn btn-outline-secondary mastercard-card"
            type="button"
          ></button>
          <button class="btn btn-outline-secondary amex-card" type="button"
          ></button>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6 mb-2">
          <input type="text" class="form-control" placeholder="MM/YY" />
        </div>
        <div class="col-md-6 mb-2">
          <input
            type="number"
            class="form-control"
            placeholder="CVV"
            min="0"
            max="9999"
          />
        </div>
      </div>
      <input
        type="text"
        class="form-control mb-2"
        placeholder="Full Name on Card"
      />
      <button class="btn btn-primary btn-block larger-pay-button">Pay</button>
    </div>
  </div>
</div>

<style>
  .title-text {
    color: purple;
    font-family: serif;
  }

  .payment-buttons {
    display: flex;
    justify-content: space-between;
    padding-bottom: 20px;
  }

  .payment-buttons .col-md-4 {
    flex: 1;
    max-width: calc(33.33% - 10px);
    margin-bottom: 20px;
  }

  .btn-primary {
    width: 100%;
    color: black;
    border-radius: 25px;
    background-color: white !important;
    border-color: #cccccc !important;
    padding: 5px 0;
    line-height: 1;
    text-align: center;
    overflow: hidden;
  }

  .payment-buttons .btn-primary img.logo {
    width: auto;
    height: 20px;
    margin-bottom: 5px;
  }

  @media (max-width: 768px) {
    .payment-buttons .col-md-4 {
      max-width: calc(50% - 10px);
    }

    .payment-buttons .col-md-4:not(:last-child) {
      margin-bottom: 0;
    }

    .payment-buttons .col-md-4:not(:first-child) {
      margin-left: -5px;
    }

    .payment-buttons .col-md-4:first-child {
      margin-right: -5px;
    }
  }

  .input-group-append {
    position: absolute;
    right: 10px;
    z-index: 1;
  }

  .input-group-append button {
    height: 80%;
  }

  .form-control {
    position: relative;
  }

  .btn-outline-secondary {
    border-radius: 0;
  }

  .logo {
    width: auto;
    height: 40px;
    margin-right: 5px;
  }

  .visa-card {
    background-image: url("/images/visa-logo.png");
    background-repeat: no-repeat;
    background-position: left center;
    background-size: auto 100%;
    padding-left: 40px;
  }

  .mastercard-card {
    background-image: url("/images/mastercard-logo.png");
    background-repeat: no-repeat;
    background-position: left center;
    background-size: auto 100%;
    padding-left: 40px;
  }

  .amex-card {
    background-image: url("/images/amex-logo.png");
    background-repeat: no-repeat;
    background-position: left center;
    background-size: auto 100%;
    padding-left: 40px;
  }

  .card-payment-form button.larger-pay-button {
    width: 60%;
    margin: 0 auto;
    border-radius: 10px;
    background-image: linear-gradient(to right, #300dad, #b74fd8);
  }

  .checkout-text,
  .or-pay-text {
    text-align: center;
    margin: 20px auto;
  }

  .checkout-text::before,
  .checkout-text::after,
  .or-pay-text::before,
  .or-pay-text::after {
    content: "";
    display: inline-block;
    width: 30px;
    border-top: 1px solid black;
    margin: 0 10px;
    vertical-align: middle;
  }

  .card-body {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>
