# Program-for-array-rotation
This program will rotate given array according to given rotation size 
class RotateArray 
{
	

	/* utility function to print an array */
	public void leftRotate (int arr[], int d , int n)
	{
	    for(int i=0;i<d;i++)
	    {
	        int tmp =arr[0];
	        for(int j=0;j<n-1;j++)
	        {
	            
	            arr[j]=arr[j+1];
	        }
	        arr[n-1]=tmp;
	    }
	    for(int k=0;k<n;k++)
	    System.out.print(arr[k]);
	}
	


	public static void main(String[] args) 
	{
		RotateArray rotate = new RotateArray();
		int arr[] = {1, 2, 3, 4, 5, 6, 7};
		rotate.leftRotate(arr, 2, 7);

	}
}


