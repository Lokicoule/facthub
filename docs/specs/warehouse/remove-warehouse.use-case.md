# UC_WAREHOUSE_REMOVE_WAREHOUSE

A. Actors

- User

B. Description

User wants to delete one or many of his referential warehouse.

C. Basic Flow

1. Use case begins when Actor navigate to `/warehouses` or `/warehouses/view/:id`.
2. Actor has to click on remove button.
3. Actor has to be authenticated (cognito).
4. The warehouse(s) should be `ONLY` deleted from WAREHOUSE referential document.

- From `/warehouses` [BR_WAREHOUSE_REMOVE_WAREHOUSES](#brwarehouseremovewarehouses)
- From `/warehouses/view/:id` [BR_WAREHOUSE_REMOVE_WAREHOUSE](#brwarehouseremovewarehouse)

5. Use case ends when Actor is redirected to sign in page.

# Business Rules

## BR_WAREHOUSE_REMOVE_WAREHOUSE

- Remove warehouse from id
- Return warehouse data on success

## BR_WAREHOUSE_REMOVE_WAREHOUSES

- Remove warehouses from array
- Return true if all warehouses are removed else return false.
