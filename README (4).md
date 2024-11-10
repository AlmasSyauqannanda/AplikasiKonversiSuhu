
# Aplikasi Aplikasi Konversi Suhu
Aplikasi sederhana yang memungkinkan pengguna untuk melakukan konversi suhu dari satu satuan ke satuan lainnya, seperti dari Celsius ke Fahrenheit, atau sebaliknya.

# Deskripsi
Aplikasi Konversi Suhu ini dirancang untuk memudahkan pengguna dalam mengonversi suhu secara cepat dan akurat. Antarmuka pengguna yang sederhana membuat aplikasi ini sangat mudah digunakan, bahkan oleh pengguna yang baru mengenal teknologi.






## Features
- Input Suhu
Pengguna dapat memasukkan nilai suhu yang ingin dikonversi melalui kolom input.

- Pilihan Satuan Suhu
Aplikasi menyediakan menu dropdown untuk memilih satuan suhu (misalnya, Celsius, Fahrenheit, atau Kelvin).

- Tombol Konversi
Setelah memasukkan nilai dan memilih satuan suhu, pengguna dapat menekan tombol Konversi untuk mendapatkan hasilnya.

- Tombol Keluar
Aplikasi dilengkapi dengan tombol Keluar yang memungkinkan pengguna untuk menutup aplikasi dengan mudah.

## Teknologi yang Digunakan
- Bahasa Pemrograman: Java
- Framework GUI: Java Swing
- Komponen Utama:
JTextField untuk input suhu
JComboBox untuk memilih satuan suhu
JButton untuk tombol Konversi dan Keluar
JLabel untuk menampilkan hasil konversi
## Konvers Suhu
import javax.swing.JOptionPane;
public class KonversiSuhuFrame extends javax.swing.JFrame {

    /**
     * Creates new form KonversiSuhuFrame
     */
    public KonversiSuhuFrame() {
        initComponents();
    }

