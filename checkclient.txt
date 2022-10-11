import java.rmi.*;
import java.rmi.server.*;
import java.util.*;
public class checkclient{
	public static void main(String[] args){
		
	try{
		checkint cht=(checkint)Naming.lookup("rmi://localhost/check");
		Scanner sc=new Scanner(System.in);
		String str=sc.next();
		System.out.println("result"+cht.check(str));
	}
	catch(Exception e)
	{
		System.out.println(e);
	}
	}
}