String user="ADMIN";
        String pass="12345";

        String field1= jTextField1.getText();
        String field2=String.valueOf(jPasswordField1.getPassword());
        if(field1.equals(user) && field2.equals(pass)){

            Connexion.super.dispose();
            new Inscription().setVisible(true);
        }
        else
        {
            JOptionPane.showMessageDialog(this,"identifiant ou mot de passe incorrect");
        }
