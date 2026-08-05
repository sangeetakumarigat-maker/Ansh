<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Local Shop — Fresh Finds, Best Prices</title>

<!-- Google Fonts: Fraunces (display) + Inter (body/UI) -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,500;0,9..144,600;0,9..144,700;1,9..144,500&family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<link rel="stylesheet" href="style.css">
</head>
<body>

<!-- ============ HEADER / NAV ============ -->
<header class="site-header" id="top">
  <div class="header-inner">
    <span class="brand-mark">The Local Shop</span>
    <nav class="header-nav">
      <a href="#products">Products</a>
      <a href="#order">Order</a>
    </nav>
  </div>
</header>

<!-- ============ HERO SECTION ============ -->
<section class="hero" style="background-image: linear-gradient(180deg, rgba(31,77,58,0.15) 0%, rgba(20,32,26,0.75) 100%), url('https://i.ibb.co/bR8R0BvV/IMG-0895.jpg');">
  <div class="hero-content">
    <p class="hero-eyebrow">Your neighbourhood store, online</p>
    <h1 class="hero-title">The Local Shop</h1>
    <p class="hero-tagline">"Fresh Finds, Best Prices"</p>
    <a href="#products" class="btn btn-primary hero-cta" id="shopNowBtn">Shop Now ↓</a>
  </div>
  <div class="awning-divider" aria-hidden="true"></div>
</section>

<!-- ============ PRODUCTS SECTION ============ -->
<section class="products-section" id="products">
  <div class="section-heading">
    <span class="eyebrow">On the shelf today</span>
    <h2>Fresh Picks For You</h2>
    <p class="section-sub">Hand-picked essentials, restocked daily. Slide through and add your favourites to the basket.</p>
  </div>

  <div class="carousel-wrap">
    <button class="carousel-arrow carousel-arrow--left" id="scrollLeft" aria-label="Scroll left">&#8249;</button>
    <div class="carousel" id="productCarousel"><!-- product cards injected by JS --></div>
    <button class="carousel-arrow carousel-arrow--right" id="scrollRight" aria-label="Scroll right">&#8250;</button>
  </div>
</section>

<div class="awning-divider awning-divider--flip" aria-hidden="true"></div>

<!-- ============ ORDER / CHECKOUT SECTION ============ -->
<section class="order-section" id="order">
  <div class="section-heading">
    <span class="eyebrow">Almost there</span>
    <h2>Place Your Order</h2>
    <p class="section-sub">Fill in your details below — we'll get your basket ready for delivery.</p>
  </div>

  <div class="order-grid">
    <!-- Order form -->
    <form class="order-form" id="orderForm">
      <label for="custName">Full Name</label>
      <input type="text" id="custName" name="custName" placeholder="e.g. Sangeeta Kumari" required>

      <label for="custPhone">Phone Number</label>
      <input type="tel" id="custPhone" name="custPhone" placeholder="e.g. 98765 43210" required>

      <label for="custAddress">Delivery Address</label>
      <textarea id="custAddress" name="custAddress" rows="3" placeholder="House no., street, area, city, pincode" required></textarea>

      <label for="custNotes">Notes <span class="optional-tag">(optional)</span></label>
      <textarea id="custNotes" name="custNotes" rows="2" placeholder="Any delivery instructions or preferences..."></textarea>
    </form>

    <!-- Order summary -->
    <div class="order-summary">
      <h3>Order Summary</h3>
      <div class="order-summary-items" id="orderSummaryItems">
        <p class="empty-note">Your basket is empty. Add some products above!</p>
      </div>
      <div class="order-summary-total">
        <span>Total</span>
        <span id="orderSummaryTotal">₹0</span>
      </div>
      <button type="submit" form="orderForm" class="btn btn-primary btn-place-order" id="placeOrderBtn">Place Order via Email</button>
      <p class="order-hint">This opens your email app with your order pre-filled, addressed to the shop.</p>
    </div>
  </div>
</section>

<!-- ============ FOOTER ============ -->
<footer class="site-footer">
  <p>&copy; <span id="year"></span> The Local Shop — Fresh Finds, Best Prices</p>
  <p class="footer-sub">Reach us at <a href="mailto:sangeetakumarigat@gmail.com">sangeetakumarigat@gmail.com</a></p>
</footer>

<!-- ============ FLOATING CART BUTTON ============ -->
<button class="fab cart-fab" id="cartFab" aria-label="Open cart">
  🛒
  <span class="cart-badge" id="cartBadge">0</span>
</button>

<!-- ============ FLOATING WHATSAPP BUTTON ============ -->
<a class="fab whatsapp-fab" id="whatsappFab" href="https://wa.me/9999999999" target="_blank" rel="noopener" aria-label="Chat on WhatsApp">
  <svg viewBox="0 0 32 32" width="28" height="28" fill="currentColor" aria-hidden="true">
    <path d="M16.001 3C9.373 3 4 8.373 4 15c0 2.386.7 4.61 1.912 6.48L4 29l7.72-1.877A11.93 11.93 0 0 0 16.001 27C22.63 27 28 21.627 28 15S22.63 3 16.001 3Zm0 21.818a9.77 9.77 0 0 1-4.983-1.363l-.357-.213-4.583 1.114 1.14-4.464-.234-.366A9.78 9.78 0 0 1 6.182 15c0-5.42 4.4-9.818 9.819-9.818S25.818 9.58 25.818 15 21.42 24.818 16.001 24.818Zm5.361-7.34c-.294-.147-1.74-.858-2.01-.956-.27-.098-.467-.147-.664.147-.196.294-.762.956-.934 1.152-.172.196-.343.221-.637.074-.294-.147-1.242-.458-2.366-1.46-.874-.78-1.464-1.744-1.636-2.038-.172-.294-.018-.453.129-.6.132-.132.294-.343.44-.514.148-.172.197-.294.295-.49.098-.196.049-.368-.025-.515-.074-.147-.664-1.6-.91-2.192-.24-.577-.484-.499-.664-.508l-.565-.01c-.196 0-.514.074-.784.368-.27.294-1.03 1.006-1.03 2.454 0 1.448 1.055 2.846 1.202 3.043.147.196 2.077 3.17 5.032 4.444.703.303 1.251.484 1.679.62.706.225 1.348.193 1.856.117.566-.085 1.74-.712 1.985-1.4.245-.688.245-1.278.172-1.4-.074-.123-.27-.196-.564-.343Z"/>
  </svg>
</a>

<!-- ============ CART DRAWER ============ -->
<div class="cart-overlay" id="cartOverlay"></div>
<aside class="cart-drawer" id="cartDrawer" aria-label="Shopping cart">
  <div class="cart-drawer-header">
    <h3>Your Basket</h3>
    <button class="cart-close" id="cartClose" aria-label="Close cart">&times;</button>
  </div>
  <div class="cart-drawer-items" id="cartDrawerItems">
    <p class="empty-note">Your basket is empty.</p>
  </div>
  <div class="cart-drawer-footer">
    <div class="cart-drawer-total">
      <span>Total</span>
      <span id="cartDrawerTotal">₹0</span>
    </div>
    <button class="btn btn-outline" id="clearCartBtn">Clear Cart</button>
    <a href="#order" class="btn btn-primary" id="goToOrderBtn">Go to Checkout</a>
  </div>
</aside>

<script src="script.js"></script>
</body>
</html>
