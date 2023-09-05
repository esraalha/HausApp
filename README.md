# HausApp
public class HausApp {
	
	static Haus h = new Haus(10) ;

	
	static void ausgabeGroesse() {
		Familie [] arr = h.getBewohner();
		for (int i = 0; i < arr.length; i++) {
			 System.out.println(arr[i].getGroesse());
			if(arr[i] == null) {
				continue;
			}
			System.out.println(arr[i].getGroesse());
			
			if(arr[i].getGroesse()> Zahlen.ZAHAL2) {
				
			}
			 if (arr[i].getGroesse()<= Zahlen.ZAHAL1) {
				System.out.println("Die Familie ist klein");
			}
			 
			 
			else {
				System.out.println("Die Familie hat eine übliche Größe");
			}
			
		}	
	}

	public static void main(String[] args) {
		
		//Familie a = new Familie ("Hesso",3);
		
		String[]arry = new String [3];
		h.einzug("Hesso", arry,2);
		arry[0] = "ali";
		arry[1]= "Mo";
		arry[2]= "Ibo";
		
		
		
		String[]arry2 = new String [3]; 
		h.einzug("Alhajje", arry2,1);
		arry2[0] = "esra";
		arry2[1]="Dua";
		
		
		ausgabeGroesse();
		System.out.println();
	}
	
