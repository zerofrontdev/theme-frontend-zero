# Changelog: zerofront/theme-frontend-zero

## 1.3.6

- Google reCAPTCHA works on every Magento form the theme renders: sign-in, registration, forgot password, contact, newsletter, reviews and the Zero checkout sign-in (theme templates for `Magento_ReCaptchaFrontendUi`, `Magento_ReCaptchaCustomer`, `Magento_ReCaptchaNewsletter`).
- A Price on Request product (Zero Quote Request) shows "Request a Price" instead of Add to Cart on every product card: category and search lists, related, up-sell and cross-sell, catalog and recently viewed or compared widgets, compare and the wish list.
- On such a product's page only the quantity and Add to Cart are replaced by the request form; Add to Wish List and Compare stay (`product/view/addtocart.phtml` renders `main_control_html` when a module sets it).
- The wish list's "Add All to Cart" says which items it leaves out, and the Recently Ordered sidebar offers "Request a Price" for them instead of a checkbox.
- A configurable product with custom options shows the chosen variant's price plus the options (the options were added to the parent's price), and the bundle summary formats amounts in the store's currency instead of `$`.
- The category sidebar's Compare Products and My Wish List load with the session bootstrap, without a request of their own.
- Swatch and layered navigation templates read only plain values from the request, so an address like `?color[]=1` no longer causes a 500.

Earlier releases (1.3.5 and before): see the Git tags.
