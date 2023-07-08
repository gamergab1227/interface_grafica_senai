# interface_grafica_senai
package formulario_java_DB;

import java.awt.EventQueue;

import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.border.EmptyBorder;
import javax.swing.JLabel;
import javax.swing.SwingConstants;
import javax.swing.ImageIcon;
import java.awt.Color;
import java.awt.Panel;
import javax.swing.JInternalFrame;
import java.awt.SystemColor;
import javax.swing.Box;
import java.awt.Font;
import javax.swing.JButton;
import javax.swing.JComboBox;
import javax.swing.DefaultComboBoxModel;

public class site_do_senai extends JFrame {

	private JPanel contentPane;
	private JPanel panel_2;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					site_do_senai frame = new site_do_senai();
					frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the frame.
	 */
	public site_do_senai() {
		setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		setBounds(100, 100, 1451, 1309);
		contentPane = new JPanel();
		contentPane.setBackground(Color.DARK_GRAY);
		contentPane.setBorder(new EmptyBorder(5, 5, 5, 5));

		setContentPane(contentPane);
		contentPane.setLayout(null);
		
		JButton btnNewButton_2 = new JButton("Prosseguir");
		btnNewButton_2.setFont(new Font("Arial Black", Font.PLAIN, 14));
		btnNewButton_2.setForeground(Color.WHITE);
		btnNewButton_2.setBackground(Color.DARK_GRAY);
		btnNewButton_2.setBounds(782, 874, 147, 29);
		contentPane.add(btnNewButton_2);
		
		JComboBox comboBox = new JComboBox();
		comboBox.setFont(new Font("Arial Black", Font.BOLD, 14));
		comboBox.setForeground(Color.WHITE);
		comboBox.setBackground(Color.DARK_GRAY);
		comboBox.setModel(new DefaultComboBoxModel(new String[] {"manhã", "tarde", "noite"}));
		comboBox.setBounds(671, 783, 358, 55);
		contentPane.add(comboBox);
		
		JButton btnNewButton_1 = new JButton("Sair.");
		btnNewButton_1.setForeground(Color.WHITE);
		btnNewButton_1.setBackground(Color.DARK_GRAY);
		btnNewButton_1.setFont(new Font("Arial Black", Font.BOLD, 14));
		btnNewButton_1.setBounds(77, 354, 147, 55);
		contentPane.add(btnNewButton_1);
		
		JLabel lblNewLabel_6 = new JLabel("Sair?");
		lblNewLabel_6.setHorizontalAlignment(SwingConstants.CENTER);
		lblNewLabel_6.setFont(new Font("Arial Black", Font.BOLD, 20));
		lblNewLabel_6.setBounds(41, 288, 224, 55);
		contentPane.add(lblNewLabel_6);
		
		JLabel lblNewLabel_5 = new JLabel("Alterar senha?");
		lblNewLabel_5.setFont(new Font("Arial Black", Font.BOLD, 20));
		lblNewLabel_5.setHorizontalAlignment(SwingConstants.CENTER);
		lblNewLabel_5.setForeground(Color.BLACK);
		lblNewLabel_5.setBackground(Color.DARK_GRAY);
		lblNewLabel_5.setBounds(37, 156, 228, 36);
		contentPane.add(lblNewLabel_5);
		
		JButton btnNewButton = new JButton("Alterar senha.");
		btnNewButton.setForeground(Color.WHITE);
		btnNewButton.setFont(new Font("Arial Black", Font.BOLD, 14));
		btnNewButton.setBackground(Color.DARK_GRAY);
		btnNewButton.setBounds(77, 199, 147, 55);
		contentPane.add(btnNewButton);
		
		JLabel lbllaboratorio = new JLabel("LABORATÓRIOS ");
		lbllaboratorio.setBounds(704, 345, 287, 72);
		contentPane.add(lbllaboratorio);
		lbllaboratorio.setFont(new Font("Arial Black", Font.BOLD | Font.ITALIC, 30));
		lbllaboratorio.setHorizontalAlignment(SwingConstants.CENTER);
		lbllaboratorio.setForeground(Color.WHITE);
		lbllaboratorio.setBackground(Color.DARK_GRAY);
		
		JLabel lblNewLabel_2 = new JLabel("");
		lblNewLabel_2.setIcon(new ImageIcon("C:\\Users\\lab-41-p07\\Pictures\\laboratorio do senai para projeto.jpg"));
		lblNewLabel_2.setBounds(671, 408, 358, 289);
		contentPane.add(lblNewLabel_2);
		
		JLabel lblNewLabel_4 = new JLabel("NDPQ");
		lblNewLabel_4.setHorizontalAlignment(SwingConstants.CENTER);
		lblNewLabel_4.setBounds(41, 60, 234, 36);
		contentPane.add(lblNewLabel_4);
		
		JLabel lblNewLabel_3 = new JLabel("USUÁRIO");
		lblNewLabel_3.setFont(new Font("BankGothic Md BT", Font.BOLD | Font.ITALIC, 40));
		lblNewLabel_3.setHorizontalAlignment(SwingConstants.CENTER);
		lblNewLabel_3.setBounds(31, 11, 252, 72);
		contentPane.add(lblNewLabel_3);
		
		JPanel panel = new JPanel();
		panel.setBounds(0, 0, 308, 1061);
		panel.setBackground(Color.GRAY);
		contentPane.add(panel);
		
		JLabel lblSenai = new JLabel("");
		lblSenai.setBounds(596, 24, 444, 113);
		contentPane.add(lblSenai);
		lblSenai.setIcon(new ImageIcon("C:\\Users\\lab-41-p07\\Pictures\\logo so senai.png"));
		lblSenai.setToolTipText("");
		
		panel_2 = new JPanel();
		panel_2.setBackground(Color.GRAY);
		panel_2.setBounds(457, 81, 744, 225);
		contentPane.add(panel_2);
		
		JPanel panel_1 = new JPanel();
		panel_1.setBackground(Color.GRAY);
		panel_1.setBounds(661, 325, 379, 620);
		contentPane.add(panel_1);
	}
}
