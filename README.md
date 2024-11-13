# user_behavior_analysis
**Project Goals**

For a home grocery delivery company, it is necessary to analyze user behavior and assess the effectiveness of user acquisition channels.

- Calculate the number of unique users for February 2020
- Count the number of app installations in January 2020
- Segment users into cohorts by app installation date and calculate the 7-day conversion rate from installation to purchase
- Identify which paid marketing channel brought in the most new users
- Analyze the stage in the funnel where most registered clients drop off
- Determine which channels have the lowest conversion rate from acquisition to first purchase
- Identify the channel with the highest median first purchase amount
- Determine which paid acquisition channel (among advertising channels) has the highest ROMI (Return on Marketing Investment)

**Advertising Costs Data:**

- Yandex – 10,491,707 RUB
- Google – 10,534,878 RUB
- Facebook – 8,590,498 RUB
- Instagram – 8,561,626 RUB
- VK – 9,553,531 RUB

Data covers the period from January 1 to March 31, 2020, for users registered after January 1, 2020.

**Data Description**

- `date` – date of the event
- `event` – event type
  - `app_install` – app installation
  - `app_start` – open app
  - `register` – register
  - `search` – go to the product search page (catalog)
  - `open_item` – view a product
  - `choose_item` – add a product to cart
  - `tap_basket` – go to cart
  - `purchase` – purchase confirmation
- `gender` – user gender
- `os_name` – user platform
- `city` – user city
- `device_id` – user device ID
- `utm_source` – user acquisition channel
  - `yandex-direct` – Yandex Direct
  - `google_ads` – Google Ads
  - `vk_ads` – VK ads
  - `instagram_ads` – Instagram ads
  - `facebook_ads` – Facebook ads
  - `referral` – "Refer a friend" campaign
  - `'-'` – channel undefined, direct app download, or non-ad traffic
- `purchase_sum` – purchase amount (for `purchase` event)
