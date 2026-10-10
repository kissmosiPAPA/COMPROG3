# COMPROG3
This is the Group 8 Project for COMPROG3 
The AniConnect application is an end-to-end e-commerce selling system developed in Java that bridges local farmers directly with consumers through a clean, programmatic graphical interface. Built using 
object-oriented principles, the platform employs an abstract base user model with role-based inheritance to separate farmer inventory controls from consumer marketplace views. When farmers publish 
produce listings, data is validated and recorded into a MySQL database via Data Access Object (DAO) design patterns. Consumers can authenticate, browse available catalog items, select quantities, and 
submit pre-orders through a guided checkout modal supporting multiple payment methods. The backend processes every checkout as an atomic transaction that verifies stock sufficiency, deducts inventory, 
registers payment records, and triggers real-time order status updates for farmers to fulfill without intermediary bottlenecks.
AniConnect Farmer Guide
What is AniConnect?
AniConnect is a desktop program that lets local farmers sell fresh produce directly to buyers.
You list what you have, with a price per kilo and how many kilos you can sell. Buyers see your
listing in the marketplace, place an order, and the order appears on your farmer screen. When
you deliver the produce, you mark the order as finished.
Prices are in pesos (₱). You sell by the kilo (kg).
How to run the system
1. Open the AniConnect project and run the program (AniConnectApp). The AniConnect -
Authentication Portal window appears first.
2. Log in or create an account, as described in the next section.
Navigation guide
After you log in as a farmer, the main window shows the following:
• Header (blue bar, top): the platform name, a welcome line showing your username and
role, and the red Logout button on the right.
• Farmer Portal (Add Produce) tab: the form for listing produce. It is the first tab, at the
top left.
• Marketplace Storefront (Buy Produce) tab: the same marketplace customers use. You
can also buy from other farmers here.
• Customer Purchase Reports table: under the form. Each row is one order for your
produce.
• Sequence Diagram Execution Log (right side): a running list of the steps the program
performs. A Clear Log button empties it.

Step-by-step technical procedure
Sign up and log in
To create an account:
1. Next to Account Role, choose Farmer.
2. Type a Username, a Password, and your Email (for Registration).
3. Click the green Create Account button. You are logged in right away.
To log in to an existing account:
1. Next to Account Role, choose Farmer.
2. Type your Username and Password.
3. Click the blue Login button.
Add your produce for sale
1. Make sure the Farmer Portal (Add Produce) tab is open.
2. In Produce Name, type what you are selling, for example Fresh Carrots.
3. In Price per Kg (₱), type the price of 1 kilo, for example 50.
4. In Quantity (Kg), type how many kilos you have, for example 100.
5. Click the green Submit Produce Listing button.
6. A message says Produce successfully saved! Click OK. Your produce now appears in the
marketplace.
Use numbers only for the price and the quantity. The Farmer Account box is filled in with your
username and cannot be changed.

See orders and mark them finished
Each row in the Customer Purchase Reports table is one order. The columns are:
• Order ID: the order number.
• Customer Name: who bought the produce.
• Produce Purchased: what they bought.
• Qty Bought (Kg): how many kilos they bought.
• Payment Amount (₱): how much the order costs.
• Stock Remaining (Kg): how many kilos you have left.
• Payment Method: Cash on Delivery or Credit/Debit Card.
• Status: every new order shows Paid, including Cash on Delivery orders. Check the Payment
Method column to see how the buyer is paying.
When an order is complete:
1. Give the produce to the buyer. If the Payment Method is Cash on Delivery, collect the
payment at the same time.
2. Click the green Mark a... button (Mark as Finished) in the Action column of that row.
3. A message says Order # ... marked as Finished! Click OK.
To refresh the table with new orders, log out and log in again. To log out, click the red Logout
button at the top right, then click Yes.

AniConnect Customer Guide
What is AniConnect?
AniConnect lets you buy fresh produce straight from local farmers. You browse what is for sale,
choose how many kilos you want, pay, and the order is recorded for the farmer. Prices are in
pesos (₱). You buy by the kilo (kg).
How to run the system
1. Open the AniConnect project and run the program (AniConnectApp). The AniConnect -
Authentication Portal window appears first.
2. Log in or create an account, as described in the next section.
Navigation guide
After you log in as a customer, the main window shows the marketplace:
• Header (blue bar, top): the platform name, a welcome line showing your username and
role, and the red Logout button on the right.
• Produce Marketplace Catalog: the table of produce for sale. Its columns are ID, Produce
Name, Price/Kg (₱), Available (Kg), and Farmer.
• Buy Selected Produce button (bottom right): starts an order for the row you selected.
• Sequence Diagram Execution Log (right side): a running list of the steps the program
performs. A Clear Log button empties it.
Step-by-step technical procedure
Sign up and log in

To create an account:
1. Next to Account Role, choose Consumer.
2. Type a Username, a Password, and your Email (for Registration).
3. Click the green Create Account button. You are logged in right away.
To log in to an existing account:
1. Next to Account Role, choose Consumer.
2. Type your Username and Password.
3. Click the blue Login button.
Buy produce
1. In the catalog table, click the produce you want. Its row is highlighted.
2. Click the orange Buy Selected Produce button at the bottom right. Double-clicking the
row also works.
3. In the Buy window, type the number of kilos in the Type Quantity (Kg) box. The Total
Amount updates as you type.
4. Click the green Proceed to Payment button.

Use whole numbers, such as 1, 2 or 5. The quantity must be more than zero and cannot be
more than the available stock.
Pay for your order
1. In the Choose Payment Method window, click Cash on Delivery to pay when the
produce arrives, or click Credit / Debit Card (Visa, MasterCard, JCB) to pay by card.
2. Click the green Confirm & Pay button at the bottom right. The amount shown on the
button is the total for your order.​
