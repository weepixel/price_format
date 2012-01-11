Price Format - an ExpressionEngine Plugin
=========================================

&copy; 2012 Wee Pixel [hello@weepixel.com](mailto:hello@weepixel.com)

Formats supplied price value with specified options and tax calculations.

Accepts six parameters:

* price="" (required, numeric value)
* decimals="" (optional, number of decimal points to show, defaults to 2)
* point="" (optional, character to use as point separator, defaults to .)
* thousands="" (optional, character to use as thousands separator or "none", defaults to ,)
* tax="" (optional, tax percentage - numeric value only, defaults to 0)
* show="" (optional, value can be "tax" to show just the tax amount or "total" to show the price including tax, defaults to "total")

Example usage:

	{exp:price_format price="1000"}
	(Output: 1,000.00)

	{exp:price_format price="1000" decimals="0"}
	(Output: 1,000)

	{exp:price_format price="1000" tax="20"}
	(Output: 1,200.00)

	{exp:price_format price="1000" tax="20" show="tax"}
	(Output: 200.00)