    /**
     * This method is called from within the constructor to initialize the form.
     * WARNING: Do NOT modify this code. The content of this method is always
     * regenerated by the Form Editor.
     */
    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        jPanel1 = new javax.swing.JPanel();
        jLabel1 = new javax.swing.JLabel();
        inputSuhuField = new javax.swing.JTextField();
        skalaComboBox = new javax.swing.JComboBox<>();
        konversiButton = new javax.swing.JButton();
        labelHasil = new javax.swing.JLabel();
        hasilLabel = new javax.swing.JLabel();
        jButton1 = new javax.swing.JButton();
        jLabel2 = new javax.swing.JLabel();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);

        jLabel1.setText("Masukan Suhu");

        inputSuhuField.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                inputSuhuFieldActionPerformed(evt);
            }
        });
        inputSuhuField.addKeyListener(new java.awt.event.KeyAdapter() {
            public void keyTyped(java.awt.event.KeyEvent evt) {
                inputSuhuFieldKeyTyped(evt);
            }
        });

        skalaComboBox.setModel(new javax.swing.DefaultComboBoxModel<>(new String[] { "Celsius", "Fahrenheit", "Reamur", "Kelvin" }));

        konversiButton.setText("Konversi");
        konversiButton.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                konversiButtonActionPerformed(evt);
            }
        });

        labelHasil.setText("Hasil Konversi");

        jButton1.setText("Keluar");
        jButton1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton1ActionPerformed(evt);
            }
        });

        javax.swing.GroupLayout jPanel1Layout = new javax.swing.GroupLayout(jPanel1);
        jPanel1.setLayout(jPanel1Layout);
        jPanel1Layout.setHorizontalGroup(
            jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(jPanel1Layout.createSequentialGroup()
                .addContainerGap(169, Short.MAX_VALUE)
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, jPanel1Layout.createSequentialGroup()
                        .addComponent(hasilLabel)
                        .addGap(83, 83, 83))
                    .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, jPanel1Layout.createSequentialGroup()
                        .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                            .addComponent(inputSuhuField, javax.swing.GroupLayout.PREFERRED_SIZE, 103, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING, false)
                                .addComponent(konversiButton, javax.swing.GroupLayout.Alignment.LEADING, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                                .addComponent(skalaComboBox, javax.swing.GroupLayout.Alignment.LEADING, 0, 103, Short.MAX_VALUE)
                                .addComponent(labelHasil, javax.swing.GroupLayout.Alignment.LEADING, javax.swing.GroupLayout.PREFERRED_SIZE, 95, javax.swing.GroupLayout.PREFERRED_SIZE)))
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                        .addComponent(jButton1)
                        .addContainerGap())))
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, jPanel1Layout.createSequentialGroup()
                .addGap(28, 28, 28)
                .addComponent(jLabel1)
                .addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE))
        );
        jPanel1Layout.setVerticalGroup(
            jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(jPanel1Layout.createSequentialGroup()
                .addContainerGap()
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(inputSuhuField, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jLabel1))
                .addGap(8, 8, 8)
                .addComponent(skalaComboBox, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(23, 23, 23)
                .addComponent(labelHasil)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(konversiButton)
                    .addComponent(jButton1))
                .addGap(29, 29, 29)
                .addComponent(hasilLabel)
                .addContainerGap(51, Short.MAX_VALUE))
        );

        jLabel2.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jLabel2.setText("Konversi Suhu ");

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(layout.createSequentialGroup()
                        .addGap(47, 47, 47)
                        .addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE))
                    .addGroup(layout.createSequentialGroup()
                        .addGap(60, 60, 60)
                        .addComponent(jLabel2)))
                .addContainerGap(58, Short.MAX_VALUE))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addContainerGap()
                .addComponent(jLabel2)
                .addGap(20, 20, 20)
                .addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addContainerGap(71, Short.MAX_VALUE))
        );

        pack();
    }// </editor-fold>                        

    private void inputSuhuFieldActionPerformed(java.awt.event.ActionEvent evt) {                                               
        // TODO add your handling code here:
    }                                              

    private void konversiButtonActionPerformed(java.awt.event.ActionEvent evt) {                                               
       try {
        // Mendapatkan nilai suhu dari input field
        double suhu = Double.parseDouble(inputSuhuField.getText());
        
        // Mendapatkan skala suhu dari combo box
        String skala = (String) skalaComboBox.getSelectedItem();
        
        // Variabel untuk menyimpan hasil konversi
        double hasil = 0;

        // Logika konversi berdasarkan pilihan skala
        switch (skala) {
            case "Celsius":
                hasil = (suhu * 9/5) + 32; // Celsius ke Fahrenheit
                hasilLabel.setText("Celsiust: " + hasil);
                break;
            case "Fahrenheit":
                hasil = (suhu - 32) * 5/9; // Fahrenheit ke Celsius
                hasilLabel.setText("Fahrenheit: " + hasil);
                break;
            case "Reamur":
                hasil = suhu * 4/5; // Celsius ke Reamur
                hasilLabel.setText("Reamur: " + hasil);
                break;
            case "Kelvin":
                hasil = suhu + 273.15; // Celsius ke Kelvin
                hasilLabel.setText("Kelvin: " + hasil);
                break;
            default:
                hasilLabel.setText("Skala tidak dikenali.");
                break;
        }
    } catch (NumberFormatException e) {
        hasilLabel.setText("Input tidak valid. Masukkan angka.");
    }
    }                                              

    private void inputSuhuFieldKeyTyped(java.awt.event.KeyEvent evt) {                                        
          char c = evt.getKeyChar();
    if (!Character.isDigit(c) && c != '.') {
        evt.consume(); // Hanya angka dan titik yang diterima
    }
    }                                       

    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
         int confirm = JOptionPane.showConfirmDialog(this, "Apakah Anda yakin ingin keluar?", "Konfirmasi Keluar", JOptionPane.YES_NO_OPTION);
    if (confirm == JOptionPane.YES_OPTION) {
        System.exit(0); // Keluar dari aplikasi
    }
    }                                        

    /**
     * @param args the command line arguments
     */
    public static void main(String args[]) {
        /* Set the Nimbus look and feel */
        //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code (optional) ">
        /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
         * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
         */
        try {
            for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                if ("Nimbus".equals(info.getName())) {
                    javax.swing.UIManager.setLookAndFeel(info.getClassName());
                    break;
                }
            }
        } catch (ClassNotFoundException ex) {
            java.util.logging.Logger.getLogger(KonversiSuhuFrame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(KonversiSuhuFrame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(KonversiSuhuFrame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(KonversiSuhuFrame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new KonversiSuhuFrame().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify                     
    private javax.swing.JLabel hasilLabel;
    private javax.swing.JTextField inputSuhuField;
    private javax.swing.JButton jButton1;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JLabel jLabel2;
    private javax.swing.JPanel jPanel1;
    private javax.swing.JButton konversiButton;
    private javax.swing.JLabel labelHasil;
    private javax.swing.JComboBox<String> skalaComboBox;
    // End of variables declaration                   
}

## Authors

- [@AlmasSyauqannanda](https://www.github.com/AlmasSyauqannanda)
