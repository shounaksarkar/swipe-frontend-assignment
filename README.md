# Invoice Generator with Real-Time Currency Conversion

## Demo
<iframe width="560" height="315" src="https://www.youtube.com/video/mGWt7YCC9P4/" frameborder="0" allowfullscreen></iframe>


## New Feature: Currency Conversion

We've implemented a real-time currency conversion feature in our Invoice Generator application. This feature allows users to create and view invoices in different currencies, with automatic conversion of all monetary values.

### Key Features:

1. **Real-time Exchange Rates**: Utilizes the Free Currency API to fetch up-to-date exchange rates.
2. **Multiple Currency Support**: Supports conversion between various currencies including USD, EUR, GBP, JPY, CAD, AUD, SGD, CNY, and INR.
3. **Dynamic Conversion**: All monetary values (item prices, subtotal, tax amount, discount, and total) are converted in real-time when changing the invoice currency.
4. **Preserves Original Values**: The original values are stored, allowing for accurate conversion between any two currencies without cumulative rounding errors.

### How It Works:

1. When the component mounts, it fetches the latest exchange rates from the Free Currency API.
2. Users can select a different currency from the dropdown menu in the invoice form.
3. Upon selection, all monetary values in the invoice are converted to the new currency using the fetched exchange rates.
4. The conversion applies to individual item prices, subtotal, tax amount, discount amount, and the total invoice value.

### Usage:

1. Create a new invoice or open an existing one.
2. Locate the "Currency" dropdown in the invoice form.
3. Select your desired currency from the options provided.
4. Watch as all monetary values in the invoice update to reflect the new currency!
