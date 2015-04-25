## Website Performance Optimization portfolio project

Improving the website performance on page rankings

Step 1: Made the google analyics to be async so that it didn't not hold back loading the page

Step 2: Change print css to be a @ media type print so it did not delay loading the page

Step 3: Resized pictures and optimized image using ImageOptim for both the Pizza picture as well as the profile pic

Step 4: In-lined the Font CSS file into the main style.css file so that the broweser did not need to load fonts separately

Step 5: In-lined the css into the main index html file. 

Step 6 : Uglify the css and html files to remove all comments and empty spces to make the website load faster. 

Improving the pizza.html - Ensuring 60fps while scrolling

Step 1: Pulled out scrolling to be outside the loop in the updatePosition function so it's not checking layout after each pixel. This will remove the forced synchronous layout error. 

Step 2: Changed the event listener function addEventLister so that the loop is now up to 30 instead of 200. You only need 30 pizzas to populate the page

Improving the pizza.html - Improving speed of resizing pizza

Rewrote the changePizzaSizes function when the input is listed it sets the new width of the pizza to be a certain percentage. This way we do not have to redo any calculations from pixels to percentages the old code was doing. 