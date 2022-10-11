import java.rmi.*;
import java.rmi.server.*;
public interface checkint extends Remote{
	public int check(String str) throws RemoteException;
}