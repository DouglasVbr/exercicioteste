# exercicioteste

PARTE.1

package exemplomaincap;

public class ExemploMainCap {

    public static void main(String[] args) {

        Caneta c1 = new Caneta(true);
        Caneta c2 = new Caneta(false);
        c1.imprimir();
        c1.setcor("laranja");

        c1.imprimir();
        c1.setponta(1.5);
        c1.imprimir();
        c1.ponta = 2.5;
        c1.imprimir();
        c1.imprimir();
        c2.setcor("roxo");
        c2.imprimir();
    }

}


PARTE.2


package exemplomaincap;

public class Caneta {

    private String cor;
    private boolean tampa = true; // esta tampada
    private int tinta;
    double ponta;

    public Caneta(boolean tampa) {

        this.cor = "Azul";
        this.tampa = tampa;
        this.ponta = 0.0;
        this.tinta = 100;
    }
    //metodos acessores

    public String setcor(String Cor) {

        this.cor = Cor;
        return cor;
    }

    String getcor() {

        return cor;

    }

    public boolean settampa(boolean tampa) {

        this.tampa = tampa;
        return tampa;

    }

    public boolean gettampa() {

        return tampa;

    }

    public double setponta(double ponta) {

        this.ponta = ponta;
        return ponta;
    }

    public double getponta() {

        return ponta;

    }

    public int settinta(int tinta) {

        this.tinta = tinta;
        return tinta;
    }

    public int gettinta() {

        return tinta;

    }

    public String VerificacaoTampa() {

        if (tampa == true) {
            return "Caneta com Tampa";
        } else {
            return "Caneta Sem Tampa";
        }
    }

    public void imprimir() {

        System.out.println(" cor = " + getcor()); // chama o metodo getcor
        System.out.println("a tampa a caneta é: " + gettampa());
        System.out.println("a tinta esta em: " + gettinta());
        System.out.println("a ponta é" + getponta());
        System.out.println("  a caneta está " + VerificacaoTampa());

    }

    

}
