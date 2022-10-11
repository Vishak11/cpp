import java.rmi.*;
import java.rmi.server.*;
public class checkserver{
	public static void main(String[] args){
		
	try{
		
	checkimpl impl=new checkimpl();
	Naming.rebind("check",impl);
	}
	catch(Exception e)
	{
		System.out.println(e);
	}
	}
}
	