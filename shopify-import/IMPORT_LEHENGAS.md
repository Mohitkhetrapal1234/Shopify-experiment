# Import Lehengas

This repo now includes a Shopify product CSV for 10 lehengas:

- `shopify-import/lehenga-products.csv`

## In Shopify admin

1. Go to `Products`
2. Click `Import`
3. Upload `shopify-import/lehenga-products.csv`
4. Review and import

## Create the collection

Create a manual or automated collection with:

- Title: `Lehengas`
- Handle: `lehengas`

For an automated collection, use condition:

- Product tag is equal to `lehenga`

## Result

Once the `Lehengas` collection exists and the CSV is imported:

- `/collections/lehengas` will show real products instead of the theme fallback
- the `Lehengas` card on the homepage can be linked to that collection

## Notes

- The current theme already includes a 10-item fallback for an empty `Lehengas` collection
- Importing real products is the correct long-term path because collections and products live in Shopify store data, not theme code
