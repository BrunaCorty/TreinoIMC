# TreinoIMC
https://www.jdoodle.com/ia/fsZ

import java.util.Scanner;
public class Calcula_IMC {
    public static void main (String args[]) {
        float pesoPessoa, alturaPessoa, valorIMC;
        String grauObesidade;
        Scanner sc = new Scanner(System.in);
        System.out.println("Entre com a altura da pessoa em metros");
        alturaPessoa = sc.nextFloat();
        System.out.println("Entre com o peso da pessoa em Kilogramas");
        pesoPessoa = sc.nextFloat();
        valorIMC = (pesoPessoa) / (alturaPessoa*alturaPessoa);
        System.out.println("O IMC da pessoa é "+valorIMC);
        if (valorIMC < 18.5)    {grauObesidade = "A pessoa está abaixo do peso"; }
        else if (valorIMC < 25) {grauObesidade = "A pessoa está com peso normal"; }
        else if (valorIMC < 30) {grauObesidade = "A pessoa está com sobrepeso"; }
        else if (valorIMC < 35) {grauObesidade = "A pessoa está com obesidade grau 1"; }
        else if (valorIMC < 40) {grauObesidade = "A pessoa está com obesidade grau 2"; }
        else                  {grauObesidade = "A pessoa está com obesidade grau 3"; }
        System.out.println("O diagnóstico da pessoa é: "+grauObesidade);
    }
}

