# Shopify Auto Shipping Label Printer
## Run

```
git clone https://github.com/pseudozach/autoprinter.git
npm i
node index.js
```

## Use
* Go to your Shopify Admin Page and create a webhook to be sent for order/paid.
* Enter your homeserver address that's running `node index.js` from this library as the endpoint.
Depending on your home/office router dynamic DNS setup it will look something like this:
`http://xxx.tplinkdns.com:3000/printit`
* Remember to forward port 3000 to the raspberry pi or computer that's running this app.

* Now everytime you have a new order/paid event, your Brother printer will automatically print the shipping label for you!

This app conforms to shopify API at https://shopify.dev/docs/admin-api/rest/reference/events/webhook#create-2021-04