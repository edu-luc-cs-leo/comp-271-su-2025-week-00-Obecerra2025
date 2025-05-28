/*
* Explanation of loops in lines 40-45
*
* First Loop:
*
* for (int i = 0; i < smallest_index; i++) {
*            temporary[i] = arr[i];
*        }
*
* The range of i goes from 0 to just before smallest_index. Then each element is copied before the smallest element and gets ->  
* copied to temporary arr and temporary in the same position before the smallest value.
* 
* Second Loop
*
* for (int i = smallest_index + 1; i < arr.length; i++) {
*            temporary[i - 1] = arr[i];
*        }
*
* The range of i goes from smallest_index + 1 to the end of the array since it copies the elements after the smallest one.
* We use temporary[i - 1] = arr[i]; because we skipped one item which is the smallest so we move the rest to the left by 1.
*/