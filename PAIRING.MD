# Take a Lorry off the Road With Some Code!

Welcome to the Gousto pairing exercise. This [code kata](http://codekata.com/) was inspired by a feature we implemented recently which allowed us to send [1 less lorry out for delivery](https://medium.com/gousto-engineering-techbrunch/taking-a-lorry-off-the-road-with-some-code-a988f70b37c1) every single day! We call this feature **Intelligent Packaging.** We'd like you to build something similar.

## The Problem

![Intelligent Packaging Explained](https://i.imgur.com/8iPoykn.png)

At Gousto we send boxes of ingredients to customers to cook at home and create their perfect dinner. Customers are able to choose multiple recipes for a different number of people. This means the number of ingredients in a box can vary, and the volume of those ingredients can vary by even more.


For this exercise you'll be given two JSON files. 

1) `boxes.json` 
This contains an array of different box sizes available for us to send an order in. Each box will have an ID, dimensions and a CO2 footprint value.
2) `orders.json`. 
This contains an array of orders, each order contains an ID and an array of ingredients. These ingredients will have a volume score.

We'd like you to build an app which takes these two files processes them and determines the smallest possible box that the order will fit into. We call this feature **Intelligent Packaging**

## Expected Output

1) Output a list of the order IDs and the boxes you've matched against them.

2) Output whether we have taken a lorry off the road:
- The sum of the CO2 footprint for every order in the file with Intelligent Packaging.
- The sum of the CO2 footprint without Intelligent Packaging (assuming every order would be in the largest box).
- Whether we have successfully removed a lorry from the road, if we have saved 1000kg of CO2 then this is true (note, these aren't the real numbers, they're much larger!).


## The Rules
1) Approach this problem any way you like, you can build a RESTful service, a command line app or a UI if you wish.

2) The session is for 1.5 hours, but we won't spend the whole time writing code; we like to leave plenty of time at the end for you to answer us questions. Don't feel you have to rush a solution. **You will not be judged on whether you finish or not**. We would much rather you **give us a solution that you are proud of** and feel best displays the type of code you would want to ship into production. That said, make sure there is a way to run your app and it does give some sort of output.

3) We'll approach this in a very similar way to how we pair at Gousto day-to-day. We'd like you to lead the session, but we'll be assisting you and asking questions along the way. We're there to help build the app, not to catch you out.
