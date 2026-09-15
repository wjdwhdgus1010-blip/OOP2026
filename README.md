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
<img width="621" height="355" alt="homework1" src="https://github.com/user-attachments/assets/34df3a55-b43e-4e17-af36-1af0bde63cab" />




### Homework2
```java
public static void main(String[] args) {
		int n = 20;
		int[] fib = new int[n];
		
		fib[0] = 1;
		fib[1] = 1;
		
		for (int i = 2; i < n; i++) {
			fib[i] = fib[i - 1] + fib[i - 2];
		}
		for (int i = 0; i < n; i++) {
			System.out.print(fib[i] + " ");
		}
	}
}
```
<img width="879" height="282" alt="homework2" src="https://github.com/user-attachments/assets/4ad0f87b-b977-4f78-8ea2-5107f23ba217" />



### Homework3
```java
public static void main(String[] agrs) {
		long a = 1;
		long b = 2;
		for (int i = 1; i <= 20; i++) {
			double ratio = (double) b / a;
			System.out.printf("%d/%d=%.2f%n",b, a, ratio);
			
			long temp = a + b;
			a = b;
			b = temp;
		}
	}

}
```
<img width="662" height="395" alt="image" src="https://github.com/user-attachments/assets/02f67f4f-8025-4e95-9d01-610d91000189" />
