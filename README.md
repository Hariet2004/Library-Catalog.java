public class Library Catalog{
public stativ void main(Srrings[]args){
  Scanner scanner = new Scanner(System.in);

        System.out.println("Welcome to the Library Catalog Program!");

        // Input the number of books in the catalog
        System.out.print("Enter the number of books in the catalog: ");
        int numberOfBooks = scanner.nextInt();
        scanner.nextLine(); // Consume the newline character

        // Arrays to store book details
        int[] serialNumbers = new int[numberOfBooks];
        String[] titles = new String[numberOfBooks];
        String[] authors = new String[numberOfBooks];
        String[] publishers = new String[numberOfBooks];
        int[] years = new int[numberOfBooks];

        // Input details for each book
        for (int i = 0; i < numberOfBooks; i++) {
            System.out.println("\nEnter details for Book " + (i + 1) + ":");

            System.out.print("Serial Number: ");
            serialNumbers[i] = scanner.nextInt();
            scanner.nextLine(); // Consume the newline character

            System.out.print("Title: ");
            titles[i] = scanner.nextLine();

            System.out.print("Author: ");
            authors[i] = scanner.nextLine();

            System.out.print("Publisher: ");
            publishers[i] = scanner.nextLine();

            System.out.print("Year: ");
            years[i] = scanner.nextInt();
            scanner.nextLine(); // Consume the newline character
        }

        // Display the catalog
        System.out.println("\nLibrary Catalog:");
        for (int i = 0; i < numberOfBooks; i++) {
            System.out.println("Book " + (i + 1) + ":");
            System.out.println("Serial Number: " + serialNumbers[i]);
            System.out.println("Title: " + titles[i]);
            System.out.println("Author: " + authors[i]);
            System.out.println("Publisher: " + publishers[i]);
            System.out.println("Year: " + years[i]);
            System.out.println("---------------");
        }

        // Close the scanner
        scanner.close();
    }
}
