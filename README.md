import java.util.Scanner;
class main{
  public static void main(String[]arggs){
 Scanner calculator = new Scanner(System.in);

    System.out.printf("Enter first number: ");
    double num1 = calculator.nextDouble();
    calculator.nextLine();

    System.out.printf("Enter second number: ");
    double num2 = calculator.nextDouble();

    System.out.printf("What operations do you want to perform? ");
    String oper = calculator.nextLine();

    if(oper.equals("sum")){
    System.out.printf("%f + %f = %f", num1, num2, num1+num2);
    } else if(oper.equals("sub")){
      System.out.printf("%f - %f = %f", num1, num2, num1-num2);
    } else if(oper.equals("mul")){
      System.out.printf("%f * %f = %f", num1, num2, num1*num2);
    }else if(oper.equals("div")){
                if(num2==0){
                  System.out.printf("NOT DEFINED");
                } else{
      System.out.printf("%f / %f = %f", num1, num2, num1/num2);
        } 
    } else {
    System.out.printf("INVALID OPERATION");
  }
    calculator.close();
    
  }
}
