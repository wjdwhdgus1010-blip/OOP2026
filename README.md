# OOP2026
### Homework1
```java
public static void main(String[] args) {
        int i, j;
        
        for (i = 0; i < 10; i++) {
        
            for (j = 0; j <= i; j++) {
                System.out.print("#");
            }
            for (j = i; j < 10; j++) {
                System.out.print(" ");
            }
            
            System.out.print("   "); 

          
            for (j = i; j < 10; j++) {
                System.out.print("#");
            }
            for (j = 0; j <= i; j++) {
                System.out.print(" ");
            }

            System.out.print("   "); 
            
            for (j = 0; j < 9 - i; j++) {
                System.out.print(" ");
            }
            for (j = 0; j <= i; j++) {
                System.out.print("#");
            }

            System.out.print("   "); 

            
            for (j = 0; j < i; j++) {
                System.out.print(" ");
            }
            for (j = i; j < 10; j++) {
                System.out.print("#");
            }

            System.out.println();
    }
  }
}



```


### Homework2

