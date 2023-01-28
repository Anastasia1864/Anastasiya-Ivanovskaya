//My-code_future_IVANOVSKAYA_ANASTASIA
  public class Main
 {


     public static void main (String arg[])
     {


        double start_price = 1000;
        double skidka = 1.05;
        double month = 2500;
        //double with_skidka = (((((start_price*skidka)*skidka+month)*skidka+month)*skidka+month)*skidka+month);
        double result = start_price*skidka+month; //считаем за 1-ый месяц уже этот результат
        int i = 1;
        while (result<=14000){
            result = result*skidka+month; 
            //полученное значение умножаем на ту же ежемесячную скидку и 
            //прибавляем степендию с ее постоянным значением. 
            //и при выполнении каждого последующего вычисления мы прибавляем +1 месяц. 
            //до тех пор, пока выражение перестанет быть истинным.
            i++;
            
        }
        System.out.print ("За "+i+" месяцев можно накопить на телеcкоп (при условии что напопления в банке хранятся под 5% в месяц).");

     }
 	}
