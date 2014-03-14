ToolsTest
=========

Used as a sample project to demonstrate how PMD works.

Use 'mvn pmd:check' to execute PMD.

This will build successfully. If you want to make it fail, just add a private global variable to App.java. For example make it like this.

public class App {

    private String name;

    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}

Now PMD will detect String name as a dead variable (Unused variable) and make the build fail.
