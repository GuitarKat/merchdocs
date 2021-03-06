---
conditions: Default.EE-B2B
title: Category Permissions
---

Category access can be limited to specific customer groups, or restricted entirely. You can control the display of product prices, and determine which customer groups can add products to the cart, and specify the landing page.

{:.bs-callout-info}
Category Permissions has a global scope and when enabled, restricts access to each category according to its individual permissions. By default, Category Permissions is not enabled.

For example, if you sell only to wholesale customers, you can allow anyone to browse the catalog, but display prices and allow purchases only to those in the Wholesale customer group. In the following example, only logged in users have access to the “Collections” category. For guests, the “Collections” option doesn’t appear in the main menu.

![]({% link images/images/storefront-category-permissions-logged-in.png %}){: .zoom}
*Only Logged-In Users See “Collections” Category*

When enabled, a new “Category Permissions” section appears on the Category page that allows you to apply the needed access for each category. You can add multiple permission rules to each category for different websites and customer groups.

## Step 1: Configure Category Permissions

1. On the _Admin_ sidebar, go to **Stores** > _Settings_ > **Configuration**.

1. In the left panel, expand **Catalog** and choose **Catalog**.

1. Expand ![]({% link images/images/btn-expand.png %}){: .Inline} the **Category Permissions** section.

1. Set **Enable** to `Yes`.

    ![]({% link images/images-ee/config-catalog-catalog-category-permissions.png %}){: .zoom}
    *[Category Permissions]({% link configuration/catalog/catalog.md %})*

1. Set the **Allow Browsing Category** option, which applies to all categories in the [website]({% link stores/websites-stores-views.md %}).

    {:.procedure}
    For Specific Customer Groups

      To allow members of a specific customer group to browse through category products, do the following:

    - Set **Allow Browsing Category** to `Specified Customer Groups`.

    - In the **Customer Groups** box, select each group that is allowed to browse through products in the category. (For multiple options, hold down the Ctrl key, and click each group.)

        ![]({% link images/images-ee/category-permissions-allow-browsing-customer-groups.png %}){: .zoom}
        *Allow Browsing by Wholesale Customer Group*

    {:.procedure}
    Redirect to Landing Page

      Although the "Allow Browsing Category" setting applies to all categories in the website, you can configure a different Landing Page for each store view.

      To restrict access and redirect to a landing page, do the following:

    - Set **Allow Browsing Category** to `No, Redirect to Landing Page`.

    - Choose the **Landing Page** to which visitors will be redirected.

        ![]({% link images/images-ee/category-permissions-browse-category-landing-page.png %}){: .zoom}
        *Redirect to Home Page*

1. Set the **Display Product Prices** option, which applies to all categories in the [website]({% link stores/websites-stores-views.md %}).

    {:.procedure}
    For Specific Customer Groups

      To allow only members of specific customer groups to see the price of products in the category, do the following:

    - Set **Display Product Prices** to `Yes, for Specified Customer Groups`.

    - In the **Customer Groups** box, select each group that is allowed to see the price of products in the category. (For multiple options, hold down the Ctrl key, and click each group.)

        ![]({% link images/images-ee/category-permissions-price-customer-groups.png %}){: .zoom}
        *Only Wholesale Customer Group Can See Prices*

1. Set the **Allow Adding to Cart** option, which applies to all categories in the [website]({% link stores/websites-stores-views.md %}).

    {:.procedure}
    For Specific Customer Groups

      To allow only members of specific customer groups to put category products into the shopping cart, do the following:

    - Set **Allow Adding to Cart** to `Yes, for Specified Customer Groups`.

    - In the **Customer Groups** box, select each group that is allowed to add products from the category to the cart. (For multiple options, hold down the Ctrl key, and click each group.)

        ![]({% link images/images-ee/category-permissions-cart-customer-groups.png %}){: .zoom}
        *Only Wholesale Customer Group Can Put Product in Cart*

1. Set the **Disallow Catalog Search** option to prevent members of a specific customer group from using Catalog Search.

   The setting applies to all categories in the [website]({% link stores/websites-stores-views.md %}).

    {:.procedure}
    For Guest

    To allow only logged in customers to use Catalog Search, select `NOT LOGGED IN`.

    {:.procedure}
    For Specific Customer Groups

    In the **Disallow Catalog Search By** box, select each group to be prevented from using Category Search. (For multiple options, hold down the Ctrl key, and click each group.)

    ![]({% link images/images-ee/category-permissions-disallow-category-search.png %}){: .zoom}
    *Catalog Search Not Allowed for General Customer Group*

1. When complete, click <span class="btn">Save Config</span>.

1. When prompted to update the cache, click the **Cache Management** link in the system message and follow the instructions to refresh the cache.

## Step 2: Apply Category Permissions

1. On the _Admin_ sidebar, go to **Catalog** > **Categories**.

1. In the category tree, select the target category.

1. Expand ![]({% link images/images/btn-expand.png %}) **Category Permissions** on the page and do the following:

    - To create a permissions rule, click <span class="btn">New Permission</span>.

      ![]({% link images/images-ee/category-permissions-section-admin.png %}){: .zoom}
      *Category Permissions Section*

    - Choose the applicable **Website** and **Customer Group**.

    - Set the individual permissions as needed.

1. When complete, click <span class="btn">Save</span>.
