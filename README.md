# Pycker (pronounced picker)

## Sync
```
Fetch orders

For each order
  Save to temp db
```

## Scanner

```
When input from scanner is detected
  find order from temp DB

  if !order
    display no order error

  if !shipped
    display packing info
    print label
    mark as shipped
  else
    display shipped warning
    display packing info
```

## Mark as shipped

```
if network
  mark as shipped
  process offline orders
else
  add to offline queue
```
