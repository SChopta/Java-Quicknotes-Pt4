//GETTERS AND RETURN VALUES
//2 ways: Follow A and B for 1st way
//STEP 1 and 2 for 2nd way

//claim the variable for example int Age= 18 (*claim get and return in the same cluster)
//use get ___()  ex. getAge() will get return age which will find the variable assigned 
/*For example:
int getAge() { return age;} will get the value from int Age=18 which is redirected to
int age = person1.getAge(); basically is a trail pointing to original variable age=18. Sysout can print this value
*/
class Person{
	String name;
	int age;
	void speak() {
		System.out.println("My name is: " + name);
	}
	void calculateYearsToRetirement() {// A. claim void and the method
		int yearsLeft = 65 - age;
		System.out.println(yearsLeft);//comment this out for alternative method
		
		//ALTERNATIVE METHOD
		//STEP1: return yearsLeft;
		
	}
}


public class App {

	public static void main(String[] args) {
		Person person1 = new Person();
		
		person1.name = "Joe";
		person1.age = 25;
		
		person1.speak();
		person1.calculateYearsToRetirement();//B. call the void method to do the calculation
		//STEP 2: int years = person1.calculateYearsToRetirement();
		// System.out.println("Years till retirements " + years);
	}

}
//alternatively you can set the initial return value then set the method to the variable which will redirect to the return value 
//and you can print out this value to get the same result.
