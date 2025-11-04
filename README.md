 

##  Tamara Payment Integration Guide for Front-End Teams

 

## 1. Implement Tamara Widget View (Promotional Messaging)

The Tamara widget view is crucial for informing customers about the "Pay in X" option and its benefits, usually displayed on the Product Details Page or, if unavailable, on the Payment Checkout Page.

| Aspect | Details |
| :--- | :--- |
| **Placement** | On the **Product Details Page** near the price, or on the **Payment Checkout Page**. |
| **Description** | Implement the widget as described in the Tamara documentation, including the required branding (logo, title, description). |
| **Interaction** | If the widget is tapped/clicked, it must open the specific informational link provided by Tamara, with all required query parameters (e.g., product price, currency). |


* **Widget Interaction Link (Example):** `https://cdn.tamara.co/widget-v2/tamara-widget.html?lang=ar&public_key=pk_123&country=SA&amount=100&inline_type=4`

* `lang`  according to current lang set to ar or en
* `public_key` (e.g., `pk_xyz`)
* `country` (e.g., `SA`)
* `amount` (e.g., `100` final total price)

 ### 🔗 Documentation Links

* [Tamara Widget](https://docs.tamara.co/docs/direct-widgets)

* [Tamara Summary Link](https://widget-docs.tamara.co/tamara-summary)
 
---
 
***

 ## 2. Present Tamara as a Payment Option

Once the customer is ready to select a payment method, Tamara must be clearly displayed and selectable.

| Aspect | Details |
| :--- | :--- |
| **Placement** | Within the list of **Payment Options** on the Checkout page. |
| **Branding** | Use the required Tamara **logo** and **title** (e.g., "Tamara"). |
| **Description** | Include the required **description** (e.g., "Monthly payments. Sharia compliant.") as specified in the docs. |

>❗ The Tamara session must be initiated and handled in the same tab on the website. No new tab or window should be opened when redirecting to Tabby's payment flow.

### 🔗 Required Documentation Links

* [Tamara's Branding and Payment Option Display Guidelines](https://docs.tamara.co/docs/tamara-widget-implementation-guidelines-saudi-arabia)
* [Tamara's Logo and Assets](https://cdn.tamara.co/merchant_docs/Tamara__Brand__Assets_v2.zip)


---


## 3. Collaboration with the Backend Team

Close collaboration is essential for smooth integration and comprehensive testing.


* [Testing Guide](https://docs.tamara.co/docs/testing-scenarios)
* [Testing Cards](https://docs.tamara.co/docs/testing-cards)
* [Go-Live Testing Checklist](https://docs.tamara.co/docs/testing-checklist)

---

## 4. Provide Testing Credentials For Tamara QA Team 

 After verifying that everything works correctly and all items in the test checklist are covered, each platform should provide one credential to assist the Tamara QA team in their testing process.
