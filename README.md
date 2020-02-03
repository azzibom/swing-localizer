# Using

  - include library in your project
  - add ```swing_<lang>_<country>.properties``` file with your localization in ```resources``` folder in your project.
  - call static method ```localize``` from class ```SwingLocalizer```.
  
    Examples: 
    ```java
    import by.azzibom.utils.swing.SwingLocalizer;
    public class Main {
      static {
        SwingLocalizer.localize();
      }
      public static void main(String[] args) {
        // ...
      }
    }
    ```
    or
    ```java
    import by.azzibom.utils.swing.SwingLocalizer;
    public class Main {
      public static void main(String... args) {
        SwingLocalizer.localize();
        // ...
      }
    }
    ```

# Compile and packaging

  Using ```Maven```
    in project root directory
    execute ```mvn clean package```.
