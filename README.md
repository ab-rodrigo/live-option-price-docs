# Live Option Price for OpenCart 3.x / 4.x

![OpenCart Version](https://img.shields.io/badge/OpenCart-4.x-blue?style=for-the-badge&logo=opencart)
![OpenCart Version](https://img.shields.io/badge/OpenCart-3.x-blue?style=for-the-badge&logo=opencart)
![License](https://img.shields.io/badge/License-GPL--3.0-green?style=for-the-badge)
![Languages](https://img.shields.io/badge/Languages-5-orange?style=for-the-badge)

[English](README.md) | [Português (BR)](README.pt-br.md) | [Português (PT)](README.pt-pt.md) | [Español](README.es-es.md) | [Français](README.fr-fr.md) | [Italiano](README.it-it.md)

![Live Option Price](./assets/images/social_preview.png)

[![Download](./assets/images/pt-br/download.png)](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)

---

## About

### Overview

<p align="center">
  <img src="./assets/images/demo-price-animation.gif" width="20%" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="./assets/images/demo-fade-effect.gif" width="20%" />
</p>

**Live Option Price** updates the product price in real-time as the customer selects their options, changes the quantity, or modifies other product-related information.

Without the module, the price displayed on the product page might remain unchanged until the customer completes an additional action. With **Live Option Price**, the values are automatically recalculated and presented directly on the product page.

The module uses natively configured values in OpenCart, including:

- Product price.
- Option prices.
- Discounts.
- Special price.
- Taxes.
- Product and option points, when enabled.
- Selected quantity.

The result is presented directly on the product page, providing the customer with an immediate view of the value corresponding to the chosen configuration.

### Compatibility

**Live Option Price** was developed to work on the following versions:

- **OpenCart 3.x**
- **OpenCart 4.x**

The administrative interface and operation may show slight visual differences between OpenCart versions, but the module's features and settings remain the same.

---

## Requirements

Ensure you have administrative permissions for:

- **Extension Installer**
- **Extensions / Modules**
- **Modifications**
- **Module Settings**

> **Important:** The installation must be performed using the official module file provided for your OpenCart version.

---

## Key Features

| Feature | Description |
| :--- | :--- |
| **Real-time price** | Automatically updates the price when the customer changes product options. |
| **Option prices** | Takes into account the markups and discounts defined in the product options. |
| **Quantity discounts** | Automatically considers quantity discounts configured in OpenCart. |
| **Special price** | Keeps the calculation compatible with the product's special price. |
| **Multiply by quantity** | Allows displaying the total value according to the selected quantity. |
| **Unit price** | Displays the price corresponding to one unit when the customer selects more than one unit. |
| **Discount badge** | Visually displays the discount percentage applied to the product. |
| **Taxes** | Updates price information related to taxes according to OpenCart's tax settings. |
| **Points** | Updates the points displayed for the product according to the selected options and quantity. |
| **Count animation** | Animates the numerical change of the price during updates. |
| **Fade effect** | Applies a visual transition during the price update. |

---

> **Important:** The module does not replace OpenCart's price settings. It uses the existing values in the product, options, discounts, and store tax settings to perform the calculation.

---

## Installation

Follow the flow below to install the extension:

1. **Download**: Get the official module directly from the [OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr).
2. **Upload**: In your store's admin panel, go to **Extensions > Installer**, click **Upload**, and select the downloaded file.
3. **Activation**: Locate the module in the extensions list and click the **Install** icon to activate it.

> **Technical Tip**: After activation, remember to go to **Extensions > Modifications** and click the **Refresh** button (blue icon) to clear the system cache.

---

## Accessing Settings

After installing the module:

1. Go to **Extensions > Extensions**.
2. Filter by **Modules**.
3. Locate **Live Option Price**.
4. Click **Edit**.

---

# Settings

![Settings](./assets/images/pt-br/docs-config-pt-br.png)

| Parameter | Function |
|---|---|
| **Multiply by quantity** | Determines whether the displayed price should consider the quantity selected by the customer.<br>**Important:** This setting specifically controls how the price is presented. The quantity continues to be considered by OpenCart in other applicable operations. |
| **Display discount badge** | Displays a badge with the discount percentage when the product has a promotional price or an applicable quantity discount.<br>**Important:** The percentage presented is calculated by the module based on the difference between the reference price and the applied discounted price. |
| **Display unit price** | Displays the value corresponding to one unit of the product when the selected quantity is greater than 1. The unit price is displayed when the calculation is set to consider the quantity and the selected quantity is more than one unit.<br>**Note:** This function only updates the information presented dynamically on the product page. OpenCart's point rules remain the source of the values used by the module. |
| **Calculate points** | When enabled, the module dynamically updates the points displayed on the product page according to the selected options. Option values may have their own point settings in OpenCart. |
| **Count animation** | Animates the numerical change of the price during updates. The numbers are animated during the transition instead of simply being replaced. This option is purely visual and can be used to provide a smoother transition between values. |
| **Fade effect** | Applies a visual opacity transition while the price is being updated. The effect helps visually indicate that the value is being updated after a change in options or quantity.<br>**Important:** When the **Count animation** is enabled, the module prioritizes the numerical price animation over the fade effect.|
| **Status** | Enables or disables the module. |

---

# Usage on the Product Page

Once the module is installed, active, and configured, no further action is required.

When accessing a product page, the price is calculated automatically.

---

# Theme Compatibility

The module updates the existing price elements on the product page and works with the standard OpenCart catalog structure.

Since third-party themes may modify the HTML structure of the product page, the visual presentation may vary depending on the theme used.

> **Important:** The calculation works independently of the theme's appearance. If a theme significantly alters the default product page structure, a specific adaptation for that theme might be required. If necessary, contact support.

---

# Troubleshooting

## The price does not update

Check:

1. If the module is installed.
2. If the module has **Status = Enabled**.
3. If the extension is enabled in OpenCart.
4. If the modifications were refreshed after installation.
5. If the OpenCart cache was cleared.
6. If the theme cache was cleared, when applicable.
7. If the product option has a price change configured.

---

## The option price does not display correctly

Check the option configuration directly in the product registration.

Confirm:

- Option value.
- Price prefix.
- Product associated with the option.
- Option selected on the product page.

**Live Option Price** uses the information registered in OpenCart to perform the calculation.

---

## The price does not change when altering the quantity

Check if: **Multiply by quantity** is enabled in the module settings. Also, confirm if the theme correctly uses the standard OpenCart quantity field.

---

## The quantity discount does not appear

Confirm if there is a discount rule registered for:

- the product;
- the customer group;
- the selected quantity;
- the current period.

Also check the priority of the discount rules configured in OpenCart.

---

## The discount badge does not appear

Confirm if: **Display discount badge** is enabled. The badge is only displayed when there is an applicable discount percentage.

---

## The unit price does not appear

Confirm if: **Display unit price** is enabled. It is also necessary that the calculation is considering the quantity and that the selected quantity is greater than one unit.

---

# Cache Clearance

After installing or updating the module, it is recommended to refresh the OpenCart caches.
Go to: **Extensions > Modifications** and click: **Refresh**. Also, clear the theme cache if this function is available in your installation.

> **Tip:** If a change made in the module does not appear immediately, the first diagnostic step should be clearing the caches.

---

## Uninstallation

Follow the steps below to perform a clean and safe uninstallation:

1. **Uninstall**: Go to **Extensions > Extensions**, filter by **Modules**, locate the module, and click **Uninstall**.
2. **Delete**: Locate the module in the installed extensions list and click the **Delete** icon.

> **What happens to the data?**: Uninstallation removes only the module settings and files.

---

# Support

If you encounter any issues during the installation or use of **Live Option Price**, please use the official extension page on the OpenCart Marketplace.

### Before Requesting Support

To facilitate diagnosis, please provide:

- OpenCart version.
- PHP version.
- Theme used.
- Live Option Price version.
- Description of the problem.
- Steps to reproduce the problem.

Whenever possible, include screenshots of the settings and the product page.

### Get Support

[Get support via the OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)

---

## Enjoying the module?

If **Live Option Price** is helping your store and improving your customers' experience, consider buying the author a coffee.

This helps maintain the development, maintenance, and future updates of the project.

[![Buy me a coffee](./assets/images/en-us/buy_me_a_coffee.png)](https://www.paypal.com/donate/?hosted_button_id=SPQH2B32XBJUW)

---

## License Information

This extension is licensed under the **GNU General Public License v3.0 (GPL-3.0)**.

- Use and modification of the software must be in accordance with the terms established by the GPL-3.0 license.
- Technical support and updates are provided exclusively to original buyers through the official OpenCart Marketplace.
- For full license details, see the **LICENSE** file distributed with the extension or visit the official [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html) page.

---

© 2026 **Rodrigoab** · [OpenCart Extensions](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)