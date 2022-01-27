class Solution:

    def reverse(self, arr, i, j):
        while j > i:
            arr[i], arr[j] = arr[j], arr[i]
            i += 1
            j -= 1
        return arr
           
    
    def nextPermutation(self, arr: List[int]) -> None:
        N = len(arr)
        if N <= 1:
            return arr
            
        i = N-2
        while i >= 0 and arr[i] >= arr[i+1]:
            i -= 1
        index1 = i
        
        if i >= 0:
            j = N-1
            while arr[i] >= arr[j]:
                j -= 1
            index2 = j
            arr[i], arr[j] = arr[j], arr[i]
        
        arr = self.reverse(arr, i+1, N-1)
        
