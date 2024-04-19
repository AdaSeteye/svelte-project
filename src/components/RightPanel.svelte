<!-- RightPanel.svelte -->

<div class="premium-image-container">
  <img
    src="/images/premium-image.jpg"
    alt="Premium Reading"
    class="premium-image"
  />
</div>
<div class="right-panel-container">
  <div class="premium-details">
    <div class="premium-header">
      <h2 class="premium-title">Premium Reading</h2>
      <p class="premium-price">$00.00</p>
    </div>
    <div class="premium-features">
      <p class="feature">
        <span class="check-mark">&#x2713;</span>50+ page unique reading to fully
        understand your personality
      </p>
      <p class="feature">
        <span class="check-mark">&#x2713;</span> Integrating Astrology, Enneagram,
        Human Design, Spiral Dynamics and Numerology
      </p>
      <p class="feature">
        <span class="check-mark">&#x2713;</span> Lifetime access to your full report
      </p>
    </div>
    <div class="premium-totals">
      <div class="premium-subtotal">
        <p class="premium-text">Subtotal Total</p>
        <p class="premium-value">$00.00</p>
      </div>
      <div class="add-promotion-container">
        <a
          href="#"
          class="add-promotion"
          style="text-decoration: none; color: purple;">+ Add promotion code</a
        >
      </div>
      <div class="premium-total">
        <p class="premium-text">Your Total</p>
        <p class="premium-value">
          <span style="color: gray; font-size: 12px;">USD</span> $00.00
        </p>
      </div>
      <hr class="total-line" />
    </div>
  </div>
</div>

<style>
  .premium-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
  }

  .premium-title {
    font-size: 24px;
    font-weight: bold;
  }

  .premium-price {
    font-size: 20px;
    font-weight: bold;
    margin-left: 20px;
  }

  .premium-features {
    margin-bottom: 20px;
  }

  .feature {
    margin-bottom: 10px;
  }

  .check-mark {
    color: purple;
    font-weight: bold;
    margin-right: 10px;
  }

  .premium-totals {
    margin-top: 20px;
    padding-bottom: 0;
  }

  .premium-subtotal,
  .premium-total {
    display: flex;
    justify-content: space-between;
  }

  .premium-text {
    font-weight: bold;
    margin-right: 10px;
    margin-bottom: 0;
  }

  .premium-value {
    font-weight: bold;
    margin-bottom: 0;
  }

  .total-line {
    border: none;
    border-top: 2px solid black;
    margin-top: 10px;
  }

  .premium-image-container {
    position: relative;
    height: 120px;
    margin-bottom: -50px;
    z-index: 1;
    padding-top: 20px;
  }

  .premium-image {
    height: 95%;
    position: absolute;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
    width: 80%;
    z-index: 2;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
  }

  .right-panel-container {
    background-color: #f4f4f4;
    padding: 20px;
    padding-top: 60px;
    margin-top: -50px;
    position: relative;
    z-index: 0;
  }

  @media (max-width: 768px) {
    .premium-price,
    .premium-title {
      text-align: center;
    }

    .total-line {
      display: none;
    }

    .add-promotion-container {
      border: 1px solid black;
      padding: 3px;
      margin-top: 10px;
      border-radius: 5px;
    }
  }
</style>
