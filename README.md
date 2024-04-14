# fichaContabanco.encap
package br.com.alura.screenmatch.modelos.Conta;

public class Conta {
    private int NumeroConta;
    private double Saldo;
    //não se esqueça que . não é , double entende o . como ,
    public String titular;
    // você errou o string pela letra maiúscula, tome cuidado com isso
    // como é publica, perceba que não se usa métodos getters e setters para os atributos
    
    public int getNumeroConta() {
        return NumeroConta;
    }

    public void setNumeroConta(int numeroConta) {
        this.NumeroConta = numeroConta;
    }

    public double getSaldo() {
        return Saldo;
    }

    public void setSaldo(double saldo) {
        this.Saldo = saldo;
    }
}
package br.com.alura.screenmatch.modelos.Conta;

public class ContaBancaria {
    public static void main(String[] args) {
        Conta pessoal = new Conta();

        pessoal.setNumeroConta(2354);
        pessoal.setSaldo(4553);
        pessoal.titular = "Pedro";

        System.out.println("Número da Conta: " + pessoal.getNumeroConta());
        System.out.println("Saldo: " + pessoal.getSaldo());
        System.out.println("Titular: " + pessoal.titular);

        pessoal.setSaldo(4553);
        System.out.println("Novo Saldo: " + pessoal.getSaldo());
    }
}
/* saída do código
Número da Conta: 2354
Saldo: 4553.0
Titular: Pedro
Novo Saldo: 4553.0 */
