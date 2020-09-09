# Refunds and Adjusting Payments

Occasionally, you may have to adjust the amount a customer pays for their order. Common scenarios include:

* Orders containing products with variable weights which are unknown at time of ordering \(such as [meat or large vegetables](../products-1/pricing-irregular-items-kg.md), sold priced by weight but as complete items\)
* A product ordered was not delivered by the producer.
* A customer contacts you to add extra items to their basket.
* One \(or more\) of the items ordered is not of the expected quality and you wish to compensate the customer.

  There are two main cases:

* The customer is due to _**pay for their produce on collection**_ and so no payment has been made in advance. In this case, you can adjust the customer's order, resend their order confirmation email, and the monies exchanged on the day of collection reflect the updated amount due.
* The _**order was paid for at the time it was placed**_ \(Stripe, PayPal, or bank transfer\). In this case there are three options:
  1. The balance is in CREDIT \(you owe the customer money\) and you wish to refund them.
  2. The balance is in CREDIT and you wish the customer to be able to use this credit on future purchases.
  3. The balance is in DEBT \(the customer owes you money\) 

## How to refund a Payment

### Refunding a Stripe Payment

_If the customer made the payment for their order to your business Stripe account, then you will be able to issue a full or partial refund from the OFN admin interface._

Make sure the order you wish to refund is marked as 'PAID':

![](../../.gitbook/assets/image%20%2817%29.png)

Adjust the order as necessary \(read [here](view-orders.md#editing-an-order) for how to edit an order or read more about [bulk order management](view-orders.md#bulk-order-management) for managing scenarios such as [product shortage](view-orders.md#example-1-you-have-a-stock-shortage-and-must-reduce-customer-order-quantities-for-a-certain-product) or [irregularly priced meat items](../products-1/pricing-irregular-items-kg.md).\)

You will then see the that there is CREDIT on the modified order. Select the 'tick' to the right of the order to issue a refund via Stripe:

![](../../.gitbook/assets/capture-du-2019-02-27-20-04-19.png)

The refund will be recorded on your business' Stripe account:

![](../../.gitbook/assets/stripecredit.png)

{% hint style="info" %}
Refunds take 5-10 days to appear on a customer's statement.
{% endhint %}

{% hint style="warning" %}
The fees charged by Stripe \(1.4% - 2.9% + 20p per transaction\) are not refunded to your business. They are charged based on the amount originally paid.  
It might, therefore, be more advantageous to offer the customer credit against their next \(or future\) order rather than issue a refund.
{% endhint %}

If an order has been totally cancelled you can issue a full refund \(if the customer paid by Stripe\) by [Edit order](view-orders.md#editing-an-order) -&gt; Payments and then selecting the 'cross' to the right hand side of the table:

![](../../.gitbook/assets/stripefullrefund.png)

### Refunding a PayPal payment

Automated partial or full refunds to customers who paid for their orders by PayPal are not supported on the OFN platform at the moment. You will need to visit your business PayPal account and issue a refund through their platform.  
This is a functionality we hope to add in the future.

### Refunding a Bank Transfer Payment

_A customer pays for their purchases by bank transfer or any other non-automated method \(ie any method except Stripe or PayPal\) and you recorded their payment. At a later date, it is necessary to_ [_edit their order_](view-orders.md#editing-an-order) _\(an item is not available or was supplied faulty\). After making this adjustment the over-payment made by the customer displays as credit against their order._  
To issue a refund by BACS you will need to do so through your business bank account.

## How to issue a customer Credit against their next order

An alternative to issuing a refund might be to manually deduct the customer's credit from their next order.

{% hint style="info" %}
Currently, as Shop or Hub manager, you would need to manually adjust the customers balance to take account of their credit. In the future we would like to automate this process. Please [contact us](https://www.openfoodnetwork.org/find-your-local-open-food-network/) if it is something which would be useful for your enterprise.
{% endhint %}

## How to bill a customer for additional funds

For example, a customer might ask to you add an additional item to an order they have already paid for, or, you might find after receipt of meat \([or other complete items priced by weight](../products-1/pricing-irregular-items-kg.md)\) that the total invoice is increased slightly.  
Any additional funds paid must be recorded manually. The customer will not be able to pay the excess by Stripe or PayPal through the OFN platform.

{% hint style="info" %}
If a customer wishes to add an item they forgot originally to their basket but pays by Stripe or PayPal then it might be simpler to ask them to create another order, rather than editing their existing order.
{% endhint %}

