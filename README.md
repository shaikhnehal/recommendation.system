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

