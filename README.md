# ÖDEV
**Dersler:Matematik,Türkçe,Fizik,Kimya,Müzik;**
* Geçme Notu = 55
* Ödev: Eğer girilen notlar 0 ve 100 aralığında değilse ortalamaya katılmasın.

```
import java.util.Scanner;

public class SinifGecme {
    public static void main(String[] args) {
        int mat, turkce, fizik, kimya, muzik;
        Scanner input = new Scanner(System.in);

        System.out.println("-----Ders Notlarınızı Giriniz-----");
        System.out.print("Matematik :");
        mat = input.nextInt();
        System.out.print("Türkçe :");
        turkce = input.nextInt();
        System.out.print("Fizik :");
        fizik = input.nextInt();
        System.out.print("Kimya :");
        kimya = input.nextInt();
        System.out.print("Müzik :");
        muzik = input.nextInt();

        int i = 1, t = 0;
        if (0 <= mat && mat <= 100) {
            i++;
            t = t + mat;
        }
        if (0 <= turkce && turkce <= 100) {
            i = i + 1;
            t = t + turkce;
        }
        if (0 <= fizik && fizik <= 100) {
            i = i + 1;
            t = t + fizik;
        }
        if (0 <= kimya && kimya <= 100) {
            i = i + 1;
            t = t + kimya;
        }
        if (0 <= muzik && muzik <= 100) {
            i = i + 1;
            t = t + muzik;
        }

        double avarage = t / (i-1.0);


        if ((0 < avarage) && (avarage < 55)) {
            System.out.println("Sınıfı Geçemediniz.Seneye Tekrar Görüşmek Üzere !");
        } else if ((55 <= avarage) && (avarage <= 100)) {
            System.out.println("Tebrikleer Sınıfı Geçtiniz !");
        }
        System.out.print("Ortalamanız : " + avarage);
    }
}
```
# Patika Profilim
***
<a href="https://academy.patika.dev/profile">Patika Profilim</a>