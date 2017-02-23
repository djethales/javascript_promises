#JavaScript Promises
Udacity Course

##Lessons
1. Callback vs Promises
  - Promise object is used for deferred and asynchronous computations.
  - asynchronous - happens at an unknown or unpredictable time
2. Callbacks vs Thens
  - Add callback to a function and run at a later time when conditions are met
  - errors - how to handle
  - sequence of work - use .then
3. Wrapping (Promise), thening (Promise->value->action), catching (Promise->value->recovery), chaining (Promise->value->promise->)
  - https://developers.google.com/web/fundamentals/getting-started/primers/promises
  - Four States:
    - Fulfilled - resolved
    - Rejected - it didn't work
    - Pending - still waiting
    - Settled - something happened
4. How and when promises executed - event listener set after even fires, never gets called.  First resolve promise, then set action for resolution value - then it will fire.
Example:  new Promise(function(resolve, reject){
            resolve('hi'); //works
            resolve('bye'); //can't happen again
          });
          - promise can only settle once
          - try and catch wrappers
5. When to use:  ajax requests, web worker (api) requests (work on separate threads and post data to main thread)
