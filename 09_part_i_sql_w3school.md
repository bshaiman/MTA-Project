# Challenge Set 9
## Part I: W3Schools SQL Lab 

*Introductory level SQL*

--

This challenge uses the [W3Schools SQL playground](http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all). Please add solutions to this markdown file and submit.

1. Which customers are from the UK?  
  
Thomas Hardy  
Victoria Ashworth  
Elizabeth Brown  
Ann Devon  
Helen Bennett  
Simon Crowther  
Hari Kumar  
   
2. What is the name of the customer who has the most orders?   
  
Ernst Handel  
  
3. Which supplier has the highest average product price?  
  
Aux joyeux ecclésiastiques  
  
4. How many different countries are all the customers from?  
  
91  
  
5. What category appears in the most orders?  
  
Dairy Products - 100  
  
6. What was the total cost for each order?   
  
A few too many orders to record here, but this is the query that will get the info:  
~~~~sql
SELECT OrderDetails.OrderID, SUM(OrderDetails.Quantity*Products.Price)   
FROM OrderDetails JOIN Products on OrderDetails.ProductID=Products.ProductID  
GROUP by OrderDetails.OrderID;  
~~~~ 
   
7. Which employee made the most sales (by total price)?  
  
Anne Dodsworth  
  
8. Which employees have BS degrees?  
  
Janet Leverling, Steven Buchanan.  
  
9. Which supplier of three or more products has the highest average product price?   

Plutzer Lebensmittelgroßmärkte AG  


