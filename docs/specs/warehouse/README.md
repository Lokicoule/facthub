# Warehouse

## Description

A. Definition

Nothing to say about it. A warehouse is a warehouse :)

B. Schema

- Warehouse

```
id: string
code: string
name: string
addresses: Address[]
```

- Address

```
id: string
name: string
postalCode: string
city: string
country: string
default: boolean
```

- [Setting](../settings/README.md)

```
useCase: ProductSettingEnum
params: Parameter[]
```

---

# Screens

## Create Warehouse Form

<img src="./screens/create-warehouse.screen.png">
<img src="./screens/create-warehouse-address.screen.png">

## Update Warehouse Form

<img src="./screens/update-warehouse.screen.png">

## View Warehouse

<img src="./screens/view-warehouse.screen.png">

## View Warehouses

<img src="./screens/view-warehouses.screen.png">

---

# Use case

- > [UC_WAREHOUSE_CREATE_WAREHOUSE](./create-warehouse.use-case.md#ucwarehousecreatewarehouse)
- > [UC_WAREHOUSE_UPDATE_WAREHOUSE](./update-warehouse.use-case.md#ucwarehouseupdatewarehouse)
- > [UC_WAREHOUSE_REMOVE_WAREHOUSE](./remove-warehouse.use-case.md#ucwarehouseremovewarehouse)
