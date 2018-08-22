# atividade-22-08package atividade;

import javax.swing.JOptionPane;

public class atividade {
    public static void main(String[] args) {
      String nome = JOptionPane.showInputDialog(null, "Digite seu nome: ","Seu nome", JOptionPane.QUESTION_MESSAGE);
      String txt = JOptionPane.showInputDialog(null, "Digite sua idade: ","Sua idade", JOptionPane.QUESTION_MESSAGE);
      int idade = Integer.parseInt(txt);
      
      if (idade >= 18){
          JOptionPane.showMessageDialog(null, nome + " você já pode tirar a CNH", "Parabéns!", JOptionPane.INFORMATION_MESSAGE);
      }else{
          JOptionPane.showMessageDialog(null, nome + " você não pode tirar a CNH, você tem apenas " + idade + " anos.", ":(", JOptionPane.INFORMATION_MESSAGE);
      }
    }
}
