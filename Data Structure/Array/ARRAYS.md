## Insertion Element of Array

```js
const insertElement = (position, element) => {
  let arr = [2, 3, 4];
  parseInt(position);

  for (let i = arr.length - 1; i >= position; i--) {
    if (i >= position) {
      arr[i + 1] = arr[i];
    }
    if (i == position) {
      arr[i] = element;
    }
  }

  return arr;
};
console.log(insertElement(0, 1));
```

## Deletion Element of Array

```js
const deleteElement = (position) => {
  let arr = [2, 3, 4];
  parseInt(position);

  for (let i = position; i < arr.length; i++) {
    if (i >= position) {
      arr[i] = arr[i + 1];
    }
  }

  arr.length = arr.length - 1;
  return arr;
};
console.log(deleteElement(2));
```

## Sorting of Array

```js
const sortingElement = () => {
  let arr = [5, 2];

  for (let i = 0; i < arr.length; i++) {
    for (let j = 0; j < arr.length; j++) {
      if (arr[j] > arr[j + 1]) {
        let temp = arr[j];
        arr[j] = arr[j + 1];
        arr[j + 1] = temp;
      }
    }
  }

  return arr;
};
console.log(sortingElement());
```

## Largest Element of Array

```js
const largeElement = () => {
  let arr = [5, 2, 11, 24, 7];
  let largest = arr[0];

  for (let i = 1; i < arr.length; i++) {
    if (largest < arr[i]) {
      largest = arr[i];
    }
  }

  return largest;
};
console.log(largeElement());
```

## Second Largest Element of Array

```js
const secondLargeElement = () => {
  let arr = [5, 2, 8, 6, 8, 5];
  let largest = arr[0];
  let secondLarge = -1;

  for (let i = 1; i < arr.length; i++) {
    if (largest < arr[i]) {
      secondLarge = largest;
      largest = arr[i];
    } else if (arr[i] > secondLarge && arr[i] < largest) {
      secondLarge = arr[i];
    }
  }

  return secondLarge;
};
console.log(secondLargeElement());
```

## Smallest Element of Array

```js
const smallElement = () => {
  let arr = [5, 3, 2, 8, 6, 8, 5];
  let smallest = arr[0];

  for (let i = 1; i < arr.length; i++) {
    if (arr[i] < smallest) {
      smallest = arr[i];
    }
  }

  return smallest;
};
console.log(smallElement());
```

## Second Smallest Element of Array

```js
const secondSmallElement = () => {
  let arr = [5, 3, 2, 2, 8, 6, 8, 5];
  let smallest = arr[0];
  let secondSmallest = Number.POSITIVE_INFINITY;

  for (let i = 1; i < arr.length; i++) {
    if (arr[i] < smallest) {
      secondSmallest = smallest;
      smallest = arr[i];
    } else if (arr[i] > secondSmallest && arr[i] < smallest) {
      secondSmallest = arr[i];
    }
  }

  return secondSmallest;
};
console.log(secondSmallElement());
```

## Remove Duplicates from Sorted Array

```js

```
