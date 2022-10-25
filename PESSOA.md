/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Main.java to edit this template
 */
package pessoa;

/**
 *
 * @author OMARI
 */
public class Pessoa {
    private String nome, sexo;
    private int ano, idade;
    private float salario,peso,altura,imc;

    @Override
    public String toString() {
        return "Nome: " + nome + "Sexo: " + sexo + "Ano de nascimento: " + ano + 
                "Salario:  " + salario + "peso: " + peso + "altura: " + altura+ 
                "IMC: "+ imc+"idade"+idade;
    }

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public String getSexo() {
        return sexo;
    }
    
    public void setSexo(String sexo) {
        this.sexo = sexo;
    }

    public int getAno() {
        return ano;
    }

    public void setAno(int ano) {
        this.ano = ano;
    }

    public float getSalario() {
        return salario;
    }

    public void setSalario(float salario) {
        this.salario = salario;
    }

    public float getPeso() {
        return peso;
    }

    public void setPeso(float peso) {
        this.peso = peso;
    }

    public float getAltura() {
        return altura;
    }

    public void setAltura(float altura) {
        this.altura = altura;
    }
    public float calculaImc() {
        imc=peso/(altura*altura);
        return imc;
    }
    public int calculaIdade() {
        idade=2022-ano;
        return idade;
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

