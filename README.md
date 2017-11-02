# PadLoper Coupon Code Module

ProcessWire module that adds the possibility to add coupon codes.

If you've never heard of PadLoper - it’s an easy and flexible eCommerce platform, built on the ProcessWire framework. [Find out more about Padloper](https://padloper.pw/) or [just go for it](https://padloper.pw/buy/).

## Usage

Just install the module, no configuration is needed.  

The module adds a template called `pad_couponcode` and appends it as product template (**PadCart** module settings).
It creates the following fields and adds them to the template: `pad_couponcode`, `pad_limit`, `pad_valid_from`, `pad_valid_until` and `pad_price`.
Furthermore it adds the `pad_couponcode` field to the `padorder` template in the last position. If you want to change the position, open **PadOrder** module settings and drag it onto the desired position.

## Add a coupon code

Create a new page, assign template `pad_couponcode` and fill out all the appropriate fields. 

- **title** – will be displayed as title in the shopping cart
- **coupon code** – this field is prefilled with a generated coupon code, of course, it is also possible to manually change it to something else
- **one-time use** – activate the checkbox if the coupon code may be used only once
- **price** – the value must be preceded by a minus (-) sign
- **valid from** – the date from which the card is valid
- **valid until** – the date up to which the card is valid

## Notes

1. Only one coupon code can be redeemed per order.
2. If one-time use is enabled, the coupon code will be disabled after usage.
3. A coupon code is not redeemable against the shipping costs.
4. A coupon code is only redeemable during a specified period.
5. Should the value of the coupon code be higher than the total price of the goods purchased, the remaining value of the coupon code will be lost.

## Restrictions

- no minimum total value of purchase adjustable
- the coupon code is not applicable to shipping costs
