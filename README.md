# How to run
Just pushing to heroku with the following system variables is the easiest way to run, or npm start locally maybe.

SHOPIFY_API_KEY:              YOUR_API_KEY

SHOPIFY_API_SECRET:           YOUR_API_SECRET

SHOPIFY_API_VERSION:          2022-04

SHOPIFY_MONGO_DB_NAME:        YOUR_DB_NAME (any name is OK)

SHOPIFY_MONGO_URL:            mongodb://YOUR_ID:YOUR_PASSWORD@YOUR_DOMAIN:YOUR_PORT/YOUR_DB_NAME

SHOPIFY_JWT_SECRET:           YOUR_JWT_SECRET (any value is OK)

# Installation Endpoint
`https://SHOPIFY_SHOP_DOMAIN/admin/oauth/authorize?client_id=YOUR_API_KEY&scope=write_payment_gateways,write_payment_sessions&redirect_uri=YOUR_APP_URL/callback&state=&grant_options[]=`　

or 

`YOUR_APP_URL/?shop=SHOPIFY_SHOP_DOMAIN`

# Map your mTLS path with payment session fields

https://shopify.dev/apps/payments/creating-a-payments-app/creating-a-payments-app#payments-app-extension-configuration-fields

Payment session URL: /payment

Refund session URL: /refund

Capture session URL: /capture

Void session URL: /void

