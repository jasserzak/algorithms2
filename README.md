function insertionSort(arr) {
  // Iterate through the array starting from the second element
  for (let i = 1; i < arr.length; i++) {
    let key = arr[i]; // Store the current element as the key
    let j = i - 1; // Initialize j to the previous index

    while (j >= 0 && arr[j] > key) {
      arr[j + 1] = arr[j]; // Shift the element to the right
      j--; // Decrease the index to compare with the previous element
    }

    
    arr[j + 1] = key;
  }

  return arr;
}

const unsortedArray = [8, 3, 6, 2, 1];
console.log(insertionSort(unsortedArray)); 
