# sistematizacoes-uniceub
Atividades Práticas  de fim de ciclo do curso ADS
Atividade Final POO 1

Classe 1 – Vacinação Covid
package POO;

public class VacinacaoCovid {
		        
	    String Laboratorio;
	    int Doses;
	    	   
	    public void setLaboratorio (String Laboratorio) {
	        this.Laboratorio = Laboratorio;
	    }
	        public String getLaboratorio () {
	            return Laboratorio;
	        }
	    
	    public void setDoses (int Doses) {
	        this.Doses = Doses;
	    }
	    public int getDoses (){
	        return Doses;
	    }
	    
}
Classe 2 - Brasilia
package POO;

public class Brasilia extends VacinacaoCovid {
	
	public static void main(String[] args) {
	//TODO autogenerated method stub
	//Aplicaçao de herança utilizando os atibutos da Classe superior
		
		Brasilia brasilia1 = new Brasilia ();
		brasilia1.setLaboratorio("oxford");
		brasilia1.setDoses(2);
		
	//Aplicação de herança utilizando o objeto da Classe superior
		
		VacinacaoCovid vacinacaocovid1 = new VacinacaoCovid ();
		vacinacaocovid1.setLaboratorio("jansen");
		vacinacaocovid1.setDoses(1);
	
	System.out.print ("Laboratorio:"+brasilia1.getLaboratorio());
	System.out.print ("Doses:"+brasilia1.getDoses());
	
	System.out.print("Laboratorio:"+vacinacaocovid1.getLaboratorio());
	System.out.print ("Laboratorio:"+vacinacaocovid1.getDoses());
		
	}

}

Polimorfismo
package POO;

public class Influenza implements Brasilia {
			
		String Laboratorio;
		int Doses;
		
		public void setLaboratorio (String Laboratorio) {
	        this.Laboratorio = Laboratorio;
	    }
	        public String getLaboratorio () {
	            return Laboratorio;
	        }
	    
	    public void setDoses (int Doses) {
	        this.Doses = Doses;
	    }
	    public int getDoses (){
	        return Doses;
	    }
	   
public static void main(String[] args) {
		  	
	    Influenza influenza1 = new Influenza();
		influenza1.setLaboratorio("GSK");
		influenza1.setDoses(1);
		
		System.out.print ("Laboratorio:"+influenza1.getLaboratorio());
		System.out.print ("Doses:"+influenza1.getDoses());
		 }
}
