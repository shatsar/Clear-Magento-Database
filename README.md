Clear Magento Database
=====================
Simple SQL modular queries to clear Magento tables filled with fake data during the development phase.

HOWTO
-----
Connect to your Magento Database

     mysql> SET FOREIGN_KEY_CHECKS=0;

choose what to clear from your database full of data created during the development phase
for example if I have to clear searches i will launch

     mysql> source reset-searches.sql

At the end remember to launch:

     mysql> SET FOREIGN_KEY_CHECKS=1;

REFERENCE
---------
Original script taken from:
[Inchoo.net](http://inchoo.net/ecommerce/magento/delete-test-orders-in-magento/)
Improved with catalogsearch and divided in sub-queries.
