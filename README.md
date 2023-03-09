# Spring-Notes
This Repo Contain Spring framework important Notes
## What is software framework:<br>
مجموعه من ال tools  بنستخدمها عشان نعمل application  معين ولكن لازم تكون ليها شرطين لازم تكون مبنية على platform  معين زى java لازم تكون بتعمل implement  ال specification  لل platform  ده  امثلة لل frameworks  دى زى spring framework – hibernate 
## What is spring boot :<br>
  •	It’s open source java-based framework used to create micro Service applications (stand alone applications)<br>
  •	Spring boot is built on top of the spring framework and it removed a lot of XML configuration files or annotations to facilitate it’s features Spring boot is rubber from spring framework<br>
## why is spring boot :<br>
  •	It’s Auto configuration ( بيعمل  auto configuration لل  unit test وال  integration test<br>
  •	Standalone (embedded HTTP servers for test)<br>
## Spring boot Initializer
  •	Naming by convention (spring data jpa)<br>
  •	Stater POMS (spring-boot-starter-web) الحته دى بخصوص ال jars files هوا دخل ملفات كتير تحت dependency <br> 
<br>Note: spring-boot-starter-web contain the most important jars that belongs to my application so it should be in the first tag (parent tag) in pox.xml file
<br>Spring Initializer screenshot:
<p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/spring%20init.png" alt="Spring boot Initializer"></p>


## Important Annotations:
1.	@Autowired  <br>
  •	Used for dependency Injection
2.	@Bean  <br>
  •	Used in Methods level
  •	 Used for Register and configure spring beans into spring container
3.	@Component<br>
  •	Used in Class Level<br>
  •	Used for Register and configure spring beans into spring container<br>
  ### @Component tag  is parent for 3 another annotations
      i.	@Controller -- used in presentation layer (control http requests and responses) 
      ii.	@Service      -- used in Business layer
      iii.	@Repository -- used in presentation layer

 <p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/arc%201.png" alt="@Component  Arc"></p><br>
 
## Spring Boot Layers
<p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/arc%202.png" alt="@Component  Arc"></p><br>

## Spring Boot flow Architecture
<p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/arc%203.png" alt="@Component  Arc" 
style="background-color:white;" >
</p>
4.	@SpringBootApplication Equivalent to<br>
  •	ComponentScan<br> 
  •	@Configuration<br>
  •	@EnableAutoConfiguration<br>
<p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/annotations%201.png" alt="@Component  Arc"></p><br>
## Create DB Connection :<br>
Step 1 - Add dependency for your database connector to pom.xml<br>
<p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/DB%20connection%201.png" alt="@Component  Arc"></p><br>

Step 2 - Configure your connection to Your Database
 
<p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/DB%20connection%202.png" alt="@Component  Arc"></p><br>

## How to bulid Restful web services using GET Request
one of the main annotations in Spring MVC: @RequestMapping. Simply put, the annotation is used to map web requests to Spring Controller methods.
Ways to use RequestMapping  and send values<br>
1.	GET without passing value 
<p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/request%20mapping%201.png" alt="@Component  Arc"></p><br>

2.	GET with passing value<br>
      a.	Passing in path<br>
      b.	Passing using @RequestParam<br>
<p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/request%20mapping%202.png" alt="@Component  Arc"></p><br>

 
3.	Get put make value not required
 <p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/request%20mapping%203.png" alt="@Component  Arc"></p><br>

4.	Get put make the value is optional
 <p align="center"><img src="https://github.com/Mohamed-Hamdy/Spring-Notes/blob/Spring-Boot-Notes/images/request%20mapping%204.png" alt="@Component  Arc"></p><br>

