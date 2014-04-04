# ChargeBee Gallery Themes

The themes that are published in the ChargeBee theme gallery. These themes are created by ChargeBee designers. If you setout to build your own theme for your checkout pages, you can use any of these stock themes to start with.

You can also install these themes directly from the gallery and make changes via theme configurator from admin console.

## File structure

<pre>
theme name
	|-- templates
		|-- checkout.html
		|-- update_card.html
		|-- iframe.html
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
All the files specified above are mandatory to be present in the theme zip before upload.


## Overview
* Templates:
    * For each hosted page - Checkout page, update card page there must be a template in the Templates folder. For example, for the Checkout page, there must be a template in the Templates folder with the name checkout.html.
    * The required files in the template folder are:
        * checkout.html - The page inside which the Checkout page for both plan specific hosted pages & api based checkout pages are rendered
        * update_card.html - The page inside which the Update card page is rendered.
        * iframe.html - The page inside which the both the checkout & update card page is rendered when requesting the hosted pages for embedding inside iframe within your app.
        * error.html - The page which is rendered with the error message in case of errors.

* Assets:
    * This holds the stylesheets and images used in the css.
    * Currently all the styles should go under the file css/theme.css.

* Conf:
    * This holds the configuration options for the theme.
    * meta.json - Configure all the options that can be modified for this theme from admin console
    * presets.json - Provide various flavours in colors, texts of the themes.

## Documentation

To build your own ChargeBee themes, see https://www.chargebee.com/docs/themes.html#building-your-own-chargebee-themes


## License

See the LICENSE file.

