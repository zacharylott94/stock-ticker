Original Code Author: Zachary Lott
This code is provided as is, without guarantee or warranty


# Directions for deployment

1. Grab an API key from here: https://www.alphavantage.co/support/#api-key
2. Head down to the function 'wrapper'
3. In each of the URLs in the httpRequests, replace APIKEY with your own API key

# Directions for adding another stock to track

1. In the body tag of the HTML, copy one of the divs with the class 'stock' and paste it under the others
2. Change the id of that div to the symbol of your new stock
3. Go down to the variable 'last' near the top of the javascript block
4. Add another property to 'last' where the name of the property is The symbol of your stock
5. Head further down to the function 'wrapper'
6. Copy one of the httpRequests and paste it under the others
7. In the URL in the new httpRequest, replace the value at 'symbol' with the symbol of the new stock you want to track


# Directions for changing the update frequency of the page

1. Go down to the bottom of this file.
2. Where it says 'setInterval', change the number to however many milliseconds you want to wait between updates. I recommend not setting this below a minute; this is to avoid excessive API calls.
