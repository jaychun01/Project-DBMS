# Project-DBMS
Tony’s Liquor King
 
Final Report


 
                                         	
 
 
“The work presented here is ours and ours alone.  I have fully participated in this phase of the project and accept responsibility for the work presented here”.


Got the Munchies?

Working on this “Got the Munchies?” was a source of immense knowledge to our group. This project gave us great opportunities to learn how to develop database system and handle data set with MS access. 

We would like to appreciate to Tony for providing his business information and being nice to us. We would like to thank to each member in our group. Omar Benavides handled our technical problems all the time, Matthew Wagner organized and assigned the tasks to the group, Karandeep Gill contacted Tony to get business information about the store, and Jaekwan Chun who kept the group on track with deadlines and getting our meet up times coordinated. Without Tony’s help and each member’s contribution, the completion of this project would not have been completed.


##Executive Summary 

Being able to access, store and enter information is key to assisting running any form of businesses. Most companies have a database to a degree that allows them to process information about their products, employees and other important information. Tony’s liquor store is a small business that currently has a database for alcohol management, but is lacking one for snacks and other convenience products.
Tony’s liquor store offers a wide range of snacks including chips, candy bars drinks etc. In addition to the product numbers that these products have, Tony’s needs to document how much inventory they have for each item, the price, all the vendor information including name, address etc. As you can see, this can mount up to a great deal of number and information that can become confusing. With the current process being done with pen and paper you can easily see how complicated it can get to document all this information and errors are more common than you might think. This leads to inconsistency with price, inventory amount etc. Our solution is a database system within Microsoft access that has the ability to document all of Tony’s needs when it comes to entering the information he needs and how to retrieve information. We are using access because it is a database system that is cheap and available with his office package. Our layout consists of a very generic and basic layout as requested so it is very user friendly. We needed a system that just does what he needs without the headache of trying to figure out how to work it. 
Our implementation of Tony’s database consisted of gathering information about his user requirements for everything he wants the system to do. In addition we looked at existing order, invoice and vendor forms to get a layout that Tony is used to so when pulling up information and entering it in the database, it is consistent with the liquor database he currently uses. Once operational, it will take some time to enter in his existing information he currently keeps on pen and paper, but once that is complete it will be relatively seamless going forwards with new deliveries or new vendors he does business with. 
Overall, Tony’s database is relatively simple but effective database that will cater to his business’s needs for documenting and entering his information. Over time, it is very easy to incorporate his liquor database into the snack one to make a more concise and well rounded database. Tony’s database also includes the ability to add store number for the future incase he decides to open another location. This gives Tony the versatility to do what he needs with the consideration of future expansion if the opportunity arises. 

##Introduction
  
Tony’s Liquor King provides a convenient way of products of consumption. It’s a retail shop that stocks a range of everyday items such as groceries, snack foods, confectionery, toiletries, soft drinks, tobacco products, magazines and newspapers. Prices in such liquor/convenience stores are higher than supermarket prices because these stores order smaller quantities of inventory at higher per-unit prices from wholesalers. Besides that it is convenient verses a supermarket. It’s a quick stop saving customers time and fuel.
The goal of these convenience/liquor stores is to keep products that customer’s request for, which keeps customers coming back. Most of these places have regular customers that come in every day to a couple times per day. They expect the convenience store/liquor store near them to carry products that they need that way they don’t have to make their way to the supermarket to get those products. That can include the alcohol they request, snack items, tobacco items, etc… They make profit through this strategy. People look for convenience, they want everything accessible in the easiest and fastest way possible.
The current system separates an alcohol entity into the categories beer, liquor, and wine. Then, those categories are classified by product brand. They are divided by product name then flavors. Each product has data relating to sale price per unit, purchase price per unit, the number of on hand units, description, and reorder point. Kam feels that this system helps him operate the store efficiently in regards to managing alcohol sales. With this in mind, he wants a similar system for his consumer snacks. Given the higher quantities per shipment of snack products, Kam has had issues with staying on top of management of this store segment. 
As with any business, the first main concern in terms of implementing new software/hardware is cost. Luckily, we have found MS Access as a viable solution to Kam’s business needs. The software is low-cost, end-user friendly, and can be remotely accessed/maintained by a database admin and/or manager. User authentication passwords can be issued to help ensure data security as well as assignment of specific user roles/access rights for the database that Kam and his coworkers will be using. We can create different snack product entities for Kam and give them unique keys that are simple to remember and easy to update in tables. For example, we can create an entity for potato chips. Under potato chips, we can have barcode numbers as a primary key, vendor as a foreign key, and sales information as a secondary key. We can have Kam utilize a hand-scanner to add the different kinds of potato chips he carries into the Access database. We would set certain integrity constraints to ensure vital information doesn’t get left out. The other obstacle we foresee is hardware compatibility, but that shouldn’t be an issue. Ultimately, Kam could shift all his data into Access if he so pleases.

