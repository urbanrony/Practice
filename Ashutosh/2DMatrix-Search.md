# Title: Matrix-Search 2D array

Question link: https://leetcode.com/problems/search-a-2d-matrix-ii/

### Code:

```
class Solution {
    public boolean searchMatrix(int[][] matrix, int target) {
    if (matrix == null || matrix.length == 0 || matrix[0].length==0)
        return false;
    int row = 0;
    int col = matrix[0].length - 1;
    while (row < matrix.length && col >=0){
        if (matrix [row][col]==target)
            return true;
        
        if (matrix[row][col]>target)
            --col;
        else 
            ++row;
}
        return false;
}
}

```

### Output:
![capture (488)](https://user-images.githubusercontent.com/68456662/120343242-2c9b3c80-c316-11eb-9d06-a45505092619.png)


### Comments:
will do it better
