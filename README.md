# Customer Churn and Returns Analysis Using SQL

## 1. Customer Churn Table

The `customer_churn` table contains customer information, including customer ID, tenure, preferred payment mode, order count, satisfaction score, and churn status. It helps analyze customer behavior and identify customers who have stopped using the service.

A new column named `ChurnStatus` was created to classify customers as **Churned** or **Active**. Another column, `ComplaintReceived`, was created to identify whether a customer made a complaint. These columns help analyze the relationship between customer complaints and churn.

## 2. Customer Returns Table

The `customer_returns` table stores information about product returns. It contains four columns: `ReturnID`, `CustomerID`, `ReturnDate`, and `RefundAmount`. Eight return records were inserted into the table.

This table helps track customer returns, return dates, and the amount refunded to customers. The `CustomerID` column connects return records to the corresponding customer information.

## 3. Joining the Two Tables

The `customer_churn` and `customer_returns` tables were joined using the `CustomerID` column with an `INNER JOIN`. This combines return details with customer information.

The query filters customers whose `ChurnStatus` is **Churned** and whose `ComplaintReceived` value is **Yes**. The result displays the return details and customer information for matching records.

## 4. Conclusion

This SQL analysis combines customer churn information with product return records. It helps identify customers who both complained and churned, while also showing their return and refund details. This information can help businesses understand customer dissatisfaction and improve customer retention.# Assignment-in-SQL
