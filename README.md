# FoodNeverArrives v1.4

<img width="2000" height="1125" alt="image" src="https://github.com/user-attachments/assets/4cd22b9c-d794-469e-b3b0-1dcd6856603e" />


> A mobile-first, one-file food-ordering showcase built as a comfort-oriented interactive web app.

FoodNeverArrives demonstrates a complete delivery-app experience without requiring a framework, package install, build command, backend, or external network request. The entire prototype ships inside one HTML file with inline CSS, JavaScript, embedded imagery, demo data, animation, and local persistence.

## Product overview

The app presents a polished fictional food-delivery flow inside a responsive phone-style shell. It supports onboarding, restaurant discovery, menu browsing, dish customization, checkout, simulated order tracking, coupons, reviews, order history, and account settings.

It is designed as a **showcase and interaction prototype**, not as a production marketplace. Payment details, GPS, notifications, restaurant availability, pricing, and delivery progress are simulated locally.

## Experience map
<img width="2000" height="1125" alt="image" src="https://github.com/user-attachments/assets/4901fff8-e287-4baf-b167-6b91a8455634" />


## Feature highlights

### Discovery and restaurant browsing

- location-aware top bar and search;
- cuisine/category filters and favorites;
- selectable delivery-speed modes;
- restaurant cards with ratings, reviews, fees, availability, and menu expansion;
- embedded food imagery and categorized dish sections.

### Dish customization and cart

- dish detail sheets;
- size, spice, topping, and quantity controls;
- price and calorie recalculation;
- one-restaurant-at-a-time cart behavior;
- item removal, subtotal, delivery fee, discounts, tips, and final total.

### Checkout and simulated delivery

- address and payment pickers;
- coupon claiming and application;
- simulated order placement;
- animated courier map, ETA, and delivery timeline;
- local push-style notifications and completion confetti.

### Retention and account surfaces

- order history and reorder;
- ratings and written reviews;
- favorites;
- saved addresses and payment methods;
- account settings and reset controls;
- local persistence between sessions.

## Data included in the prototype

| Item | Included |
|---|---:|
| Restaurants | 17 |
| Dishes | 393 |
| Coupons | 5 |
| Named JavaScript functions | 107 |
| External runtime dependencies | 0 |
| Build step | None |

## Technical profile

```text
Single HTML document
├─ responsive mobile shell
├─ inline design system and component CSS
├─ inline application state and navigation
├─ embedded WebP food imagery
├─ restaurant, menu, coupon, review, and tracking demo data
├─ localStorage persistence with in-memory fallback
└─ zero external scripts, fonts, APIs, or network requests
```

### Runtime characteristics

- Opens directly from `file://`.
- Also works through any basic static web server.
- Uses localStorage keys under the `fna_` prefix.
- Falls back to in-memory storage when localStorage is unavailable.
- Simulates delivery progress locally.
- Includes `prefers-reduced-motion` fallbacks.
- Uses responsive sizing for mobile and framed desktop presentation.

## Run the showcase

### Directly

Open:

```text
foodneverarrives_v1.4.html
```

in a modern browser.

### Through a local server

```bash
python -m http.server 8080
```

Then visit:

```text
http://localhost:8080/foodneverarrives_v1.4.html
```

## Persistence model

The prototype stores demo state locally, including setup completion, selected area, saved addresses and payment methods, favorites, claimed coupons, tip selection, order history, active tracking state, and reviews.

No data is transmitted to a server by the provided file.

## Accessibility and motion

The source includes responsive touch targets, safe-area handling, reduced-motion overrides for key animations, and conventional form controls. A production accessibility audit, keyboard-flow audit, localization pass, and screen-reader validation would still be required before release.

## Scope boundaries

This package does **not** provide real restaurant inventory, live courier GPS, payment processing, authentication, server-side order storage, fraud prevention, production security controls, live push infrastructure, or service-worker cache management.

## Full README overview

<img width="2000" height="1125" alt="image" src="https://github.com/user-attachments/assets/1789f8f2-d035-4a02-8009-e8af19967186" />


## Included source

```text
foodneverarrives_v1.4.html
```

The original single-file application is preserved unchanged inside this package.
