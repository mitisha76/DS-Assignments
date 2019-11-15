package STACK;
import java.util.*;

public class CheckParenthesis {

	
	void check()
	{
		System.out.println("Enter the String");
		Scanner sc=new Scanner(System.in);
		String str=sc.next();
		Stack<Character> s=new Stack<Character>();
		char[] a=str.toCharArray();
		int flag=0;
		for(int i=0;i<a.length;i++)
		{
			if(a[i]=='('||a[i]=='['||a[i]=='{')
				s.push(a[i]);
			else if((a[i]==')'||a[i]=='}'||a[i]==']')&&s.empty())
			{
				flag=1;
				break;
			}
			else if(a[i]==')'&&s.peek()=='(')
				s.pop();
			else if(a[i]=='}'&&s.peek()=='{')
				s.pop();
			else if(a[i]==']'&&s.peek()=='[')
				s.pop();
			
		}
		if(flag==0&&s.empty())
			System.out.println("Balanced");
		else
			System.out.println("Unbalanced");
	}
	public static void main(String args[])
	{
		CheckParenthesis p=new CheckParenthesis();
		p.check();
	}

}
