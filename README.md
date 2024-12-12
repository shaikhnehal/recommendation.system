/*Create a function which takes three numbers "A" , "B" , "N" as a parameter.
If the number N is 1 , ADD A and B
If the number N is 2, SUBTRACT B from A
If the number N is 3, MULTIPLY A and B
If the number N is 4 , DIVIDE B from A
if the given number "N"  is none from the above four numbers , return -1 */


public class problem_1 {
 public static int Homies(int A, int B, int N) {
        switch (N) {
            case 1:
                return A + B; 
            case 2:
                return A - B; 
            case 3:
                return A * B; 
            case 4:
                if (B != 0) {
                    return A / B; 
                } else {
                    throw new ArithmeticException("Division by zero is not allowed.");
                }
            default:
                return -1; 
        }
    }

    public static void main(String[] args) {
        
        System.out.println(Homies(10, 5, 1)); 
        System.out.println(Homies(10, 5, 2)); 
        System.out.println(Homies(10, 5, 3)); 
        System.out.println(Homies(10, 5, 4)); 
        System.out.println(Homies(10, 5, 0)); 
    }
}

