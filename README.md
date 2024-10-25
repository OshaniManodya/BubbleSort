import java.util.Scanner;
import java.util.Arrays;
public class BubbleSortEx{
    public static void main (String[]args)
    {
       int number[] = new int[] {8, 3, 1, 4, 5, 11, 7, 2, 17, 13};

       System.out.println("Unsorted array: "+Arrays.toString(number));
       int i;
       int j;
       int n=number.length;

       for(i=0;i<n-1;i++)
       {
        for(j=0;j<n-i-1;j++)
        {
           if(number[j]>number[j+1])
           {
            int swap=number[j];
            number[j]=number[j+1];
            number[j+1]=swap;

           }
        }
        
       }
       System.out.println("Sorted array: "+Arrays.toString(number));

    }
}
