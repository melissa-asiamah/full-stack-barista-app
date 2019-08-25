# Project
This is a full stack app for barista cafe workers where they can enter in a customer's name and order to a queue, check off a completed order while having it called out using Javascript's built in text-to-speech property and lastly clear all completed orders.

![alt tag](img/landing-page.png)
![alt tag](img/profile-page.png)

## How It's Made:

**Live preview here:** https://order-ready-app.herokuapp.com/

**Tech used:** HTML, CSS, JavaScript, Node.js, Mongoose, MongoDB

This is a simple CRUD app using OAuth to authenticate the user login process. Anytime a barista logs in, they can only view their specific orders to indivually mark off to complete. The posting of the orders is handled by an app.post and displayed in the DOM using a loop via EJS. Once the order is compeleted it is updated with a fetch that changes it's property from false to true in MongoDB. This allows it to be rendered into the DOM on the completed side. Lastly, the barista is able to clear all orders by clicking the clear button that triggers an app.delete that removes all orders marked as "true" in the MongoDB collection.


## Lessons Learned:

Some important takeaways from working on this series was learning how to handle NoSQL JSON issues in my collection and connecting it to CRUD methods via Node.
