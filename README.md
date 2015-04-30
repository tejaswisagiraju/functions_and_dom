# Functions and The DOM

Try the following exercises in the browser.


## Practice With Functions

* Write a function to swap to values at two different indicies in an array.

  ```
  var swap = function (arr, indexOne, indexTwo) {
    // swap values 

    return arr;
  };
  ```

```

  var arr = [1,2,3]

  var swap = function (arr,indexOne, indexTwo) {

    var value = arr[indexOne]
    arr[indexOne] = arr[indexTwo]; 
    arr[indexTwo] = value 
    
    return arr;
  }

  swap(arr,0,1);

  console.log(arr);


```

* Write a function to generate a random number in a specified range.

  ```
  var getRand = function (low, high) {
    // your work

    return randNum;
  };
  ```

```

  var getRand = function (low, high) {
    
    var randNum = Math.random() * (high - low + 1) + low;

    return randNum;
};

getRand(5,6);



```

* Write a function to create a specified number of random numbers from `1` to `100` in an array.

  ```
  var randArr = function (size) {
    // your work;

    return arr; 
  }
  ```



* Write a function to find the maximum number in an array.

```
  var getMax = function (arr) {
    // your work
    
    return max;
  }

```

```

  var array = [6,4,9,8,7];

  var getMax = function (arr) {
    
    var maximumNumber = arr[0];
    for (var i =1; i< arr.length; i++) {
      if (arr[i] > maximumNumber) {
        maximumNumber = arr[i];
      } 
    }  
  
  return maximumNumber;
  
  }

  console.log(getMax(array));


```



## Playing With The DOM

Go to [generalassemb.ly](https://generalassemb.ly) and try the following exercises.

* Grab the `body` from the page using, `document.querySelector`. and chnage the `opacity` to `.5`.
* Grab all the `img` tags from the page. Iterate through each image and change the source to `http://www.maine-coon-cat-nation.com/image-files/girl-kitten-names.jpg`.
  * Create a `kittenPaint` function for your code above .Save it as a snippet in your developer console. Go to yahoo and run it there.
* Using `document.querySelectorAll("*")` to grab all elements on the page, iterate through each `element` in the list using a `for` loop. Use `element.style.backgroundImage = "url(http://www.maine-coon-cat-nation.com/image-files/girl-kitten-names.jpg)"` to change every element to have a kitten background image.
  * Create a `kittenBomb` function with the above backgroundImage changing feature and save it to your `sources` under snippets. Run it on your favorite site.
* Select the `body` from the page. When the body is clicked, change its style using the following, `body.style.transform = "rotateZ(60deg)";`.
* Using the element transform from above, grab every `img` off the page, and create a `click` event on the `body` that iterates through all images and rotates them. In other words, when the page is clicked rotate all images on the pages.


