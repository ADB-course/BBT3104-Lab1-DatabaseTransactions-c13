[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/r-tQZu0l)
# BBT3104-Lab1of6-DatabaseTransactions


| **Key**                                                               | Value                                                                                                                                                                              |
|---------------|---------------------------------------------------------|
| **Group Name** C13                                                              | ? |
| **Semester Duration**                                                 | 19<sup>th</sup> August - 25<sup>th</sup> November 2024                                                                                                                       |

## Flowchart
![alt text](<WhatsApp Image 2024-09-17 at 11.49.53_a6afe673.jpg>)

## Pseudocode
START

SET TRANSACTION ISOLATION LEVEL

SELECT DATABASE

START TRANSACTION

GET OrderNumber

INSERT INTO Orders (OrderNumber)
INSERT INTO OrderItems (OrderId, ProductId, Quantity)

UPDATE Products SET Quantity = Quantity - QuantitySold WHERE ProductId = ProductId

SAVEPOINT beforeProduct

RECEIVE Payment

COMMIT

## Support for the Sales Departments' Report
They can calculate the unpaid balance. Using a a simple query we can subtract the amount that has already been paid from the total amount that should be paid therefore showing what specific amount is still unpaid for each individual order.
