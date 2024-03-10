1. ## Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

---

- ### Answer :-
  **Product**: This table represents individual products. Each row in the "Product" table corresponds to a single product, identified uniquely by its id. Products have various attributes such as name, desc (description), SKU (Stock Keeping Unit), price, category_id, inventory_id, discount_id, created_at, modified_at, and deleted_at. The category_id column in the "Product" table serves as a foreign key referencing the id column of the "Product_Category" table, establishing a relationship between products and their respective categories.

**Product_Category**: This table represents categories or groups into which products are classified. Each row in the "Product_Category" table corresponds to a single category, identified uniquely by its id. Categories have attributes such as name, desc (description), created_at, modified_at, and deleted_at. The id column in the "Product_Category" table serves as the primary key, while the id column in the "Product" table serves as a foreign key referencing this primary key, creating a one-to-many relationship between categories and products. This means that each product belongs to one category, but a category can have multiple products associated with it.

2. ## How could you ensure that each product in the "Product" table has a valid category assigned to it?

---

- ### Answer :-

To ensure that each product in the Product table has a valid category assigned to it, you can utilize a foreign key constraint. In MySQL, you can define a foreign key constraint when creating the table, which ensures referential integrity between the "Product" table and the Product_Category table.

# End.