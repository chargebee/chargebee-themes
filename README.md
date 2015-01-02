# ChargeBee Gallery Themes

The themes that are published in the ChargeBee theme gallery. These themes are created by ChargeBee designers. If you setout to build your own theme for your checkout pages, you can use any of these stock themes to start with.

You can also install these themes directly from the gallery and make changes via theme configurator from admin console.

## File structure

<pre>
theme_name
	|-- templates
		|-- checkout.html
		|-- thank_you.html
		|-- update_payment_method.html
		|-- iframe.html
		|-- login.html
		|-- portal.html
		|-- edit.html
		|-- error.html
	|-- conf
		|-- meta.json
		|-- presets.json
	|-- assets
		|-- css
			|-- theme.css
		|-- images
			|-- *.jpg,*.jpeg,*.gif,*.png,*.ico
</pre>
All the files specified above (except "thank_you.html") are mandatory to be present in the theme zip before upload.


## Overview
* Templates:
    * For each hosted page - Checkout page, update card page there must be a template in the Templates folder. For example, for the Checkout page, there must be a template in the Templates folder with the name checkout.html.
    * The required files in the template folder are:
        * checkout.html - The page inside which the Checkout page for both plan specific hosted pages & API based checkout pages are rendered.
		* thank_you.html - Page users will be forwarded to on completion of a successful checkout.
		* update_payment_method.html - The page which is used to render an option to update the payment method - (Credit Card payment, PayPal Express Checkout, Amazon Payments)
		* iframe.html - The page inside which the both the checkout & update card page is rendered when requesting the hosted pages for embedding inside iframe within your app.
		* login.html - The page which is used to render the customer portal login page along with options to request reset password and signup link.
		* portal.html - The customer portal page which is used to render the account details, billing address, card details, invoices, subscription details and shipping address for a customer.
		* edit.html - The customer portal page which is used to render the edit page for account details, billing address, card details and shipping address. This page is also used to render the page for making subscription changes as well as canceling the subscription.
		* error.html - The page which is rendered with the error message in case of errors while accessing the checkout page, update card page and customer portal pages.

* Assets:
    * This holds the stylesheets and images used in the css.
    * Currently all the styles should go under the file css/theme.css.

* Conf:
    * This holds the configuration options for the theme.
    * meta.json - Configure all the options that can be modified for this theme from admin console.
    * presets.json - Provide various flavours in colors, texts of the themes.

## Documentation

To build your own ChargeBee themes, see https://www.chargebee.com/docs/themes.html#building-your-own-chargebee-themes


## License

See the LICENSE file.

