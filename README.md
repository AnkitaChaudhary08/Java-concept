# Java-concept

1.setup IDE(eclipse, intellij) 2.selenium(click,type,locator,dropdown,selection,pop-up page,scroll up,scroll down) 3.core java 4.Framework(cucumber(BDD),TestNg) 5.RestAssured(API Automation) 6.GIT (VCS)/Github 7.jenkins(CI/CD) 8.AWS (EC-2 instance)

------getting started-------- 1-downlaod the Selenium 2-Download JDK (go to the C drive and copy paste the Bin folder and Set the Variable) 3-java --version (if downloaded) 4-Maven download (rename the name like -maven) copy paste the C drive progrm files ) 5-click on the new in eclipse and search the Quickstart file its take some time to download) 6-after maven download see all the libraries of the maven 7-pom.xml (wee need to copy paste the Selenium libraries),,,search the maven repositories (serch-java maven) and copy paste the libraries) 8-first we have to create the package (rifht click on the project) 9-in package we have to create the class 10.in class we need to write the code in mian method

thread.sleep(3000) getText() driver.findElement(By.xpath) driver.quit->close the entire browser data driver.close->close the current tab data actions class->handle the click action class-context click,double click,drag and drop,mouse hover ,over windowobject->parent window,child window javascriprt executer->handle the pure click

window handle->handle the multipile tab getWindowHandle->return the string getwindowHandles->return the set of string

javascript pop-up-> alert() interface use krte hn ye inbuild method hota h 4- method

1-String getText(),2-dismiss(), 3-accept, 4-sendkeys

--navigate maethod --selenium --driver.navigate().back(); --thread.sleet(3000); --driver.navigate().forward(); --thread.sleep(3000); --driver.navigate().refresh(); --driver.navigate().to("url")

driver.navigate().back(); Thread.sleep(3000); driver.naviagte(). forward (); Thread.sleep(3000); driver.navigate.refresh(); Driver.navigate().To(url);

TestNG

Add dependcy (mvn repositories) Install plugin (help - eclipse work space search test ng)

Output report ..index.html

Method..(annotations) @Test (priority=0, description= "login" ) @Test (before method) @Test (after method)

user.properties(store the data with key n value) --------BDD _CUCUMBER----

File:-features(iske ander hm test case likhte hn gharkin keywords (given, when,then,and )with gharkin language or plain text) 1-login.feature 2-logout.feature

Every test case ko link krate hn method k saath jisko (stepdefinition file)bolte hn..

Dependencies-cucumber.io Plugin - natural

---cucumber layer---- 1- features file(iske ander hm test cases likhte hn) 2-stepdefinition file(test cases ko link krte hn method ke through or object bnate hn or call krate hn) 3-page (iske ander web elements or method likhte hn selenium ke )like logic likhte hn) 4-runner file (iske ander features ka path location provide krte hn , tags provide krte hn @smoke,@regression etc -plugin - ke ander report generate krte hn , glue ke ander step definitions file ka path location pass krte hn) basically ye execution file hoti hai..) ..

(.Test cases ke upper @regression @smoke likh dete hn)

--chrome options (incognito mode mai script ryn krte hn)(object bna do - Chromeoption option = new Chrome option (); option.chromeoptions(--incognito) -Firefox options ( -edgeootions

-automation hmesha regression testing ke liye use hota kch cheeze jha automate nhi chla skte - color ,font weight,suzey,barcody, captcha) -automation hmesha (n-1) sprint mai chlta h Like 20 sprint running h 19 sprint tk sb test cases regression hone chaiye

...... Surefire Master thought-plugin cucumber report generate Mvn clean Mvn clean install Mvn compile

--- drop-down --- Method-- Selectbyindex Selecrbyvalue Selectvyvisibletext --- windows handle -- method get.windowhandle

--prop.getproperty---

--static method of api rest assured--- --io.restassured --io.hemcrest.matchers

--isme hm body ,headera,res,req send krte hn

---cucumber ke through report generate krna-- 1- masterthought - dependencies add krni pdegi 2-surefire - dependencies add krni pdegi

Implicit wait Explicit wait -- assert - error msg k liye use krte hn

_Staleelement ko kaise handle karte hn

Try Catch Block se handle krte hn

-++ build tools+++ Maven Gradle Ant

---logging ke liye dependencies+++ --Log4j -> add krte hn Log4j.properties -> predefined code hota h copy paste krte hn ---cucumber ki site se ----++ Cucumber hooks ->

--apache poi --dependicies add krte hn excel se multupile user ka data read krne ke liye

Framework-> best practices (kisi bhi kaam ko krne ki) browser launch ka code hota h bs hme kisi ki bhi site ka url pass krna hota h or scenerio likhne hote hn)

Helper -<> webdriverhelper.java - isme hm generic method likhte hn

---workflow of automation--- code editor-> json wire protocol ->json ->chromedriver , firefoxdriver,edgedriver

