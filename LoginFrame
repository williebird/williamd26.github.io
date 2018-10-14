import java.awt.EventQueue;

import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JOptionPane;
import javax.swing.JTextField;
import javax.swing.JPasswordField;
import javax.swing.JButton;
import java.awt.event.ActionListener;
import java.awt.event.ActionEvent;

public class LoginFrame {

	private JFrame frame;
	private JTextField username;
	private JPasswordField passwordField;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					LoginFrame window = new LoginFrame();
					window.frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the application.
	 */
	public LoginFrame() {
		initialize();
	}

	/**
	 * Initialize the contents of the frame.
	 */
	private void initialize() {
		frame = new JFrame();
		frame.setBounds(100, 100, 450, 300);
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		frame.getContentPane().setLayout(null);
		
		JLabel lblUsername = new JLabel("Username");
		lblUsername.setBounds(46, 112, 131, 31);
		frame.getContentPane().add(lblUsername);
		
		JLabel lblPassword = new JLabel("Password");
		lblPassword.setBounds(46, 68, 131, 31);
		frame.getContentPane().add(lblPassword);
		
		username = new JTextField();
		username.setBounds(181, 68, 169, 31);
		frame.getContentPane().add(username);
		username.setColumns(10);
		
		passwordField = new JPasswordField();
		passwordField.setBounds(181, 112, 169, 31);
		frame.getContentPane().add(passwordField);
		
		JButton btnLogin = new JButton("Login");
		btnLogin.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				
				if(username.getText().equals("Antony") && passwordField.getText().equals("Antony"))
				{
					JOptionPane.showMessageDialog(frame, "Succesfully logged in");
					
					MainFrame Main= new MainFrame();
					Main.setVisible(true);
					
					
				}
				else
				{
					JOptionPane.showMessageDialog(frame, "Invalid Information!");
				}
				
			}
		});
		btnLogin.setBounds(181, 168, 169, 38);
		frame.getContentPane().add(btnLogin);
	}

}
