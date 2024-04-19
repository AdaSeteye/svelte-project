<!-- BottomPanel.svelte -->

<div class="bottom-panel-container">
  <div class="longer-texts">
    <div class="text-group">
      <span class="symbol">⟳</span>
      <p class="title">Lifetime Updates</p>
      <p class="text">
        We are constantly extending and improving all Type Reports. Any future
        content we add to it you will receive for free.
      </p>
    </div>
    <div class="text-group">
      <span class="symbol">↩</span>
      <p class="title">30 Days Money Back</p>
      <p class="text">
        We believe that this guide will help you you so much that we will give
        you a refund should you feel otherwise. No questions asked!
      </p>
    </div>
    <div class="text-group">
      <span class="symbol"> 🛡️</span>
      <p class="title">Safe & Secure</p>
      <p class="text">
        We don't record your payment details. They'll be sent over a secure,
        encrypted channel.
      </p>
    </div>
  </div>
  <div class="star-rating">
    <span class="star">★</span>
    <span class="star">★</span>
    <span class="star">★</span>
    <span class="star">★</span>
    <span class="star">★</span>
  </div>
  <p class="longer-text">
    "The Journey to Higher Self section outlines personal challenges I have
    recently discovered about myself."
    <span style="color: gray;">The Technical Expert | 1-5-3</span>
    <span style="color: purple;">Evan H.</span>
  </p>

  <!-- Copyright and terms/privacy -->
  <p class="copyright">
    © 2024 <a href="#" style="text-decoration: none; color:black;">Terms</a>
    <a href="#" style="text-decoration: none; color:black;">Privacy</a>
  </p>
</div>

<style>
  .bottom-panel-container {
    text-align: center;
    padding: 20px;
    position: relative;
  }

  .longer-texts {
    display: flex;
    justify-content: center;
    gap: 10px;
    margin-bottom: 20px;
  }

  .text-group {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .symbol {
    font-size: 24px;
    color: purple;
  }

  .title {
    color: purple;
    font-weight: bold;
    margin-top: 5px;
    margin-bottom: 5px;
    font-size: medium;
  }

  .text {
    margin: 0;
  }

  .star-rating {
    margin-bottom: 0;
  }

  .star {
    font-size: 24px;
    color: gold;
  }

  .longer-text {
    font-weight: normal;
    max-width: 50%;
    margin: 0 auto 150px;
    text-align: center;
    margin-bottom: 150px;
  }

  .copyright {
    position: absolute;
    bottom: 20px;
    right: 20px;
    text-align: right;
  }

  @media (max-width: 768px) {
    .copyright {
      text-align: center;
      margin-top: 20px;
      width: 100%;
    }

    .longer-texts {
      flex-direction: column;
      align-items: center;
      gap: 20px;
      margin-bottom: 20px;
    }
  }
</style>
