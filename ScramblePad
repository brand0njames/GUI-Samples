/**
 * ScramblePad.java
 *
 * version:
 *    $Id: ScramblePad.java,v 1.2 2013/11/26 21:22:59 bj8649 Exp bj8649 $
 *
 * revision:
 *    $Log: ScramblePad.java,v $
 *    Revision 1.2  2013/11/26 21:22:59  bj8649
 *    Code complete and tested
 *
 *    Revision 1.1  2013/11/26 21:16:28  bj8649
 *    Initial revision
 *
 *
 * @author: Brandon James
 */

import javax.swing.*;
import java.awt.*;

public class ScramblePad extends JFrame{

    public ScramblePad(){
        //create container for content pane
        Container container = getContentPane();
        container.setLayout(new BorderLayout());

        //set up panel to hold the scramble pad buttons
        JPanel panel1 = new JPanel();
        panel1.setLayout(new GridLayout(4, 3));

        //add buttons 1-9
        for(int i=1; i<10; i++){
            JButton button = new JButton(""+i);
            button.setForeground(Color.YELLOW);
            button.setBackground(Color.BLACK);
            panel1.add(button);
        }
        
        //add the zero button between two blank buttons
        JButton button = new JButton();
        button.setBackground(Color.BLACK);
        panel1.add(button);
        button = new JButton("0");
        button.setForeground(Color.YELLOW);
        button.setBackground(Color.BLACK);
        panel1.add(button);
        button = new JButton();
        button.setBackground(Color.BLACK);
        panel1.add(button);

        //set up a second panel to hold the label
        JPanel panel2 = new JPanel(new BorderLayout());
        JLabel lockLabel = new JLabel("LOCKED", JLabel.CENTER);
        panel2.setBackground(Color.BLACK);
        lockLabel.setForeground(Color.RED);
        panel2.add(lockLabel);
        
        //set up a third panel to hold bottom buttons
        JPanel panel3 = new JPanel(new FlowLayout());
        panel3.setBackground(Color.BLACK);
        button = new JButton("Start");
        panel3.add(button);
        button = new JButton("Okay");
        panel3.add(button);

        //add all panels to the container
        container.add(panel2, BorderLayout.NORTH);
        container.add(panel1, BorderLayout.CENTER);
        container.add(panel3, BorderLayout.SOUTH);
    }//constructor

    //main method creates the specified window
    public static void main(String args[]){
        ScramblePad frame = new ScramblePad();
        frame.setTitle("DCS Scramble Pad");
        frame.setSize(200, 300);
        frame.setLocation(100, 100);
        frame.setVisible(true);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }//main
}//ScramblePad
