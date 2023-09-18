- 👋 Hi, I’m @hugobernar
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
hugobernar/hugobernar is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
/ CLASSE DE CADASTRO DE USUARIOS...

import java.util.Scanner;
import java.util.ArrayList;
public class Usuarios {

    public static void main(String[] args) {
     
        Scanner l = new Scanner(System.in);
        
        System.out.println("BEM VINDO AO CADASTRO DE USUÁRIOS");
        
        System.out.println("Digite os dados: "+"\nNome ");
        
        String nome = l.nextLine();
        
        System.out.println("Login desejado ");
        
        String login = l.nextLine();
        
        System.out.println("Cargo ");
        
        String cargo = l.nextLine();
        
        System.out.println("Senha de acesso");
        
        int senha = l.nextInt();
        
        
        Dados usuario;
        
        usuario = new Dados();
        
        usuario.setNome(nome);
        usuario.setLogin(login);
        usuario.setCargo(cargo);
        
        
        ArrayList<Dados> usuarios = new ArrayList<Dados>();
        
        usuarios.add(usuario);
        
        System.out.println(usuario.getNome()+"\n"+usuario.getLogin()+"\n"+usuario.getCargo());
     }
}
// CLASSE QUE GUARDA AS VARIAVEIS DOS OBJETOS...
public class Dados {
    
   private String nome;
   
   private int senha;
   
   private String login;
   
   private String cargo;
    
   
   public Dados(){
   
   
   }
   
   public String getNome(){
   
   return nome;
   }
   
   public void setNome(String name){
   
   nome = name;
   }
   
   public String getLogin(){
   
   return login;
   }
   
   public void setLogin(String log ){
   
   login = log;
   }
   
   public String getCargo(){
   
   return cargo;
   }
   
   public void setCargo(String car){
   
   cargo = car;
   }
   
   
   
}
