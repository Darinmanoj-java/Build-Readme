# URL Manager

URL Manager is a Java application for managing URLs and their associated data.

## Requirements
- Java 18 or higher
- JUnit 5 library added to the build path for testing

## Usage
1. **Extract the ZIP file:**
   - Extract the contents of the ZIP file received via email to a directory on your computer.
2. **Open the project in your Java IDE:**
   - Open your preferred Java IDE (Integrated Development Environment) such as IntelliJ IDEA, Eclipse, or NetBeans.
3. **Import the project:**
   - Import the extracted project folder into your IDE using the "Import" or "Open Project" option.
4. **Add the JUnit 5 library to the build path:**
   - Download the JUnit 5 JAR files or add JUnit 5 dependencies to your build configuration.
   - Include the JUnit 5 JAR files in the build path of your project.
5. **Run the Main class:**
   - Open the `Main.java` file located in the `codingchallenge.main` package.
   - Run the main method to start the URL Manager application.
   - Follow the command-line prompts to add, remove, export statistics, or exit the application.

## Testing
The project includes unit tests using JUnit 5. To run the tests:
1. **Open the `URLManagerTest.java` file** located in the `codingchallenge.test` package.
2. Right-click on the file and select **"Run As" > "JUnit Test"** (or equivalent option based on your IDE).

## Future/production Enhancements 
1. **Domain Extraction Robustness:**
   - Currently, the code accepts URLs with standard formats like `https://www.example.com`. However, it does not handle URLs that include ports (e.g., `http://localhost:8080`), authentication info, etc. Consider extending the functionality to accommodate these scenarios.
   
2. **Handling of Similar Domains:**
   - The code does not currently account for subdomains or different top-level domains (TLDs) that could technically be part of the same "domain" in a broader sense. Adjust the code to consider these scenarios, for example, `sub.example.com` and `example.com`, or `example.com` and `example.org`, should be treated as the same entity.

3. **Allow Adding Existing URLs with Updated Social Scores:**
   - Users should be allowed to add existing URLs again, but the social score will be updated to the new score provided by the user.
