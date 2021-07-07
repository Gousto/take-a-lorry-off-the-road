# Take a Lorry off the Road With Some Code!
## Take-home Test

Welcome to the Gousto Tech Test. This [code kata](http://codekata.com/) was inspired by a feature we implemented recently which allowed us to send [1 less lorry out for delivery](https://medium.com/gousto-engineering-techbrunch/taking-a-lorry-off-the-road-with-some-code-a988f70b37c1) every single day! We'd like you to do something similar.

## The Problem

![Intelligent Packaging Explained](https://i.imgur.com/8iPoykn.png)

At Gousto we send boxes of ingredients to customers to cook at home and create their perfect dinner. Customers are able to choose multiple recipes for a different number of people. This means the number of ingredients in a box can vary, and the volume of those ingredients can vary by even more.


In this test you'll be given two JSON files. 

1) [`boxes.json`](https://github.com/Gousto/take-a-lorry-off-the-road/blob/master/boxes.json)
This contains an array of different box sizes available for us to send an order in. Each box will have an ID, dimensions and a CO2 footprint value.
2) [`orders.json`](https://github.com/Gousto/take-a-lorry-off-the-road/blob/master/orders.json) 
This contains an array of orders, each order contains an ID and an array of ingredients. These ingredients will have a volume score.

We'd like you to build an app (command line, REST service, whatever you desire) which takes these two files processes them and determines the smallest possible box that the order will fit into. We call this feature **Intelligent Packaging**

## Expected Output

Once you have the smallest possible box that fits all the ingredients we'd like you to return some information to the user

1) Have you taken a lorry off the road?
We'd like you to output 3 things:
- The sum of the CO2 footprint per box for every order in the file with Intelligent Packaging
- The sum of the CO2 footprint without Intelligent Packaging (every order would be in the largest box we have).
- Whether we have successfully removed a lorry from the road, if we have saved 1000kg of CO2 then this is true (note, these aren't the real numbers, they're much larger!)

2) Output a list of the order IDs and the IDs of the boxes you've matched against them.

## The Rules
1) Approach this problem any way you like, you can build a RESTful service, a command line app or a UI if you wish.

2) Spend around 2 hours on this, don't feel you have to rush a solution. **You will not be judged on whether you finish or not**. We would much rather you **give us a solution that you are proud of** and feel best displays the type of code you would want to ship into production. That said, make sure there is a way to run your app and it does give some sort of output.

3) Tests are not a hard requirement but are strongly encouraged, if you're not used to testing your code have a go at it anyway. It's not that hard to get started with it and we promise it will be a great skill for you to learn.

4) Add a Read Me file we'd like you to cover three things. 
- How to run your app
- Explain how you approached the problem, why you've done what you've done and importantly, if this wasn't a 2 hour tech test, what would you do differently?
- Any other comments for us
