**Hesap Makinesi Programı**
---
---
Hesap makinesini __switch-case__ kullanarak programlanması.


---
___

[patika.dev linkim](https://app.patika.dev/betulozgen)

----

**Aynı kodun __else-if__ kullanılarak programlanması.**

---
    //Kullanıcıdan veri alabilmek için Scanner sınıfını dahil ediyoruz.
    import java.util.Scanner;
    public class Calculator {
    public static void main(String[] args) {

        //Kullanıcıdan alacağımız sayılar için değişken tanımladık.
        int number1,number2,select;

        //Scanner sınıfını tanımladık.
        Scanner input = new Scanner(System.in);

        //Kullanıcıdan sayıları istiyoruz.
        System.out.print("Please enter number1:");
        number1 = input.nextInt();

        System.out.print("Please enter number2:");
        number2 = input.nextInt();

        //Kullanıcının işlem seçimini sağlıyoruz.
        System.out.println("Please select an action\n1-Addition\n2-Subtraction\n3-Multiplication\n4-Dividing");
        System.out.println("Your select:");
        select = input.nextInt();

        //Hesaplama işlemleri if-else koşulları ile yaptırılıyor.
        if (select == 1){
            System.out.println("Addition: "+(number1 + number2));
        } else if (select == 2) {
            System.out.println("Subtraction: "+(number1 - number2));
        } else if (select == 3) {
            System.out.println("Multiplication: "+(number1 * number2));
        } else if (select == 4) {
            if( number2 != 0) {
                System.out.println("Dividing: " + (number1 / number2));
            }else {
                System.out.println("A number cannot be divided by 0");
            }
        }else {
            System.out.println("Please select valid option!");
        }
    }
    }