class-> its a blueprint. its is a collection of data and we can pass the method and create the object inside the class,once class hold the multipile methoid method->its is a block of code and collection of the statement. we can perform any specific action inside the method object->its a real time entity, its show the behaviour of the class. we can create the object with the help of new keywords package->one package can hold the multipile class constructor->when we craete an object of the class then automatically initialized the constructor its called constrctor super->iits called the parent class constructor

string method-> equals contains startsWith endsWith Replace split toUpperCase toLowerCase length concat

primitive data type->int,char,double,float,byte,short,long non-primitive data type-arra,string,class

method overloading-> multiple methods can have the same name with different parameters:

assertion-> it is a condition that check if the given condition is true or false. if a condtition is ture then execution of the prgram will continue and if the condition is false then execution of programme will stop.

how to handle the alert in the automation->using alert interface-

how to take screenshot-_usinf takescreenshot iterafce->method->getScreenShotas()

getText()->return the visible text of the webelement getAttributes()->return the value of specific attributes of the webelement.

locator->find the location of particular webelement locator should be unique like one of one syntax of x-path->//tagname[@attribute='value']

Thread.sleep()->error throw nhi krta hai .explicit wait()->error throw krta hai

POM-> is a design pattern in Selenium that creates an object repository for storing all web elements. It helps reduce code duplication and improves test case maintenance. In Page Object Model, consider each web page of an application as a class file.

Exception in selenium-> checked exception->handling the during write the code uncheked exception->it is the runtime exception list of some exception-> 1-NoSuchElementException 2- NoSuchFrameException 3-NoSuchWindowException 4-NotFoundException: 5-ScreenshotException 6-timeout exception handle the exception-try,->block of code catch->handl the exception

finally->it is block that execute the important code its is like a connection closed.. throw->throw keyword is used to thrown an exception the throw are followed by instance and used with method we can not throw multipile exceptions

throws->the throws keyword is used to declare exception throws are followed by class and used with the method signature we can declare multipile exception

exception in java->ArithmeticException, FileNotFoundException, ArrayIndexOutOfBoundsException, SecurityException

abstract in java->abstract class is a restricted class that can not be used to create objects (to access it,it must be inherited from another class) the abstract keyword is a non-access modifier used for class and ,method

Abstraction ->>data abstraction is a process to hiding the internal details of the user and showing the essential information to the user. abstraction can be achieved with either abstract class or interface

Interface->>an interface in java is a blueprint of a class. It has static constants and abstract methods. It is used to achieve abstraction and multiple inheritance in Java.

Feature->Feature is a test script which has to be executed.

Scenario->Scenario describes the steps and expected outcome for a particular test case

Scenario outline->same scenario can be executed for multipile sets of data using scenario outline.

Example->data provide in the tabular format

why we use maven build-->Maven provides easy access to all the required information. Maven makes it easy for the developer to build a project in different environments.it is simple to add new dependencies

Cucumber->Cucumber is a testing tool based on Behavior Driven Development (BDD) framework. It is used to run functional tests written in plain text and develop test cases for software functionality.

Encapulation->The meaning of encapulation is to make sure that sensitive data is hidden from users. to achieve this you must--- 1-declare class var/attributes as private 2-provide public get and set methods to access and update the value of a private varaible

Polymorphism-->>its occurs when there are one or more classes or objects related to each other by inheritance. polymorphism means one name having multipile forms like-_man-Mman can be husband, son,employee etc

Types-->Compile time polymorphism->method overloading, operator overloading run time poly->method overriding, operator overidding

INHERITANCE-one class inherit from the another class with the help of extends keyword.

parent class having the method and attributes then access it by subclass it is called the inheritance ..it's use to reusability the code.

Type->single level-> class a, class b inherit from each other

multilevel->class a, class b, class c->inherit from each other

hierarchial->class a having two sub class ->class a->class b, class c

Hybrid-> class a inherit from class b or class c->class b or c inherit from class d -->not supporetd by java ->it ahndle by interface using implements keywords

Multipile-> class a or claas b inherit from class c->not supported by java->interface implemented

--static var---- ---Static keyword-> static variables gets memory only once during the class loading.its allocate memory only one times during class loading its is efficient for the memory and save times for the developers.

---non static variables->we need to create the obj of the non sttaic varaible and then call it.->it will get memeory everytime while obj is created of the class

-Final->final keyword is used with the classes, methods and variables --once declared final variable becomes constant and can not be modified. --final class can not be inherited

--finally-->finally is the block in java exception handling to execute the important code whether the exception occurs or not?

Finalize->Finalize is the method in java which is used to perform clean up processing just before object is garbage collected

Throwable-> throwable is a superclass for all types of errors and exceptions in java. this class is a member of java.lang package only.

This-> the this keyword refers to the current object in a method or constructor.

used--invoked current class constructor invoked current class method and pass an argument====
