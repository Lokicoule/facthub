# UC_PRODUCT_REMOVE_PRODUCT

A. Actors

- User

B. Description

User wants to delete one or many of his referential product.

C. Basic Flow

1. Use case begins when Actor navigate to `/products` or `/products/view/:id`.
2. Actor has to click on remove button.
3. Actor has to be authenticated (cognito).
4. The product(s) should be `ONLY` deleted from PRODUCT referential document.

- From `/products` [BR_PRODUCT_REMOVE_PRODUCTS](#brproductremoveproducts)
- From `/products/view/:id` [BR_PRODUCT_REMOVE_PRODUCT](#brproductremoveproduct)

5. Use case ends when Actor is redirected to sign in page.

# Business Rules

## BR_PRODUCT_REMOVE_PRODUCT

- Remove product from id
- Return product data on success

## BR_PRODUCT_REMOVE_PRODUCTS

- Remove products from array
- Return true if all products are removed else return false.
