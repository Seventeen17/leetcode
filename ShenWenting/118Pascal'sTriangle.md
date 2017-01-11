
```

class Solution(object):
    def generate(self, numRows):
        """
        :type numRows: int
        :rtype: List[List[int]]
        """
    	G = [[1] * i for i in range(1,numRows+1) ] 
    	print G
    	for i in range(2, numRows):
    		for j in range(i-1):
    			G[i][j+1]=G[i-1][j]+G[i-1][j+1]
    	return G
      
```
