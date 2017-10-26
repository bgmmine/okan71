package deneme;
import java.util.Scanner;

public class lab1 {
	public static void main(String[] args){
     // TODO Auto-generated method stub
	// verileri yarat
	
	int count = 1;
	int dogrusayi =0;
	int n1, n2;
	int kullsonuc, asilsonuc ;
	final int MAXSORUSAYISI = 5;
	Scanner input = new Scanner (System.in); 
	while (count <= MAXSORUSAYISI) {
	
		 n1 = (int) (Math.random()*11);
		 n2 = (int) (Math.random()*11);
		 if (n1>n2)
			 asilsonuc = n1-n2;
		 else
			 asilsonuc = n2-n1;
		System.out.println(count + "-cikarma isleminin sonucunu girin " +n1 +" " + n2 );
		kullsonuc = input.nextInt();
		if(kullsonuc == asilsonuc){
			dogrusayi++;
		} 
			count++;
		}
	System.out.println("dogru sayiniz " + dogrusayi);
	}
}
