# Create-menubar-in-java

package practise1;
import javax.swing.*;
import java.awt.event.*;

public class JMenuBar1 extends JFrame implements ActionListener
{
  JMenuBar menubar;
  JMenu menu1,menu2,menu3;
  JMenuItem menuItem1,menuItem2,menuItem3,menuItem4,menuItem5,menuItem6,menuItem7,menuItem8,menuItem9,menuItem10,menuItem11;
  JMenuBar1()
  {
   setLayout(null);
   menubar=new JMenuBar();
   menu1=new JMenu("File");
   menu2=new JMenu("Edit");
   menu3=new JMenu("View");
   
   menuItem1=new JMenuItem("New Project");
   menuItem2=new JMenuItem("New File");
   menuItem3=new JMenuItem("Open Project");
   menuItem4=new JMenuItem("Undo");
   menuItem5=new JMenuItem("Cut");
   menuItem6=new JMenuItem("Copy");
   menuItem7=new JMenuItem("Paste");
   menuItem8=new JMenuItem("Delete");
   menuItem9=new JMenuItem("Editor");
   menuItem10=new JMenuItem("Split");
   menuItem11=new JMenuItem("Code Folder");
   
   menu3.add(menuItem9);
   menu3.add(menuItem10);
   menu3.add(menuItem11);
   
   menu1.add(menuItem1);
   menu1.add(menuItem2);
   menu1.add(menuItem3);
   //menu1.add(menu3);
   
   menu2.add(menuItem4);
   menu2.add(menuItem5);
   menu2.add(menuItem6);
   menu2.add(menuItem7);
   menu2.add(menuItem8);
   menubar.add(menu1);
   menubar.add(menu2);
   menubar.add(menu3);
   
   setJMenuBar(menubar);
   menuItem1.addActionListener(this);
   menuItem2.addActionListener(this);
   menuItem3.addActionListener(this);

   setSize(500,500);
   setVisible(true);
  }
  public void actionPerformed(ActionEvent e)
  {
   if(e.getSource()==menuItem1)
   {
    JOptionPane.showMessageDialog(null,"Youclicked\""+menuItem1.getText()+"\"");
   }
   else if(e.getSource()==menuItem2)
   {
    JOptionPane.showMessageDialog(null,"Youclicked\""+menuItem2.getText()+"\"");
   }
   else if(e.getSource()==menuItem3)
   {
    JOptionPane.showMessageDialog(null,"youclicked\""+menuItem3.getText()+"\"");
   }
  }
  public static void main(String args[])
  {
    JMenuBar1 obj=new JMenuBar1();
  }
}
## output:-
if you click any menu then got some more option.......
![image](https://user-images.githubusercontent.com/96234273/180630553-fe5eed3e-1641-4025-8961-cb3667eee585.png)
