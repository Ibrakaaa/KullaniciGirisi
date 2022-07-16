# KullaniciGirisi
### Java-101 Kullanıcı Girişi Dersi
(www.patika.dev)

import java.util.Scanner;
public class KullaniciGirisi {
    public static void main(String[] args) {

        String kadi,sifre,yeniSifre;
        int secim;

        Scanner bilgi = new Scanner(System.in);
        System.out.print("Lütfen Kullanıcı Adınızı Giriniz: ");
        kadi = bilgi.nextLine();
        System.out.print("Lütfen Şifrenizi Giriniz: ");
        sifre = bilgi.nextLine();

        if(kadi.equals("patikadev")&&(sifre.equals("12345"))){
            System.out.print("Başarılı Bİr Şekilde Giriş Yaptınız.");

        }else{
            System.out.println("Bilgilerinizden Biri Yanlış!!!");
            System.out.println("Şifrenizi Değiştirmek İSter Misiniz?\n1-Evet\n2-Hayır");

            secim = bilgi.nextInt();

            if(secim==1){
                System.out.print("Lütfen Yeni Şifrenizi Giriniz: ");
                yeniSifre = bilgi.next();
                if(yeniSifre.equals("12345")){
                    System.out.print("Yeni Şifreniz Eskisiyle Aynı Olamaz!!!");

                }else{
                    System.out.print("Şifreniz Başarıyla Değiştirildi.");
                }

            }else{
                System.out.println("Programa Girişiniz Yapılamadı");
            }
            }


        }


        }








