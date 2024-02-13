**Report on Star Schema Model using Financial Sample**

**Introduction:**
The purpose of this report is to present the development of a Star Schema model using the Financial Sample table as a data source. The Star Schema is a dimensional database model commonly used in data warehousing to facilitate data analysis. In this project, we created dimension tables and a fact table based on the provided requirements.

![fato2](/fato2.png)

**Methods:**
1. **Financials_origem (hidden mode – backup):** A copy of the original Financial Sample table was made for backup purposes.
2. **D_Products:** Relevant columns from the main table were selected to compose this dimension table, including product information and sales statistics.
3. **D_Products_Details:** Columns related to product details, such as sale price, units sold, and manufacturing prices, were selected.
4. **D_Discounts:** This table was created to store information about discounts applied to each product.
5. **D_Details:** An additional table was created to include additional product details not present in other tables.
6. **D_Calendar:** This table was generated using the `calendar()` function to provide a comprehensive calendar for temporal analysis.
7. **F_Sales:** The fact table containing sales metrics, such as units sold, sales price, profit, etc., was created.

**Results:**
The tables were created in CSV format as specified, including Financials_origem.csv, D_Products.csv, D_Products_Details.csv, D_Discounts.csv, D_Details.csv, D_Calendar.csv, and F_Sales.csv. These files were imported into Power BI for data modeling and analysis.

**Conclusion:**
The Star Schema model developed in this project facilitates the analysis of sales data from the Financial Sample. The dimension tables provide detailed contexts about products, discounts, and other relevant information, while the fact table offers key metrics for analysis. Integrating these tables into Power BI enables effective data visualization and valuable insights for decision-making.

**Case Study:**
A case study could involve analyzing product sales across different segments and countries over time using the developed Star Schema model. This can help a company identify sales trends, assess the effectiveness of applied discounts, and make strategic decisions to optimize sales performance across different regions and market segments.
