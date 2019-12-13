import java.applet.Applet;
import java.awt.GridLayout;
import java.awt.Label;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.*;

public class appletnew extends Applet implements ActionListener
{
    TextField t1=new TextField();
    TextField t2=new TextField();
    TextField t3=new TextField();
    public appletnew()
    {
        setBackground(Color.BLACK);
        setForeground(Color.RED);
        Label l1=new Label("First Number:  ");
        Label l2=new Label("Second Number:  ");
        Label l3=new Label("Result:  ");
        setLayout(new GridLayout(3,3,3,1));
        add(l1);
        add(t1);
        add(l2);
        add(t2);
        add(l3);
        add(t3);
        t2.addActionListener(this);
    }
    public void actionPerformed(ActionEvent e)
    {
        t3.setText("Hello");
    }
}
