# simple-spa-router-ts
Basic router written in one class. Useful for small projects/prototyping.

`yarn add simple-spa-router-ts`

## Example

```javascript

import Router from "simple-spa-router-ts";

const router = new Router({
    mode: "hash",  // hash or history
    root: "/",
});

// Add routes + logic to handle route changes
router
    .addRoute(/about/, () => {
        // Route to about page: /#/about/
    })
    .addRoute(/blog\/post/, () => {
        // Regex to handle all URLs starting with /#/blog/post/
    })
    .addRoute("", () => {
        // Route to homepage: /#/
    });

```
