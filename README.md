Shopping Cart Price Rule Fix
============================

When creating a shopping cart price rule in Magento CE 1.9 and using 'Stop Further Rules Processing', the logic has been changed since 1.8 CE and is now flawed.  This flawed logic now stops rules being applied correcty with more than one product in the cart and doesn't consider 'Stop Further Rules Processing' at the item level.  This means that you get incorrect discount amounts applied as per the bug report here:

http://www.magentocommerce.com/bug-tracking/issue/index/id/67

This extension corrects the flawed logic and causes 'Stop Further Rules Processing' to be considered at the item level allowing rules to be processed for all items in the cart.
