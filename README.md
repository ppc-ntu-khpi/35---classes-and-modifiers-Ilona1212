Завдання 1
=====
## Customer
```
package domain;

public class Customer {
    private int ID = 1;
    private boolean isNew = true;
    private double total = 1000;
    
    public void displayCustomerInfo(){
        System.out.println("Customer ID: " + ID);
        System.out.println("Is new customer: " + isNew);
        System.out.println("Total purchases are: " + total);
    }
}
```
## CustomerTest
```
package test;

import domain.Customer;

public class CustomerTest {

    public static void main(String[] args){
    
        Customer c = new Customer();
        c.displayCustomerInfo();
    }
}
```
Фото виконання програми:

![](https://github.com/ppc-ntu-khpi/35---classes-and-modifiers-Ilona1212/blob/main/Solution/done.png?raw=true)


Завдання 2
=====
## Custome
```
package domain;

public class Customer{
  private int ID;
  private boolean isNew;
  private float total; 

  public Customer(){
    ID = 1;
    isNew = true;
    total = 1000.0F;
  }
  
  public void displayCustomerInfo(){
        System.out.println("Customer ID: " + ID);
        System.out.println("Is new customer: " + isNew);
        System.out.println("Total purchases are: " + total);

  public int getID() {
        return ID;
    }

    public void setID(int newID) {
        if(newID > 0)
            ID = newID;
        else
            ID = 0;
    }

    public boolean getStatus() {
        return isNew;
    }

    public void setStatus(boolean New) {
        isNew = New;
    }

    public double getTotal() {
        return total;
    }

    public void setTotal(double newTotal) {
        if(newTotal > 0)
            total = newTotal;
        else
            total = 0;
    }
}
}
```
## CustomeTest
```
package test;

import domain.Customer;

public class CustomerTest {

    public static void main(String[] args){
    
        Customer c = new Customer();
        c.setID(23);
        c.setStatus(false);
        c.setTotal(2113.34F);
        c.displayCustomerInfo();

    }
}
```
Фото виконання програми:

![](https://github.com/ppc-ntu-khpi/35---classes-and-modifiers-Ilona1212/blob/main/Solution/advanced.png?raw=true)

