class FindDuplicate {
    
    void printRepeating(int arr[], int size)
    {
        int i;
        System.out.println("The repeating elements are : ");
         
        for (i = 0; i < size; i++) {
            int j = Math.abs(arr[i]);
            if (arr[j] >= 0)
                arr[j] = -arr[j];
            else
                System.out.print(j + " ");
        }
    }
 
 
    public static void main(String[] args)
    {
        FindDuplicate duplicate = new FindDuplicate();
		
		nums1 = [1,3,4,2,2];
        int nums1_arr_size = nums1.length;
        duplicate.printRepeating(nums1, nums1_arr_size);
		
		nums2 = [3,1,3,4,2];
        int nums2_arr_size = nums2.length;
        duplicate.printRepeating(nums2, nums2_arr_size);
		
		nums3 = [1,1];
        int nums3_arr_size = nums3.length;
        duplicate.printRepeating(nums3, nums3_arr_size);
		
		nums4 = [1,1,2];
		int nums4_arr_size = nums4.length;
        duplicate.printRepeating(nums4, nums4_arr_size);
    }
}
