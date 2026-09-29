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

### Homework4
```java
public class Homework4 {
    public static void main(String[] args) {
        for (int i = 1; i <= 9; i++) {
            for (int j = 1; j <= 9; j++) {
                System.out.printf("%d*%d=%-2d  ", j, i, (j * i));
            }
            System.out.println();
        }
    }
}
```
<img width="1282" height="420" alt="스크린샷 2026-09-28 004005" src="https://github.com/user-attachments/assets/e85deafc-f81d-409e-9804-11c682af02ab" />

### Homework5
```java
public class Homework5 {
    public static void main(String[] args) {
        
        double pi1 = 0.0;
        int sign = 1;
        for (int k = 0; k < 1000000; k++) {
            pi1 += sign * (4.0 / (2 * k + 1));
            sign *= -1; 
        }
        System.out.println("Gregory–Leibniz series: " + pi1);

        
        double sum = 0.0;
        for (int k = 0; k < 10; k++) {
            double term = Math.pow(-1.0 / 3.0, k) / (2 * k + 1);
            sum += term;
        }
        double pi2 = Math.sqrt(12) * sum;
        System.out.println("Madhava series: " + pi2);
    }
}
```
<img width="890" height="266" alt="image" src="https://github.com/user-attachments/assets/5dafee22-0f50-4a9f-a534-6afba01fb6cb" />



### Homework6
```java

public class Homework6 {
	 public static void main(String []args){
		 int rows =7;
		 int[][] binomial = new int[rows][];
		 
		 for (int i =0; i < rows; i++) {
			 binomial[i] = new int[i + 1];
			 binomial[i][0] = 1;
			 binomial[i][i] = 1;
			 
			 for (int j = 1; j < i; j++) {
				 binomial[i][j] = binomial[i -1][j - 1] + binomial[i-1][j];
			 }
		 }
		 
		 for (int i = 0; i < rows; i++) {
			 for (int j =0; j <= i; j++) {
				 System.out.print(binomial[i][j] + " ");
			 }
			 System.out.println();
		 }
	 }

}
```
<img width="424" height="206" alt="스크린샷 2026-09-28 142458" src="https://github.com/user-attachments/assets/626f7db7-3424-4c75-ae1a-9b60228332fa" />

### Homework7
```java

public class Homework7 {
	public static void main(String[] args) {
		int data[] = new int[20];
		
		for (int i =0; i < 20; i++) {
			data[i] = (int) (Math.random() *100);
		}
		
		for (int i =0; i <19; i++) {
			for (int j = i + 1; j < 20; j++) {
				if (data[i] > data[j]) {
					int temp = data[i];
					data[i] = data[j];
					data[j] = temp;
				}
			}
		}
		
		for (int i =0; i < 20; i++) {
			System.out.println(data[i]);
		}
		
	}
}
```
<img width="648" height="375" alt="스크린샷 2026-09-29 155312" src="https://github.com/user-attachments/assets/9eda753f-73eb-4711-8a3d-ff5975cf025a" />

