<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GrabDeals - Premium Coupons, Promo Codes & Deals Aggregator</title>
  <meta name="description" content="Save big with human-verified coupon codes, discount offers, and trending deals for Swiggy, Amazon, Myntra, Hostinger, Zomato, and more on GrabDeals.">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link rel="stylesheet" href="assets/css/style.css">
</head>
<body>

  <!-- Top Announcement Promo Bar -->
  <div class="promo-bar" id="promo-banner">
    ⚡ Monsoon loot is live! Save up to 80% on Hosting, Fashion, and Electronics. Verified codes updated 5 minutes ago!
  </div>

  <!-- Frosted Glass Navigation Header -->
  <header>
    <div class="header-container">
      <!-- Brand Logo -->
      <a href="index.html" class="brand-logo-container">
        <h1 class="brand-logo">
          🏷️ GrabDeals <span class="brand-tag">PRO</span>
        </h1>
      </a>

      <!-- Instant Search & Autosuggest -->
      <div class="search-wrapper">
        <div class="search-bar">
          <span class="search-icon"><i class="fa-solid fa-magnifying-glass"></i></span>
          <input type="text" id="search-input" placeholder="Search brands, deals, or categories..." autocomplete="off">
        </div>
        <div class="suggestions-dropdown" id="search-suggestions">
          <!-- Populated dynamically via JS -->
        </div>
      </div>

      <!-- Action Items -->
      <div class="header-actions">
        <!-- Theme Toggle -->
        <button class="theme-toggle-btn" id="theme-toggle-btn" title="Toggle Dark/Light Mode">
          <span id="theme-icon"><i class="fa-solid fa-moon"></i></span>
        </button>

        <!-- Bookmarks Trigger -->
        <button class="bookmarks-toggle-btn" id="bookmarks-btn" title="View Bookmarked Coupons">
          <i class="fa-solid fa-star"></i>
          <span class="bookmark-count-badge" id="bookmark-badge">0</span>
        </button>

        <!-- Submit Coupon Button -->
        <button class="submit-btn" id="header-submit-btn">
          <i class="fa-solid fa-plus"></i> Submit Coupon
        </button>
      </div>
    </div>
  </header>

  <!-- Main Content Body -->
  <main>
    
    <!-- Hero Slider / Carousel Banner -->
    <section class="hero-slider-section" id="hero-slider">
      <div class="slider-container">
        
        <!-- Slide 1: Swiggy -->
        <div class="slide active" style="background: linear-gradient(135deg, #FF6B00 0%, #1e1e24 100%)">
          <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=1200&q=80" alt="Delicious Food" class="slide-bg-img">
          <div class="slide-overlay"></div>
          <div class="slide-content">
            <span class="slide-tag">Trending Offer</span>
            <h2 class="slide-title">Craving Delicious Food? Save 50% on Swiggy!</h2>
            <p class="slide-desc">Order from your favorite restaurants and get flat 50% discount up to ₹100 on your first food order. Check active codes.</p>
            <button class="slide-cta" data-store="Swiggy">Grab Swiggy Coupons &rarr;</button>
          </div>
        </div>

        <!-- Slide 2: Myntra -->
        <div class="slide" style="background: linear-gradient(135deg, #E81A5F 0%, #1c1921 100%)">
          <img src="https://images.unsplash.com/photo-1483985988355-763728e1935b?auto=format&fit=crop&w=1200&q=80" alt="Fashion Trends" class="slide-bg-img">
          <div class="slide-overlay"></div>
          <div class="slide-content">
            <span class="slide-tag">Fashion Special</span>
            <h2 class="slide-title">End Of Reason Sale: Up to 70% Off on Myntra</h2>
            <p class="slide-desc">Revamp your wardrobe with top global fashion brands. Get extra savings with exclusive app coupon codes.</p>
            <button class="slide-cta" data-store="Myntra">Explore Fashion Deals &rarr;</button>
          </div>
        </div>

        <!-- Slide 3: Hostinger -->
        <div class="slide" style="background: linear-gradient(135deg, #673AB7 0%, #120b1f 100%)">
          <img src="https://images.unsplash.com/photo-1600132806370-bf17e65e942f?auto=format&fit=crop&w=1200&q=80" alt="Web Hosting Servers" class="slide-bg-img">
          <div class="slide-overlay"></div>
          <div class="slide-content">
            <span class="slide-tag">Web Hosting</span>
            <h2 class="slide-title">Get Online Today! Extra 10% Hostinger Savings</h2>
            <p class="slide-desc">Host your website with premium SSD speeds, free domains, and round-the-clock support. Limited period coupon code.</p>
            <button class="slide-cta" data-store="Hostinger">Get Hosting Coupon &rarr;</button>
          </div>
        </div>

      </div>

      <!-- Slider Indicators -->
      <div class="slider-dots" id="slider-dots-container">
        <span class="dot active" data-index="0"></span>
        <span class="dot" data-index="1"></span>
        <span class="dot" data-index="2"></span>
      </div>
    </section>

    <!-- Popular Stores Selection Grid -->
    <section>
      <div class="section-title-wrap">
        <h2 class="section-title">Shop by Top Verified Stores</h2>
      </div>
      <div class="stores-slider-container" id="stores-list-container">
        <!-- Rendered dynamically by JS -->
      </div>
    </section>

    <!-- Deals Of The Day Section -->
    <section class="deals-of-the-day-section">
      <div class="section-title-wrap">
        <div style="display: flex; align-items: baseline; gap: 15px; flex-wrap: wrap;">
          <h2 class="section-title">Deals Of The Day</h2>
          <a href="deals.html" style="color: var(--accent-color); font-size: 0.9rem; font-weight: 700; text-decoration: none; transition: opacity 0.2s;" onmouseover="this.style.opacity='0.8'" onmouseout="this.style.opacity='1'">View All Deals &rarr;</a>
        </div>
        <div class="deals-timer-badge">⏳ Offers expire in: <span id="deals-timer">23:59:59</span></div>
      </div>
      <div class="deals-of-the-day-grid" id="deals-of-the-day-container">
        <!-- Rendered dynamically via JS -->
      </div>
    </section>

    <!-- Popular Offers of the Day Section -->
    <section class="popular-offers-section">
      <div class="section-title-wrap">
        <div style="display: flex; align-items: baseline; gap: 15px; flex-wrap: wrap;">
          <h2 class="section-title">Popular Offers of the Day</h2>
          <span style="color: var(--text-muted); font-size: 0.85rem; font-weight: 700;">🔥 Top trending codes used today</span>
        </div>
        <div class="slider-nav-controls">
          <button class="slider-nav-btn" id="popular-prev-btn" title="Previous Offer"><i class="fa-solid fa-chevron-left"></i></button>
          <button class="slider-nav-btn" id="popular-next-btn" title="Next Offer"><i class="fa-solid fa-chevron-right"></i></button>
        </div>
      </div>
      <div class="popular-slider-viewport">
        <div class="popular-slider-track" id="popular-offers-container">
          <!-- Rendered dynamically via JS -->
        </div>
      </div>
    </section>

    <!-- Coupons & Deals Feed -->
    <section>
      <!-- Filter Toolbar -->
      <div class="coupons-toolbar">
        <!-- Category filters -->
        <div class="toolbar-left" id="categories-tabs-container">
          <!-- Rendered dynamically by JS -->
        </div>

        <!-- Coupon Type filters -->
        <div class="toolbar-right">
          <button class="filter-tab active" id="type-all">All Offers</button>
          <button class="filter-tab" id="type-codes">Promo Codes</button>
          <button class="filter-tab" id="type-deals">Deals</button>
          <button class="filter-tab" id="type-bookmarks">Bookmarked</button>
        </div>
      </div>

      <!-- Active Filter Status Title -->
      <div class="section-title-wrap" style="margin-bottom: 20px;">
        <h3 id="current-filter-title" style="font-size: 1.1rem; color: var(--text-muted); font-weight: 600;">
          Showing All Active Deals & Coupons
        </h3>
      </div>

      <!-- Coupon Grid Feed -->
      <div class="coupons-grid" id="coupons-grid-container">
        <!-- Rendered dynamically by JS -->
      </div>
    </section>

    <!-- GrabDeals Collections Section -->
    <section class="collections-section">
      <div class="section-title-wrap">
        <h2 class="section-title">GrabDeals Collections</h2>
      </div>
      <div class="collections-grid" id="collections-container">
        <!-- Rendered dynamically via JS -->
      </div>
    </section>

    <!-- Gamified Savings Calculator Widget -->
    <section class="savings-calculator-section">
      <h2 class="section-title">Calculate Your Yearly Savings</h2>
      <p style="color: var(--text-muted); font-size: 0.95rem; margin-top: 5px;">
        See how much money you can put back into your wallet using GrabDeals coupons on your daily spending!
      </p>

      <div class="calculator-layout">
        <!-- Sliders panel -->
        <div class="calc-sliders">
          <!-- Slider 1 -->
          <div class="slider-group">
            <div class="slider-header">
              <span>🍔 Food & Dining (Monthly spend)</span>
              <span id="val-food">₹0</span>
            </div>
            <input type="range" class="range-input" id="spend-food" min="0" max="25000" step="500" value="8000">
          </div>

          <!-- Slider 2 -->
          <div class="slider-group">
            <div class="slider-header">
              <span>👗 Fashion & Apparel (Monthly spend)</span>
              <span id="val-fashion">₹0</span>
            </div>
            <input type="range" class="range-input" id="spend-fashion" min="0" max="20000" step="500" value="4000">
          </div>

          <!-- Slider 3 -->
          <div class="slider-group">
            <div class="slider-header">
              <span>⚡ Electronics & Mobiles (Annual spend)</span>
              <span id="val-electronics">₹0</span>
            </div>
            <input type="range" class="range-input" id="spend-electronics" min="0" max="100000" step="1000" value="25000">
          </div>

          <!-- Slider 4 -->
          <div class="slider-group">
            <div class="slider-header">
              <span>✈️ Cabs & Travel (Monthly spend)</span>
              <span id="val-travel">₹0</span>
            </div>
            <input type="range" class="range-input" id="spend-travel" min="0" max="15000" step="500" value="3000">
          </div>
        </div>

        <!-- Math Display dashboard -->
        <div class="calc-display-card">
          <div class="calc-display-title">Estimated Annual Savings</div>
          <div class="calc-big-savings" id="calc-savings-amount">₹0</div>
          <p class="calc-subtext">
            Based on current deals, that's enough to pay for your weekend trip or 5 premium restaurant dinners!
          </p>
          <div class="calc-monthly-savings-wrap">
            <span>Estimated Monthly Savings</span>
            <span id="calc-monthly-savings">₹0</span>
          </div>
        </div>
      </div>
    </section>

  </main>

  <!-- Submit Coupon Slide Drawer -->
  <div class="slide-drawer" id="submit-drawer">
    <div class="drawer-header">
      <h2>Submit a Coupon Code</h2>
      <button class="drawer-close-btn" id="drawer-close-btn"><i class="fa-solid fa-xmark"></i></button>
    </div>
    
    <div class="drawer-body">
      <p style="color: var(--text-muted); font-size: 0.85rem; margin-bottom: 20px;">
        Share working codes you've found and help others save money. Submitted coupons appear instantly in the feed!
      </p>

      <form class="submit-form" id="submit-coupon-form">
        <!-- Store Select -->
        <div class="form-group">
          <label for="form-store">Select Store *</label>
          <select id="form-store" required>
            <option value="Swiggy">Swiggy</option>
            <option value="Amazon">Amazon</option>
            <option value="Flipkart">Flipkart</option>
            <option value="Myntra">Myntra</option>
            <option value="Hostinger">Hostinger</option>
            <option value="Zomato">Zomato</option>
            <option value="Dominos">Domino's</option>
            <option value="OnePlus">OnePlus</option>
          </select>
        </div>

        <!-- Discount -->
        <div class="form-group">
          <label for="form-discount">Discount Label (e.g. 50% OFF, Flat ₹100 Off) *</label>
          <input type="text" id="form-discount" placeholder="e.g. 60% OFF" required>
        </div>

        <!-- Title -->
        <div class="form-group">
          <label for="form-title">Offer Title *</label>
          <input type="text" id="form-title" placeholder="e.g. Up to 60% Off on Pizzas" required>
        </div>

        <!-- Description -->
        <div class="form-group">
          <label for="form-desc">Offer Description *</label>
          <textarea id="form-desc" rows="3" placeholder="Describe the deal terms and conditions..." required></textarea>
        </div>

        <!-- Code (Optional) -->
        <div class="form-group">
          <label for="form-code">Coupon Code (Leave blank for deals without code)</label>
          <input type="text" id="form-code" placeholder="e.g. LOOT60">
        </div>

        <div class="form-row">
          <!-- Category -->
          <div class="form-group">
            <label for="form-category">Category *</label>
            <select id="form-category" required>
              <option value="food">Food & Dining</option>
              <option value="fashion">Fashion & Apparel</option>
              <option value="electronics">Electronics & Mobiles</option>
              <option value="travel">Travel & Flights</option>
              <option value="hosting">Hosting & Domains</option>
            </select>
          </div>

          <!-- Expiry -->
          <div class="form-group">
            <label for="form-expiry">Expiry Date</label>
            <input type="date" id="form-expiry">
          </div>
        </div>

        <button type="submit" class="form-submit-btn">Submit Coupon &rarr;</button>
      </form>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    <div class="footer-container">
      <div class="footer-brand">
        <h3>🏷️ GrabDeals</h3>
        <p style="margin-top: 10px;">Your ultimate destination for verified coupons, promo codes, and daily deals. We help smart shoppers save millions every single month.</p>
      </div>

      <div class="footer-links-col">
        <h4>Top Categories</h4>
        <ul>
          <li><a href="#" class="foot-cat-link" data-cat="food">🍔 Food & Dining</a></li>
          <li><a href="#" class="foot-cat-link" data-cat="fashion">👗 Fashion & Apparel</a></li>
          <li><a href="#" class="foot-cat-link" data-cat="electronics">⚡ Electronics & Mobiles</a></li>
          <li><a href="#" class="foot-cat-link" data-cat="travel">✈️ Travel & Flights</a></li>
        </ul>
      </div>

      <div class="footer-links-col">
        <h4>Popular Stores</h4>
        <ul>
          <li><a href="#" class="foot-store-link" data-store="Swiggy">🍊 Swiggy</a></li>
          <li><a href="#" class="foot-store-link" data-store="Amazon">🛒 Amazon</a></li>
          <li><a href="#" class="foot-store-link" data-store="Myntra">👠 Myntra</a></li>
          <li><a href="#" class="foot-store-link" data-store="Hostinger">💻 Hostinger</a></li>
        </ul>
      </div>

      <div class="footer-newsletter">
        <h4>Stay Updated!</h4>
        <p>Subscribe to our weekly newsletter and never miss premium verified coupons again.</p>
        <form class="newsletter-form" id="newsletter-form">
          <input type="email" placeholder="Enter your email..." required>
          <button type="submit">Subscribe</button>
        </form>
      </div>
    </div>

    <div class="footer-bottom">
      <div>&copy; 2026 GrabDeals. Designed for premium savings. All rights reserved.</div>
      <div style="display: flex; gap: 20px;">
        <a href="#" style="color: var(--text-muted); text-decoration: none;">Privacy Policy</a>
        <a href="#" style="color: var(--text-muted); text-decoration: none;">Terms of Service</a>
      </div>
    </div>
  </footer>

  <!-- App logic entry -->
  <script type="module" src="assets/js/app.js"></script>
</body>
</html>
