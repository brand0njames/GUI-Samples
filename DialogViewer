/**
 * DialogViewer.java
 *
 * version:
 *    $Id: DialogViewer.java,v 1.2 2013/11/27 00:37:58 bj8649 Exp bj8649 $
 *
 * revision:
 *    $Log: DialogViewer.java,v $
 *    Revision 1.2  2013/11/27 00:37:58  bj8649
 *    Code complete and tested
 *
 *    Revision 1.1  2013/11/27 00:02:40  bj8649
 *    Initial revision
 *
 * @author: Brandon James
 */

import javax.swing.*;
import java.awt.*;

public class DialogViewer{

    //display a file chooser menu
    private JFileChooser fc = new JFileChooser();
    //display a dialog box
    private JOptionPane op = new JOptionPane();
    //selection for confirm dialog button press
    private int selection;

    //selects an action based on command line input
    //method will display either a file selection window,
    //a confirmation dialog box, or a message window
    private void actionSelect(String action){
        //displays file selection window when 'f' is input
        if(action.equals("f")){
            fc.showOpenDialog(null);

            //displays appropriate message if no file is selected
            if(fc.getSelectedFile() == null)
                System.out.println("No file selected.");
            else
                System.out.println(fc.getSelectedFile());
        }
        //displays confirmation window when 'c' is input
        else if(action.equals("c")){
            selection = op.showConfirmDialog(null, "Are you sure?");
            
            //displays which type of button was pressed
            switch(selection){
                case 0: System.out.println("Yes");
                        break;
                case 1: System.out.println("No");
                        break;
                case 2: System.out.println("Cancel");
                        break;
                default: System.out.println("Incorrect option");
            }
        }
        //displays message window when 'm' is input
        else if(action.equals("m")){
            op.showMessageDialog(null, "Brandon James");
        }
        //if input is invalid, error is displayed and program exits
        else{
            System.err.println("Incorrect command.");
            System.exit(0);
        }
    }

    //main method accepts a command line argument and displays
    //the appropriate dialog using the actionSelect command
    public static void main(String args[]){
        //program exits if number of command line args is incorrect
        if(args.length != 1){
            System.err.println("usage: java DialogViewer action-type");
            System.exit(0);
        }

        DialogViewer dv = new DialogViewer();
        String input = args[0];
        
        //selects dialog based on input
        dv.actionSelect(input);

        //exits program
        System.exit(0);
    }
}
