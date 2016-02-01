/**
 * AddressScreen.java
 *
 * version:
 *    $Id: AddressScreen.java,v 1.2 2013/11/26 20:22:41 bj8649 Exp bj8649 $
 *
 * revision:
 *    $Log: AddressScreen.java,v $
 *    Revision 1.2  2013/11/26 20:22:41  bj8649
 *    Code complete and tested
 *
 *    Revision 1.1  2013/11/21 23:19:29  bj8649
 *    Initial revision
 *
 *
 * @author: Brandon James
 */

import javax.swing.*;
import java.awt.*;

public class AddressScreen extends JFrame{

    public AddressScreen(){
        //create container for content pane
        Container container = getContentPane();
        container.setLayout(new BorderLayout());

        //set up panel to hold address info
        JPanel panel1 = new JPanel();
        panel1.setLayout(new GridLayout(5, 2));

        //create labels for address info, followed by text fields
        JLabel label = new JLabel("Name");
        panel1.add(label);
        panel1.add(new JTextField());
        label = new JLabel("Address");
        panel1.add(label);
        panel1.add(new JTextField());
        label = new JLabel("City");
        panel1.add(label);
        panel1.add(new JTextField());
        label = new JLabel("State");
        panel1.add(label);
        panel1.add(new JTextField());
        label = new JLabel("Zip");
        panel1.add(label);
        panel1.add(new JTextField());

        //create new panel for buttons, create each button
        JPanel panel2 = new JPanel(new FlowLayout());
        JButton button1 = new JButton("Add");
        panel2.add(button1);
        JButton button2 = new JButton("Modify");
        panel2.add(button2);
        JButton button3 = new JButton("Delete");
        panel2.add(button3);

        //add info panel to top of container and button panel 
        //bottom of panel
        container.add(panel1, BorderLayout.NORTH);
        container.add(panel2, BorderLayout.SOUTH);
        
    }//constructor

    //main method creates the specified window
    public static void main(String args[]){
        AddressScreen frame = new AddressScreen();
        frame.setTitle("Address Information");
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setSize(320, 190);
        frame.setLocation(100, 100);
        frame.setVisible(true);
    }//main
}//AddressScreen