##System Requirements - the scope of database 

The scope of the database project is tracking snack items. Tony’s liquor store has long been tracking their drinks including beer, alcohol, and soda. Our goal is to build database system that will track snacks such as candy, chips, nuts, jerky, and donuts. In addition, the vendor's information is followed. Since our database system has to be connected to the system already existed, store entity is again defined and be basis of overall database system. Tony wants to expand his business eventually as well, store entity will help to supervise all stores. Store entity is including Store ID, store name, location, and person who is currently working. Item is identified with item id, and is including item name, price, type, and vendor id. Each vendor has vendor id, vendor name and contact number. Both item and vendor information is documented in invoice. Tony want to know about both order date and delivery date and amount of which he ordered. He stores snack items in the inventory and keep track of date he stocks items and number of items in inventory in which the data is calculated by subtract amount they order to number of the item sold. 

##Roadmap diagram

 
##Overall User Requirements.

There are two overall user requirements for Tony’s Liquor King. Currently, there is no system to track items or inventory; therefore, the two overall user requirements are focused on tracking items and inventory for snack foods. The first one is for Tony of Tony’s Liquor King to be able to track items based on different vendors. The second one is for Tony to be able to track the inventory of the items.
He wants to connect this database system with existing db. Story entity, hence, will be focus of overall db; it will contain store ID, store name, manager, city, state, zip. Inventory entity will contain Inventory_Code, Store_Id, Invoice_num, Item_ID, Inventory_date, Units-on_Hand. Invoice entity will include Invoice_num, Puchase_price, Units_ordered, Order_Date, Units_on_Hand, Cost, and Revenue. Item entity will contain Item_ID, Item_name, Sale_Price Item_category, and Vendor Id. Vendor entity will contain vendor id, Vendor_name, and Vendor_phone.

##ERD




##Relational schema:

STORE(Store_ID*, Store_name, Manager, City, State, ZIP)
INVENTORY(Inventory_code*, Store_ID, Invoice_num, Date_taken, Units_on_hand)
INVOICE(Invoice_num*, Item_ID, Purchase_price,Units_ordered, Order_date, Cost, Revenue)
ITEM(Item_id*, Item_name, Sale_price, Unit_sold Item_category, Vendor_ID)
VENDOR(Vendor_id*, Vendor_name, Vendor_phone)

##Individual user requirements

The individual user requirements include a way to add, modify or view each vendor, add, modify or view each snack item; as well as a way to view the reports. The individual requirements for vendor will need to be a location to search for through name, phone number, and vendor id. Then for item, there will need to be a location to search for name, item price, and type. For reports, there should be a location to go through different invoices as well as inventory reports. Then lastly, for invoice, there should be a location to search for invoice number, order date, and the delivery date.






##Nomalization

Table name: Store
Store (Store_ID*, Store_name, Manager, City, State, ZIP)




STORE_ID
STORE_NAME















Table name: Inventory
Inventory (Inventory_code*, Store_ID, Invoice_num, Item_id, Inventory_date, Units_on_hand)





INVENTORY_CODE
STORE_ID
INVENTORY_DATE








Table name: Invoice
Invoice (Invoice_num*, Item_ID, Purchase_price,Units_ordered, Order_date, Units_on_hand, Cost, Revenue)




INVOICE_NUM
ITEM_ID











Table name: Item
Item (Item_id*, Item_name, Sale_price, Item_category, Vendor_ID)




ITEM_ID
ITEM_NAME
VENDOR_ID





Table name: Vendor
Vendor (Vendor_id*, Vendor_name, Vendor_phone)


VENDOR_ID
VENDOR_NAME


Data dictionary
