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
![capture (488)](https://user-images.githubusercontent.com/68456662/120341860-e1345e80-c314-11eb-8074-974604b71d74.png)


### Comments:
will do it better
