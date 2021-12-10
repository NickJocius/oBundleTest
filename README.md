# Obundle Test

Preview code: l8qj8qqd2y

Github Repo: https://github.com/NickJocius/oBundleTest

### Steps Taken

1. added custom catergory page named customCategory.html
2. mapped custom page on config.stencil.json
3. created product from storefront control panel
4. created category from storefront control panel and added custom template
5. created custom js file called customCategory.js and added it the the customClass object in app.js
6. imported swal to use as alert pop up for user triggered events
7. declared variables cartId, addProdUrl and catProds from context
8. created addAllToCart function:
   > > This function takes event, product url as arguments, it is triggered when addAll button is clicked.
   > > it add item to cart or creates and add product to new cart if one doesn't exist.
   > > It makes an http post request using the add to cart url, the sweet alert is triggerd on success or failure and triggers the updateCartContent function.
9. created removeAll function:
   > > This function takes the triggered event and cart id as parameter and makes a DELETE request to the delete cart endpoint. The sweet alert is used for notifying of error or success.
10. I created two buttons in the html page, one addAll button and one removeAll.
11. The removeAll button is only displayed if a users cart is not empty.
12. I used in-line styling to style the new html elements.
13. I created an element above the added form and buttons that displays the customers id, name, email and phone.
    > > This required injecting customer into the html.
14. I created a series of functions to change image on hover.
    > > I used jquery to access the card-image and created two empty arrays to add images to. Then as I looped over the image array I changed the size variables to not revieve error then added on mouseover event to change to second image and on mouseout changed back to original image.
