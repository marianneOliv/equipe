# import java.util.ArrayList;
import javax.swing.JOptionPane;


public class ExecutaPessoa {
    public static void main(String[] args) {   
    ArrayList<Pessoa> Pessoa=new ArrayList<>();
    
    int quantHomens=0, quantMulheres=0,cadastros=0;
    cadastros=Integer.parseInt(JOptionPane.showInputDialog(null,"Quantidade de cadastros:"));
    
    for (int i= cadastros;i>0;i++){
    if (cadastros>0 || cadastros==cadastros){
        Pessoa p=new Pessoa();
    
    p.setNome(JOptionPane.showInputDialog("Informe o nome:"));
    p.setAno(Integer.parseInt(JOptionPane.showInputDialog("AAAA")));
    p.setPeso(Float.parseFloat(JOptionPane.showInputDialog("Peso")));
    p.setAltura(Float.parseFloat(JOptionPane.showInputDialog("Altura")));
    p.setSalario(Float.parseFloat(JOptionPane.showInputDialog("Salario")));
    p.setSexo(JOptionPane.showInputDialog("(F)ou (M)"));
    
    if (p.getSexo().equals("M")) {
        quantHomens++;
    } else if (p.getSexo().equals("F")) {
        quantMulheres++;
    }
    Pessoa.add(p);
                    
    }else {
         JOptionPane.showMessageDialog(null, "INFO\n\n Total: "+ Pessoa.size() + "\n Homens: " + quantHomens + " - " +
                 (quantHomens * 100 / Pessoa.size()) + "%" + "\n Mulheres: "
                 + quantMulheres + " - " + (quantMulheres * 100 / Pessoa.size()));
    }
        
    }
   
    }

}





import java.util.ArrayList;
import javax.swing.JOptionPane;


public class ExecutaPessoa {
    public static void main(String[] args) {   
    ArrayList<Pessoa> Pessoa=new ArrayList<>();
    
    int quantHomens=0, quantMulheres=0,cadastros=0;
    cadastros=Integer.parseInt(JOptionPane.showInputDialog(null,"Quantidade de cadastros:"));
    
    for (int i= cadastros;i>0;i++){
    if (cadastros>0 || cadastros==cadastros){
        Pessoa p=new Pessoa();
    
    p.setNome(JOptionPane.showInputDialog("Informe o nome:"));
    p.setAno(Integer.parseInt(JOptionPane.showInputDialog("AAAA")));
    p.setPeso(Float.parseFloat(JOptionPane.showInputDialog("Peso")));
    p.setAltura(Float.parseFloat(JOptionPane.showInputDialog("Altura")));
    p.setSalario(Float.parseFloat(JOptionPane.showInputDialog("Salario")));
    p.setSexo(JOptionPane.showInputDialog("(F)ou (M)"));
    
    if (p.getSexo().equals("M")) {
        quantHomens++;
    } else if (p.getSexo().equals("F")) {
        quantMulheres++;
    }
    Pessoa.add(p);
                    
    }else {
         JOptionPane.showMessageDialog(null, "INFO\n\n Total: "+ Pessoa.size() + "\n Homens: " + quantHomens + " - " +
                 (quantHomens * 100 / Pessoa.size()) + "%" + "\n Mulheres: "
                 + quantMulheres + " - " + (quantMulheres * 100 / Pessoa.size()));
    }
        
    }
   
    }

}

