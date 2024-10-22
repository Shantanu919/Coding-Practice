# Coding-Practice
Through- This- Repository- I- Practice- Coding -Problems 
# Given an integer array nums, return an array answer such that answer[i] is equal to the product of all the elements of nums except nums[i].

# The product of any prefix or suffix of nums is guaranteed to fit in a 32-bit integer.

# You must write an algorithm that runs in O(n) time and without using the division operation.

nums = [1,2,3]
class Solution(object):
    def productExceptSelf(self, nums):
        answer = []
        product = 1
        for i in range(len(nums)):

          for j in range(len(nums)):

            if i != j :
              product = product*nums[j]
            else:
                continue

          answer.append(product)

        return answer

we = Solution()
we.productExceptSelf(nums)
#wrong approach
