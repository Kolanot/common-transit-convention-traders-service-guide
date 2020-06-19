---
# Movements diagram

Version 0.1 3rd June 2020
***


This diagram shows the end-to-end process of transporting goods using the Common Transit Convention API. It shows at what stage in the process each message is sent, and who each message is sent to and from.

<img src="../figures/ctc-movements.svg"/>

1.a Trader at departure fills in and sends a declaration notification IE015.
1.b Office of departure receives declaration notification.
2.a Office of departure sends an acknowledgement of declaration notification 1E928.
2.b Trader at departure receives acknowledgement notification.
3.a Office of departure sends a Movement Reference Number (MRN) for the goods IE028.
3.b Trader at departure receives MRN.
4.a Office of departure sends notification releasing goods for transit IE029.
4.b Office of departure receives notification releasing goods for transit.
5.a Office of departure sends a notification to each Office in the countries the goods will pass through in transit. This does not use the CTC Traders API.
5.b Office(s) of transit receive(s) notification that goods will pass through their border.
6.a Office of departure sends a notification to confirm the goods have been released for transit to their Office. This does not use the CTC Traders API.
6.b Office of destination receives notification that goods are on route to their Office.
7.a Office(s) of Transit sends a notification to confirm goods have passed through their border. This does not use the CTC Traders API.
7.b Office of departure receives confirmation that goods have passed through planned borders on their journey.
8.a Trader at destination sends a notification to confirm that goods have arrived at their final destination IE007.
8.b Office of destination receives confirmation that goods have reached their final destination.
9.a Office of destination sends a notification to confirm goods have reached their final destination. This does not use the CTC Traders API.
9.b. Office of departure receives notification that goods have reached their final destination. 
10.a Office of destination sends notification that goods have passed or failed control checks.This does not use the CTC Traders API.
10.b Office of departure receives notification that goods have passed or failed control checks.
11.a Office of departure sends notification to release the goods IE025.
11.b Trader at destination receives a notification that goods have been released.
12.a Office of destination sends notification to confirm that the goods movement is complete IE045.  This confirms that all taxes have been paid.
12.b Trader at departure receives notification that the goods movement is complete. Goods are now released to be sold.
