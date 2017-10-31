# Lab-10-NumberPalindrome
calculates largest palindrome 

package lab10;

public class PalindromTest {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		int ar[]= new int[91];
		int num = 10;
		for(int i =1;i<91;i++)
		{
			ar[i]=num;
			num++;
			//System.out.print(ar[i] + " ");
		}
		int n =0;
		while(n>=0)
		{
			n = calcAr(ar);
			System.out.println(n);
			if(!palindromeCheck(n))
			{
				System.out.println("N is not palindrome");
			}
			else
				System.out.println("N is a palindrome");
		}

	}

	private static boolean palindromeCheck(int n) {
		
		return false;
	}

	private static int calcAr(int[] ar) {
		// TODO Auto-generated method stub
		int num=0;
		for(int i =90;i>=1;i--)
		{
			num = ar[i]*ar[i-1];
		}
		return num;
		
	}

}
