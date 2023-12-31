# Amazon Mockup Website

This is a mock website of the official Amazon website. The main function of this website is to display items in a grid view, each with a rating and a price with the option to add quantities of each item (up to 10 items quantity). Adding them to the cart will affect the number and will change depending on how many items are added. 

![](images/amazonhome.png)

It exists to test my JavaScript skills and apply them to a website modelled after a real world website. 

The technical concepts my project supports is the use of media queries to modify the CSS of HTML elements depending on the size of the screen being used to view the website, making an array of objects to showcase within a grid, and how to id each object so that the code knows the difference between each object. 

## Core Technical Concepts

This is an array of objects in the products.js file. Each object or product has an id, image, name, rating, price, and keywords. Each product is given an id to help the code determine the differences between each product for the code to give the correct item with the correct price at checkout.

![](images/products.png)

For each product in the products array, the document body produces HTML that displays each product with its respective properties i.e. rating, price, and more.

![](images/js.png)

Every time add to cart below any product gets pressed, the productId is set equal to the productId of the dataset of the button. For each item in the cart, if the productId set earlier matches the productId of the item, matchingItem equals item. Then it tests if the matchingItem is a truthy statement. If it is or if the item being added is already in the cart, add 1 more to it, else push the new item to the cart and give it a quantity of 1. Then, the cartQuantity is set equal to each itemQuantity and the cartQuantity is added to the document body. 

![](images/js1.png)

This was added to make the text less congested and keep each product item name the same height. 

![](images/limit_two_lines.png)



![](images/product_example.png)

![](images/css.png)

The media queries for the checkout page. At 1000px width, the payment summary becomes a horizontal grid. Max-width here means the code is testing desktop first. In most cases, media queries are tested mobile first. I tested it this way because I wanted the desktop version of the website to appear good before I had to worry about the smaller versions of the website.

![](images/css1.png)

Over 1000px width.

![](images/checkout.png)

Under 1000px width.

![](images/checkout1.png)

![](images/checkout2.png)

Code for tracking orders. A progress bar is shown for each order that is set to 50% complete (shipped).

![](images/progress_bar.png)

![](images/progress.png)

## Getting Started/Requirements

To run this website, download the code from [github.com/JCV2022/About-Me-Website](https://github.com/JCV2022/About-Me-Website)

A code editor program is needed. Any should do fine, I used Visual Studio Code to code my website.

If you do use Visual Studio Code as your code editor, install the extension Live Server to be able to run the code in real-time. After installing this extension, right click the code and click on 'open live server'. You can then see the changes you make to the code live whenever you save and view those changes on the browser the code shows up on. 

![](images/liveserver.png)

If node.js isn't installed on your machine, download the LTS version through this link [nodejs.org/en](https://nodejs.org/en) and run the installation.exe file.

Git was used for this project. Go to [git-scm.com/downloads](https://git-scm.com/downloads) and download git for your respective device. After downloading the file and running the installation exe found in your downloads folder, open Visual Studio Code and click on source control on the left hand bar with the project still open and click on 'initialize repository'. This allows you to keep track of changes you make to the code and also lets you push code to the GitHub repository without having to updating the repository manually. 

## Todo

Make the JavaScript take product quantities inputted into consideration when manipulating the number added to the cart i.e. adding 10 basketballs to the cart should increment the number added to the cart to 10 not 1. 

Add functionality to the checkout.html. Right now, only displays two set products and can't checkout.

Edit tracking.html to take orders placed and track them. Set orders are in place by default.

Complete cart.js and checkout.js files.

## Contact Info

My email address is vujonathan00@gmail.com

My github is github.com/JCV2022

My linkedIn is linkedin.com/in/jonathan-vu-409a71132/
