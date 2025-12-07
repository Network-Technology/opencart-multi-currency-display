# Multi-Currency Display (EUR → BGN)

This is an OpenCart OCMOD extension that displays the BGN equivalent next to every formatted EUR price.  
If the store's default currency is **EUR**, the module automatically appends a secondary converted value in **BGN**.

Example output:

`€25.00 (49.00 лв.)`

---

## Features

- Shows BGN value next to all EUR-formatted prices  
- Works only when **default store currency = EUR**  
- Uses OpenCart’s native `convert()` method  
- Respects currency formatting, decimals, symbols  
- No admin settings — plug-and-play  
- Lightweight OCMOD modification of `system/library/cart/currency.php`

---

## Installation

1. Log into your OpenCart admin panel  
2. Go to **Extensions → Installer**  
3. Upload `install.xml`  
4. Go to **Extensions → Modifications** and click **Refresh**  
5. Clear theme/system cache if necessary

---

## Compatibility

- OpenCart **3.x**  
- PHP 7.x / 8.x  
- Compatible with Journal3 theme (tested)

---

## Files

- `install.xml` — OCMOD override implementing the secondary BGN display

---

## Example Logic

If:

- Default currency = **EUR**
- Formatted currency = **EUR**
- BGN currency exists in store settings

Then the module outputs:

`EUR price + (BGN converted price)`

---

## Author

**Network Technology**  
https://ntg.bg
