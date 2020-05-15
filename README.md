# Returning Strings Lab

## Objectives

- Return a string from a route.
- Use that string and replace the inner HTML of a div.

## Introduction

Included in the lab is a simple Order/Invoice/Customer application.
We're going to use what we've learned so far to add API endpoints and
use AJAX to bring data to the page.

## Instructions

1.  Add a product `description` and an `inventory` count to the `Product`
    model.
2.  Create an index page for all products that displays name and a truncated description, but not inventory.
3.  Create the new product page so you can add new products, otherwise the rest of this might be kind of underwhelming!
4.  Add a route and action that gets just a product description as a
    plain string.
5.  Add another route and action that checks if inventory is available.
    This route should return just `"true"` or `"false"` as strings.
6.  Add a "More Info" button to each product that, when clicked, fetches
    the description and the inventory and displays the result. If there
    is inventory available, display "Available" and if there isn't, display
    "Sold Out".
7.  Make sure tests pass!

## PhantomJS Errors

If you receive this error:

`Could not find an executable ["phantomjs"] on your path.`

You'll need to install PhantomJS on your computer before the tests will work. 

For Mac users, run the following:

```sh
brew cask install phantomjs
```

For Windows users, run the following:

```sh
npm install -g phantomjs-prebuilt
```

You can confirm the installation has worked by running `phantomjs -v`.
