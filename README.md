# Mukemmel-Sayi-Bulan-Program
Patika.dev > Java101 > Döngüler > Ödev2 - Mükemmel Sayı Bulan Program

## Klavyeden girilen bir sayının mükemmel sayı olup/olmadığını bulan ve sayı mükemmel sayı ise ekrana “mükemmel sayıdır.” değilse “mükemmel sayı değildir.” ifadelerini ekrana yazan programı Java dilinde yazınız.

### Mükemmel Sayı Nedir ?
Bir sayının kendisi hariç pozitif tam sayı çarpanları (kalansız bölen sayıların) toplamı kendisine eşit olan sayıya mükemmel sayı denir.


      import java.util.*;

      public class mukemmel_sayi {

        public static void main(String[] args) {

              Scanner sc = new Scanner(System.in);

              System.out.print("Enter a number: ");
              int n = sc.nextInt();

              int toplam = 0;
              for(int i=1; i < n; i++) {
                if(n % i == 0)
                  toplam += i;
              }
              
              if(n == toplam)
                System.out.println(n + " Mükemmel sayıdır.");

              else
                System.out.println(n + " Mükemmel sayı değildir.");
         }
      }
