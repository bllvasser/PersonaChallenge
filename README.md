# PersonaChallenge
package academy.learnprogrmming;

public class Persona {
    String firstName;
    String lastName;
    int age;

    public String getFirstName() {
        return firstName;
    }

    public void setFirstName(String firstName) {
        this.firstName = firstName;
    }
    public String getLastName() {
        return lastName;
    }
    public void setLastName(String lastName) {
        this.lastName = lastName;
    }
    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
        if(age < 0 || age > 100) {
            age = 0;
        }
    }
    public boolean isTeen(){
        if(age > 12 && age < 20) {
            return true;
        }
        return false;
    }
    public String getFullName() {
        lastName.isEmpty();
        firstName.isEmpty();
        return firstName + lastName;

    }
}
package academy.learnprogrmming;

public class Main {

    public static void main(String[] args) {

        Persona persona = new Persona();
        persona.setFirstName("");
        persona.getFirstName();
        persona.setLastName("");
        persona.getLastName();
        persona.setAge(10);
        persona.getAge();
        System.out.println(" fullName= " + persona.getFullName());
        System.out.println(" teen= " + persona.isTeen());
        persona.setFirstName("John");
        persona.getFirstName();
        persona.setAge(18);
        persona.getAge();
        System.out.println(" fullName = " + persona.getFullName());
        System.out.println(" teen = " + persona.isTeen());
        persona.setLastName(" Smith ");
        persona.getLastName();
        System.out.println(" fullName = " + persona.getFullName());

    }
}
"C:\Program Files\Java\jdk-15.0.1\bin\java.exe" "-javaagent:C:\Users\nadiy\OneDrive\Desktop\IntelliJ IDEA Community Edition 2020.2.3\lib\idea_rt.jar=51690:C:\Users\nadiy\OneDrive\Desktop\IntelliJ IDEA Community Edition 2020.2.3\bin" -Dfile.encoding=UTF-8 -classpath C:\Users\nadiy\IdeaProjects\PersonChallenge\out\production\PersonChallenge academy.learnprogrmming.Main
 fullName= 
 teen= false
 fullName = John
 teen = true
 fullName = John Smith 

Process finished with exit code 0

