![Module Preview](https://raw.githubusercontent.com/Network-Technology/opencart-multi-currency-display/main/788be9a9-cffc-4b14-93d1-a8ac06caeeba_20251205_133137_c1d84f.png)

# Multi-Currency Display (EUR → BGN)

This is an OpenCart OCMOD extension that displays the BGN equivalent next to every formatted EUR price.  
If the store's default currency is **EUR**, the module automatically appends a secondary converted value in **BGN**.

Example output:

`€25.00 (49.00 лв.)`


## Licensing & Availability (Paid Extension)

This is a **paid commercial extension** developed by Network Technology.  
The full OCMOD package is available only to customers with a valid purchase.

💰 **Module price: 50 EUR**

For licensing or inquiries: **office@ntg.bg**  
Official website: https://ntg.bg  

**Product articles:**  
- 🇧🇬 Bulgarian: https://ntg.bg/blog/opencart-eur-bgn  
- 🇬🇧 English: https://ntg.bg/en/blog/opencart-eur-bgn


## Features

- Shows BGN value next to all EUR-formatted prices  
- Works only when **default store currency = EUR**  
- Uses OpenCart’s native `convert()` method  
- Respects currency formatting, decimals, symbols  
- No admin settings — plug-and-play  
- Lightweight OCMOD modification of `system/library/cart/currency.php`


## Installation

> ⚠️ Full installation package is provided only to licensed users.

1. Log into your OpenCart admin panel  
2. Go to **Extensions → Installer**  
3. Upload the provided `.ocmod.zip` package  
4. Go to **Extensions → Modifications** and click **Refresh**  
5. Clear theme/system cache if necessary


## Compatibility

- OpenCart **3.x**  
- PHP 7.x / 8.x  
- Compatible with Journal3 theme (tested)


## Files

- `install.xml` — OCMOD override implementing the secondary BGN display


## Example Logic

If:

- Default currency = **EUR**
- Formatted currency = **EUR**
- BGN currency exists in store settings

Then the module outputs:

`EUR price + (BGN converted price)`


## Author

**Network Technology**  
https://ntg.bg
