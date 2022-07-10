# Kullanici-Giri-i
www.patika.dev Kullanici girisi basit



        import java.util.Scanner;
        public class kullanici {
        public static void main(String[] args) {
        String username, password, yenigiris1;
        System.out.println("Lutfen Kullanici Adinizi Girin:");
        Scanner name = new Scanner(System.in);
        username = name.nextLine();
        System.out.println("Lutfen Sifrenizi Girin:");
        Scanner pass = new Scanner(System.in);
        password = pass.nextLine();
        if (username.equals("sinan") && password.equals("123456")) {
            System.out.println("Giris Yapildi");
        } else {
            System.out.println("Hatali Bilgiler");
            System.out.println("Sifrenizi Sifirlamak Ister misiniz? Birini yazin 'evet' ya da 'hayir'");
            Scanner select = new Scanner(System.in);
            String durum = select.nextLine();
            if (durum.equals("evet")) {
                System.out.println("Lutfen Yeni Sifrenizi Giriniz:");
                Scanner yenigiris2 = new Scanner(System.in);
                yenigiris1 = yenigiris2.nextLine();
                if (yenigiris1.equals("123456") || (yenigiris1.equals(password))) {
                    System.out.println("Yeni sifre olusmadi tekrar deneyiniz");
                } else {
                    System.out.println("Yeni Sifre Olusturuldu");
                    }
            }
        }
        }
    }
