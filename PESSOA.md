
package pessoa;

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



