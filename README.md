# node-lodash-average-array
A node application using lodash library to compute average from array
Certainly! Here's an example of how you can calculate the average of an array of objects containing prices with dates using JavaScript with the lodash library's functional approach:

Assuming the array of objects looks like this:

```javascript
const data = [
  { date: '2023-12-01', price: 10.5 },
  { date: '2023-12-02', price: 15.3 },
  { date: '2023-12-03', price: 20.0 },
  // ... more objects
];
```

You can calculate the average price using lodash's functional programming methods like `map`, `reduce`, and `mean`:

```javascript
const _ = require('lodash');

// Example data
const data = [
  { date: '2023-12-01', price: 10.5 },
  { date: '2023-12-02', price: 15.3 },
  { date: '2023-12-03', price: 20.0 },
  // ... more objects
];

// Extract prices into an array
const prices = _.map(data, 'price');

// Calculate average using lodash's mean function
const averagePrice = _.mean(prices);

console.log('Average price:', averagePrice);
```

In this example:

1. `_.map(data, 'price')` extracts an array of prices from the array of objects using lodash's `map` function.
2. `_.mean(prices)` calculates the average of the prices array using lodash's `mean` function.

This approach leverages lodash's functional programming methods to succinctly extract prices and compute the average, providing a clean and concise solution. Make sure to install lodash via npm (`npm install lodash`) or include it via a CDN before using it in your code (`const _ = require('lodash');`).
