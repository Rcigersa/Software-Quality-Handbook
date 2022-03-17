# Coding Standards

<a href="https://i0.wp.com/blog.codacy.com/wp-content/uploads/2018/10/20181002_WhyCodingStandardsMatter.jpg?resize=750%2C400&ssl=1">
<img alt="Estimation Techniques" src="https://i0.wp.com/blog.codacy.com/wp-content/uploads/2018/10/20181002_WhyCodingStandardsMatter.jpg?resize=750%2C400&ssl=1" width="350">
</a>

## **What are coding standards?**
Coding standards are a set of rules or recommendations developed by specific industries for developers to follow in order to ensure their code is secure and reliable. [WordPress](https://codex.wordpress.org/WordPress_Coding_Standards), for example, an open-source content management system, has published coding standards handbooks for all the languages it supports, including PHP, CSS, HTML, and JavaScript.

## **Why do we have / follow coding standards?**
- The overall quality of the software improves if developers comply with the coding standards.
- All stakeholders, from project managers to end users, value software quality.
- Following coding standards increases the software's correctness, reliability, efficiency, security and stability in day to day operations. This will then further reduce the risk of code defects and bugs.
- If additional requirements or environments arise in the future, it also enhances maintainability, testability, and adaptability.
- Other developers will have to put in less effort to understand and modify your code and as a result it will positively affect, portability, interoperability, and reusability.

## **Coding standards practices**
### **Inform developers on coding standards**
It is important to explain to developers why they must comply with coding standards. Using coding standards, as previously stated, eliminates unwanted code behaviour and errors. Rather than asking a developer to perform something a certain way simply because it is the we do it or the right way, educate them on why and how to do it by providing instructional material and knowledge.

### **Deciding which coding standards are most suitable**
Choosing the right industry-recognized coding standards early on is crucial because the faster you implement the coding standard within your organisation, the faster your employees will be trained. No norm will have been formed, making defect avoidance easier.

### **Some common examples of coding standards**
#### **Indentation**
Indenting code using tabs or spaces produces a more logical structure. Readability, reusability, and maintainability all benefit from indentation.  

*Bad* - hard to read

```java
int number = getNumber();
if(number != 0)
{
if(number < 5) 
{
System.out.println("Number is less than 5");
}
else if (number > 5 )
{
System.out.println("Number is more than 5");
}
else 
{
System.out.println("Number is 5");
}
}
else
{
System.out.println("Number is 0");
}
```

*Good* - easy to read

```java
int number = getNumber();
if(number != 0){
    if(number < 5){
        System.out.println("Number is less than 5");
    } 
    else if (number > 5 ) {
        System.out.println("Number is more than 5");
    }
    else {
        System.out.println("Number is 5");
    }
}
else{
    System.out.println("Number is 0");
}
```

#### **Optimize space usage**
Reduce the size of files, enhance readability, make it easier to find bugs, and increase maintainability by removing unnecessary empty lines of code.  

*Bad* - uses 17 lines

```java
1.  int number = getNumber();
2.
3.  if(number < 5){
4. 
5.      System.out.println("Number is less than 5");
6.
7.  } 
8.  else if (number > 5 ) {
9.  
10.     System.out.println("Number is more than 5");
11.
12. }
13. else {
14.
15.     System.out.println("Number is 5");
16. 
17. }
```

*Good* - uses 11 lines

```java
1.  int number = getNumber();
2. 
3.  if(number < 5){
4.      System.out.println("Number is less than 5");
5.  } 
6.  else if (number > 5 ) {
7.      System.out.println("Number is more than 5");
8.  }
9.  else {
10.     System.out.println("Number is 5");
11. }
```

#### **Formatting code**
Consistency in styling is critical in all programming languages. Consistency is defined as making minimal to no changes to the format of the code. Developers who are used to a particular format may find it challenging to adjust to new coding standards. Formatting code may either make or break a system because it improves readability while also increasing the risk of bugs. For example, SQL statements must follow a specific structure, complex queries must be broken down into multiple lines of code, and query words must be capitalized.

#### **Naming conventions**
This is the most well known and widely used coding standard among developers. When the proper format, lowercase, uppercase, underscores, and hyphens are used, it is easier to recognise and use for example variable names, class names, folder names and method names. It is also very important for names to be self explanatory.  

*Bad* - we don't know what something respresents if the variable is declared separately in a class from the if statement

```java
int something = getSomething();

if(something < 5){
    System.out.println("Age is less than 5");
} 
else if (something > 5 ) {
    System.out.println("Age is more than 5");
}
else {
    System.out.println("Age is 5");
}
```

*Good* - we know age represents a persons age

```java
int age = getAge();

if(age < 5){
    System.out.println("Age is less than 5");
} 
else if (age > 5 ) {
    System.out.println("Age is more than 5");
}
else {
    System.out.println("Age is 5");
}
```

#### **Commenting**
Putting descriptions into computer programs is referred to as commenting. When you utilize comments in your code, you make it easier to maintain. If functions have a description of how they work, it is easier to find a way to reuse them. This also helps if the naming conventions coding standard is not followed and the name of something is not self explanatory.  

*Bad* - we don't know what number represents

```java
int number = getNumber();

if(number < 5){
    System.out.println("Age is less than 5");
} 
else if (number > 5 ) {
    System.out.println("Age is more than 5");
}
else {
    System.out.println("Age is 5");
}
```

*Good* - even though the word number is used we know from the comment it represents age

```java
//the number represents the age in this class
int number = getNumber();

if(number < 5){
    System.out.println("Age is less than 5");
} 
else if (number > 5 ) {
    System.out.println("Age is more than 5");
}
else {
    System.out.println("Age is 5");
}
```

## **For more information please visit the following online resources:**
[Coding Best Practices: How to Use Coding Standards](https://www.perforce.com/blog/qac/coding-best-practices-how-use-coding-standards)  
[Guide To WordPress Coding Standards](https://www.smashingmagazine.com/2012/07/guide-wordpress-coding-standards/)  
