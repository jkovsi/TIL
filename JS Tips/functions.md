# Tips about Javascript Functions

- Jake Archibald wrote a nice tips

 - LINK: https://jakearchibald.com/2021/function-callback-risks/


 - Don't use callbacks where they are not intendent to be used, for example `arr.map(callback)` use it as `arr.map(i => callback(i))` so that you avoid unnecessary risk and breaks of the app

 - Same thing goes to *PROMISES* 
  - ``` const nextFrame = () => new Promise(requestAnimationFrame) ```
  - This is equivavelent to 
  - ``` const nextFrame = () => new Promise((resolve,reject) => requestAnimationFrame(resolve, reject))```


  