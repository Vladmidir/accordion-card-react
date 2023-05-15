### notes:
- In react && can be used to conditionally render elements or render nothing otherwise.
- array.map() takes in a function that is being applied to every element in the array. 
We can pass an arrow function and access the array element via parameters.
- When creating elements using array.map(), we need to add a 'key' property to the outermost returned element.
Here are notes on how to properly use [map() for rendering elements.](https://react.dev/learn/rendering-lists)
Since we render multiple Accordions, each needs a unique key.
```js
//use id as a key
{ accordionData.map(({id, title, body}) => (
    <Accoridion key={id} title={title} body={body} />
  ))}
```
- run `npm run build` AFTER configuring package.json to deploy at github pages.
- run `npm run deploy` to update the deployment at github pages.

