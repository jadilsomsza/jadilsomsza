public class IncrementNumbers {
    public static void main(String[] args) {
        if (args.length != 2) {
            System.out.println("Por favor, forneça exatamente dois números inteiros como argumentos.");
            return;
        }

        try {
            int num1 = Integer.parseInt(args[0]);
            int num2 = Integer.parseInt(args[1]);

            if (num1 <= num2) {
                for (int i = num1; i <= num2; i++) {
                    System.out.print(i + " ");
                }
            } else {
                for (int i = num1; i >= num2; i--) {
                    System.out.print(i + " ");
                }
            }
        } catch (NumberFormatException e) {
            System.out.println("Os argumentos fornecidos não são números inteiros válidos.");
        }
    }
}

