# Spring-Java-Configurations
The central artifact in Spring's new Java-configuration support is the @Configuration-annotated class. These classes consist principally of @Bean-annotated methods that define instantiation, configuration, and initialization logic for objects that are managed by the Spring IoC container.

Annotating a class with the @Configuration indicates that the class can be used by the Spring IoC container as a source of bean definitions. The simplest possible @Configuration class would read as follows:

@Configuration
public class AppConfig {

}            
An application may use one @Configuration-annotated class, or many. @Configuration is meta-annotated as a @Component. Therefore, @Configuration-annotated classes are candidates for component-scanning and can also take advantage of @Autowired annotations at the field and method levels, but not at the constructor level. @Configuration-annotated classes must also have a default constructor. You can wire externalized values into @Configuration-annotated classes with the @Value annotation.
