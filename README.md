Spring-starter

#  1. Intro
=================

## 1. Введение

+ `Модули Spring (out of the box)`
+ `Удобство и простота использования`
+ ` Микросервисная архитектура`
+ `Support & Community`
+ `Что нужно знать для изучения курса Spring`


## 2. Установка программного обеспечения

+ `Установка Java 17`
+ `Установка IntelliJ IDEA Ultimate Edition`
+ `Установка PostgreSQL`
+ `Установка Docker`
+ `Создание нового проекта`
## 3. Inversion of Control. Dependency Injection

+ `Object Dependencies`
+ `Object Dependencies в коде`
+ `Inversion of Control & Dependency Injection`
+ `Inversion of Control & Dependency Injection в коде`
+ `3 способа внедрения зависимостей в объекте`


## 4. IoC Container

+ `Spring IoC Container`
+ `Bean`
+ `Bean Definition`
+ `POJO`
+ `Основные интерфейсы IoC Container`
+ `3 способа создания Bean Definitions`




# 2. XML-based Configuration


## 5. XML-based Configuration

+ `BeanFactory и ApplicationContext интерфейсы`
+ `ClassPathXmlApplicationContext`
+ `XML config`
+ `Идентификаторы (id) бинов как ключи в IoC Container`
+ `Алиасы бинов (alias)`

## 6. Constructor Injection

+ `Внедрение примитивных типов данных`
+ `Внедрение коллекций list/set`
+ `Внедрение ассоциативного массива map`
+ `Поле genericArgumentValues в BeanDefinition`
+ `Поле indexedArgumentValues в BeanDefinition`
+ `Указание атрибута type в параметрах конструктора`
+ `Указание атрибута name в параметрах конструктора`

## 7. Factory Method Injection

+ `Внедрение других бинов через ref*`
+ `Создание новое бина CompanyRepository`
+ `Внедрение зависимостей через factory method`
+ `Атрибут factory-bean (паттерн ServiceLocator)`

## 8. Property Injection

+ `Использование set* методов в ConnectionPool`
+ `Поле propertyValues в BeanDefinition`
+ `Упрощенный жизненный цикл бинов - Bean Lifecycle`
+ `Плюсы и минусы Constructor и Property Injections`
+ `Циклические зависимости через Property Injection`

## 9. Bean Scopes

+ `Common Bean Scopes`
+ `Custom Bean Scopes`
+ `Web Bean Scopes`
+ `Prototype Bean Scope`

## 10. Lifecycle Callbacks

+ `Измененный Bean Lifecycle`
+ `Initialization callbacks`
+ `Destruction callbacks`

## 11. Injection from Properties Files

+ `Зачем использовать properties files`
+ `Создание файла application.properties`
+ `PropertySourcesPlaceholderConfigurer bean`
+ `Expression Language (EL)`
+ `Spring Expression Language (SpEL)`
+ `SpEL документация`
+ `System properties`

## 12. BeanFactoryPostProcessor (BFPP)

+ `Интерфейс BeanFactoryPostProcessor`
+ `Как работает PropertySourcesPlaceholderConfigurer`
+ `Измененный Bean Lifecycle`
+ `Метод isAssignableFrom`

## 13. Custom BeanFactoryPostProcessor

+ `Создание собственных BeanFactoryPostProcessor`
+ `Интерфейс Ordered`
+ `Интерфейс PriorityOrdered`


# 3. Annotation-based Configuration

## 14. Annotation-based Configuration

+ `Подключение зависимости jakarta annotation api`
+ `Аннотации @PostConstruct и @PreDestroy`
+ `Класс CommonAnnotationBeanPostProcessor`
+ `context:annotation-config xml element`




## 15. BeanPostProcessor (BPP)

+ `Интерфейс BeanPostProcessor`
+ `Bean Lifecycle (final version)`
+ `Интерфейс Aware`
+ `Класс ApplicationContextAwareProcessor`


## 16. Custom BeanPostProcessor. Часть 1

+ `Создание своей аннотации @InjectBean`
+ `Создание InjectBeanPostProcessor`
+ `Утилитный класс ReflectionUtils`
+ `Тестирование InjectBeanPostProcessor`

## 17. Custom BeanPostProcessor. Часть 2
+ `Создание аннотации @Transaction`
+ `Создание CrudRepository`
+ `Создание TransactionBeanPostProcessor`
+ `Тестирование TransactionBeanPostProcessor`
+ `Корректируем TransactionBeanPostProcessor`
+ `Создание AuditingBeanPostProcessor`


## 18. @Autowired & @Value

+ `Аннотация @Autowired`
+ `Аннотация @Resource`
+ `Решение конлифкта бинов. @Qualifier`
+ `Collection injection`
+ `Properties injection. @Value`


## 19. Classpath Scanning
+ `context:component-scan. Аннотации @Component`
+ `Замена бинов из xml на @Component`
+ `Тестирование функционала`

## 20. Bean Definition Readers

+ `Component Scan classes`
+ `Bean Definition Readers`
+ `Класс ComponentScanBeanDefinitionParser`
+ `Класс AnnotatedBeanDefinitionReader`

## 21. Type Filters

+ `Атрибут annotation-config`
+ `Атрибут name-generator`
+ `Атрибут resource-pattern`
+ `Атрибут scoped-proxy`
+ `Атрибут scope-resolver`
+ `Атрибут use-default-filters`
+ `5 type filters`
+ `Custom filters`


## 22. @Scope
+ `Атрибут scope-resolver`
+ `Класс AnnotationScopeMetadataResolver`
+ `Аннотация @Scope`


## 23. JSR 250, JSR 330

+ `Аббревиатура JSR`
+ `JSR 250`
+ `JSR 330`
+ `Класс Jsr330ScopeMetadataResolver`



# 4. Java-based Configuration

## 24. Java-based Configuration
+ `Класс ConfigurationClassBeanDefinitionReader`
+ `Создание ApplicationConfiguration. @Configuration`
+ `Аннотация @PropertySource`
+ `Аннотация @ComponentScan`
+ `Класс AnnotationConfigApplicationContext`


## 25. @Import & @ImportResource
+ `Класс AnnotationConfigApplicationContext`
+ `Аннотация @ImportResource`
+ `Аннотация @Import`

## 26. @Bean. Часть 1

+ `Аннотация @Bean`
+ `Тестирование Java конфигурации`
+ `Свойства аннотации @Bean`
+ `Аннотация @Scope с @Bean`
+ `Внедрение зависимостей с @Bean`
+ `Конфликт имен @Bean и @Component`

## 27. @Bean. Часть 2

+ `3-ий вариант внедрения зависимостей в @Bean`
+ `Cglib proxy в @Configuration`
+ `Свойство proxyBeanMethods в @Configuration`
+ `@Bean создаются через паттерн Service Locator`

## 28. Profiles
+ `Environment Bean`
+ `Аннотация @Profile`
+ `Активация profiles через properties`
+ `Активация profiles через ApplicationContext`





# 5. Event Listeners


## 29. Event Listeners. Часть 1
+ `Шаблон проектирования Listener`
+ `Создание события (Event)`
+ `Создание слушателя событий (Listener). @EventListener`
+ `Реализация логики для отправки события`

## 30. Event Listeners. Часть 2

+ `Bean ApplicationEventPublisher`
+ `Тестирование слушателей событий`
+ `Listeners order`
+ `Listeners conditions`


# 6. Spring Boot







## 31. Spring Boot. Введение

+ `Spring modules`
+ `Spring Data Configuration`
+ `Modules Auto Configuration`
+ `Conditions`
+ `Spring Boot Starters`
+ `Dependency Management`
+ `How to build Spring Boot Application`

## 32. @Conditional

+ `Аннотация @Conditional`
+ `Класс Condition`
+ `Custom JpaCondition`
+ `Тестирование JpaCondition`
+ `Аннотация @Profile`
+ `Другие @Condition аннотации`

## 33. Spring Boot. Настройка проекта

+ `Spring Boot Gradle Plugin`
+ `Spring Dependency Management Plugin`
+ `spring-boot-starter`
+ `Run Spring Boot Application`
+ `Autogenerated Spring Boot Project`
+ `Maven spring-boot-starter-parent pom`

## 34. @SpringBootApplication

+ `Структура Spring Boot приложения`
+ `Что делает метод SpringApplication.run`
+ `Аннотация @SpringBootApplication`
+ `Аннотация @SpringBootConfiguration`
+ `Аннотация @ComponentScan`
+ `Аннотация @PropertySource`
+ `Аннотация @EnableAutoConfiguration`


## 35. Lombok

+ `Подключение Lombok`
+ `Gradle Lombok Plugin`
+ `IntelliJ IDEA Lombok Plugin`
+ `Аннотации Lombok`
+ `Файл lombok.config`

## 36. Properties

+ `Файл spring.properties`
+ `Externalized Configuration`
+ `Profile-specific properties`
+ `Spring program arguments & VM options`
+ `Property Placeholders & Default values`
+ `spring.config.location`

## 37. Yaml format

+ `YAML - Yet Another Markup Language`
+ `Класс YamlPropertiesFactoryBean`
+ `Приоритет properties vs yaml`
+ `Переписывание application.properties на yaml`


## 38. @ConfigurationProperties

+ `Класс JpaProperties`
+ `Класс DatabaseProperties`
+ `Аннотация @ConfigurationProperties`
+ `Аннотация @ConfigurationPropertiesScan`
+ `Immutable DatabaseProperties`
+ `DatabaseProperties as record`
+ `Property key names`



# 7. Logging Starter


## 39. Logging Starter

+ `Application as a Black Box`
+ `Logging libraries`
+ `Log Levels`
+ `spring-boot-starter-logging dependency`
+ `Аннотация @Slf4j`
+ `Delombok annotations`
+ `Формат логов по умолчанию`
+ `logging.* properties`

## 40. Logback Configuration

+ `Logback default xml configs`
+ `File Output`
+ `Custom log configuration`


# 8. Test Starter

## 41. Test Starter

+ `Подключение spring-boot-starter-test`
+ `Транзитивные зависимости spring-boot-starter-test`
+ `Зависимость spring-test`
+ `Зависимость spring-boot-test`
+ `Зависимость spring-boot-test-autoconfigure`
+ `Пример написания Unit тестов`
+ `Java Gradle Plugin tasks relationship`

## 42. Integration Testing. Part 1

+ `Основные цели Spring Integration Testing`
+ `Жизненный цикл тестов`
+ `JUnit 5 Extension Model`
+ `TestContext Framework`
+ `SpringExtension source code
  `
## 43. Integration Testing. Part 2

+ `Создание CompanyServiceIT`
+ `SpringExtension via @ExtendWith`
+ `Аннотация @ContextConfiguration`
+ `Аннотация @TestPropertySource`
+ `Класс ApplicationContextInitializer`
+ `Аннотация @SpringBootTest`
+ `Написание первого интеграционного теста`
+ `Класс DependencyInjectionTestExecutionListener`

## 44. Integration Testing. Part 3

+ `Аннотация @ActiveProfiles`
+ `Custom Test Annotations`
+ `Аннотация @TestConstructor`
+ `Замена @TestConstructor на spring.properties`

## 45. Context Caching

+ `Создание нескольких ApplicationContext в тестах`
+ `Аннотации @MockBean и @SpyBean`
+ `Класс MockitoTestExecutionListener`
+ `Аннотация @TestConfiguration`
+ `Аннотация @DirtiesContext`


# 9. Data JPA Starter

## 46. Data JPA Starter. Введение
+ `Чего не хватало в Hibernate`
+ `Установка PostgreSQL`
+ `Установка Docker`
+ `Postgres Docker Image`
+ `Подключение к postgres из IntelliJ IDEA`

## 47. Data JPA Starter. Подключение

+ `Подключение spring-boot-starter-data-jpa`
+ `Зависимости spring-boot-starter-data-jpa`
+ `Класс HibernateJpaAutoConfiguration`
+ `Настройка spring.datasource и spring.jpa properties`
+ `Тестирование приложения`

## 48. Hibernate Entities

+ `UML диаграмма выполненных sql скриптов`
+ `Создание сущности Company`
+ `Создание коллекции locales (ElementCollection)`
+ `Создание сущности User`
+ `Создание сущности Payment`
+ `Создание сущности Chat`
+ `Создание сущности UserChat`
+ `Проверка маппинга сущностей через hbm2ddl.auto`
+ `Аннотация @EntityScan`


# 10. Data JPA Transactions

## 49. @Transactional. TestContext
+ `Общая структура работы с TransactionManager`
+ `Создание CompanyRepository IT`
+ `Аннотации @Transactional из Jakarta EE и Spring`
+ `Класс TransactionalTestExecutionListener`
+ `Аннотации @Commit и @Rollback`

## 50. TransactionAutoConfiguration
+ `Класс TransactionAutoConfiguration`
+ `Как происходит обработка транзакций в proxy`
+ `Аннотация @Transactional и Cglib proxy`
+ `Как работает Cglib proxy с TransactionManager`
+ `Как подключить механизм транзакций внутри объекта (не proxy)`
+ `Механизм транзакций между несколькими Cglib proxy`
+
## 51. @Transactional Settings
+ `Свойства @Transactional. transactionManager`
+ `Transaction propagation`
+ `Transaction propagation резюме`
+ `Transaction isolation`
+ `Transaction timeout`
+ `ReadOnly transaction`
+ `Transaction rollbackFor & rollbackForClassName`
+ `Transaction noRollbackFor & noRollbackForClassName`


## 52. Manual Transactions
+ `Свойства объекта TransactionTemplate`
+ `Функционал TransactionTemplate`
+ `Обработка checked exceptions`
+ `Взаимодействие TransactionTemplate с другими Proxy`
+ `Вынесение @Transactional в @IT`


# 11. Data JPA Repositories

## 53. Repository
+ `Интерфейс Repository`
+ `Написание теста на удаление Company`
+ `Класс JpaRepositoryAutoConfiguration`

## 54. RepositoryQuery
+ `Создание Proxy на классы Repository`
+ `Класс QueryExecutorMethodInterceptor`
+ `Класс RepositoryQuery`
+ `Наследники Repository`

## 55. PartTreeJpaQuery
+ `Класс PartTreeJpaQuery`
+ `Примеры написания запросов`
+ `Тестирование запросов`
+ `Весь список ключевых слов PartTreeJpaQuery`


## 56. NamedQuery

+ `Недостатки PartTreeJpaQuery`
+ `Класс NamedQuery`
+ `Аннотация @NamedQuery`
+ `Тестирование NamedQuery`
+ `Аннотация @Param`

## 57. @Query
+ `StoredProcedureJpaQuery`
+ `Аннотация @Query`
+ `Демонстрация работы @Query`
+ `Усовершенствованный оператор LIKE`
+ `Native Query`

## 58. @Modifying

+ `Запрос на обновление через @Query`
+ `Аннотация @Modifying`
+ `Hibernate PersistenceContext`
+ `Свойства clearAutomatically и flushAutomatically`
+ `clearAutomatically и LazyInitializationException`

## 59. Special parameters

+ `Top & First`
+ `TopN & FirstN`
+ `Класс Sort`
+ `Класс Pageable`

## 60. Page & Slice
+ `Spring классы Streamable, Slice, Page`
+ `Демонстрация работы Slice объекта`
+ `Почему Slice объекта недостаточно`
+ `Демонстрация работы Page объекта`

## 61. @EntityGraph

+ `Аннотация @EntityGraph`
+ `Именованные графы @NamedEntityGraph`
+ `Свойство attributePaths в @EntityGraph`
+ `Конфликт Pageable при получении EAGER связей`

## 62. @Lock & @QueryHints

+ `Аннотация @Lock`
+ `Демонстрация пессимистических блокировок`
+ `Аннотация @QueryHints`

## 63. Projection

+ `Class-based Projections`
+ `Generic Class-based Projections`
+ `Interface-based Projections`
+ `SpEL in Projections`

## 64. Custom Repository Implementation

+ `Запрос фильтрации через Custom Implementation`
+ `Criteria API для запроса фильтрации`
+ `Аннотация @EnableJpaRepository`
+ `Тестирование запроса фильтрации`

## 65. JPA Auditing
+ `Создание AuditingEntity`
+ `Аннотация @EnableJpaAuditing`
+ `Тестирование @CreatedDate и @LastModifiedDate`
+ `Аннотации @CreatedBy и @LastModifiedBy`
+ `Создание AuditorAware Bean`
+ `Тестирование @CreatedBy и @LastModifiedBy`

## 66. Hibernate Envers
+ `Подключение Hibernate Envers`
+ `Создание сущности Revision`
+ `Аннотация @Audited`
+ `Аннотация @EnableEnversRepositories`
+ Тестирование Hibernate Envers
+ `Класс RevisionRepository`


## 67. Querydsl

+ `Подключение Querydsl`
+ `Создание QPredicates`
+ `Замена Criteria API на Querydsl`
+ `Тестирование Querydsl`
+ `Класс QuerydslPredicateExecutor`


# 12. JDBC Starter


## 68. JDBC Starter
+ `Зависимость spring-boot-starter-jdbc`
+ `JdbcTemplateAutoConfiguration`
+ `Функционал класса JdbcTemplate`
+ `Практика JdbcTemplate`
+ `Тестирование функционала`
+ `Подключение логов для JdbcTemplate`


## 69. Batch size & Fetch size
+ `Batch запросы`
+ `Batch запрос через JdbcTemplate`
+ `Тестирование Batch запроса через JdbcTemplate`
+ `Batch запрос через NamedParameterJdbcTemplate`
+ `Установка batch_size в Hibernate`
+ `Fetch size`




# 13. Databases in tests

## 70. In-Memory databases. H2
+ `Два варианта поднятия тестовой базы данных`
+ `Подключение H2 database`
+ `Аннотация @Sql`

## 71. Testcontainers
+ `testcontainers lib`
+ `Подключение testcontainers`
+ `Создание IntegrationTestBase`
+ `Тестирование testcontainers`
+ `Тестовые данные (ids)`



# 14. Database Migrations

## 72. Liquibase. Теория
+ `Устройство migration frameworks`
+ `Стуктура Liquibase changelog`
+ `Changelog master file`

## 73. Liquibase. Практика

+ `Подключение зависимости liquibase-core`
+ `Класс LiquibaseAutoConfiguration`
+ `Создание master changelog`
+ `liquibase formatted sql`
+ `Тестирование Liquibase`
+ `Добавление нового changelog (envers tables)`
+ `md5sum`
+ `Использование Liquibase в тестах`


# 15. Web Starter

## 74. Web Starter. Введение
+ `MVC и классические web-приложения`
+ `web-приложение на Spring Boot`
+ `Embedded Tomcat`
+ `Настройка spring-web приложения`
+ `Класс WebMvcAutoConfiguration`


## 75. Dispatcher Servlet
+ `Жизненный цикл сервлетов`
+ `Псевдокод метода service в DispatcherServlet`
+ `Исходный код класса DispatcherServlet`


## 76. @Controller
+ `Подключение зависимостей и настройка view resolver`
+ `Создание контроллера. @Controller`


## 77. @RequestMapping
+ `Основные составляющие HTTP запроса и HTTP ответа`
+ `Основные составляющие URL`
+ `Аннотации @RequestMapping`


## 78. Parameters, Headers, Cookies
+ `Parameters. @RequestParam annotation`
+ `Headers. @RequestHeader annotation`
+ `Cookies. @CookieValue annotation`
+ `Method params naming`
+ `DispatcherServlet sources`
+ `@PathVariable annotation`


## 79. Model
+ `Attributes`
+ `Добавление Request атрибутов в Model`
+ `Добавление Session атрибутов в Model`
+ `DispatcherServlet sources`


## 80. @ModelAttribute
+ `Упрощение работы с объектом ModelAndView`
+ `Динамическое создание атрибутов`
+ `Аннотация @ModelAttribute`
+ `HTML Form. LoginController`


## 81. Forward, Include, Redirect
+ `3 вида перенаправления запросов`
+ `forward in Spring`
+ `redirect in Spring`

## 82. CRUD. API Design
+ `API design best practices`
+ `CRUD. Method findAll`
+ `CRUD. Method findById`
+ `CRUD. Method create`
+ `CRUD. Method update`
+ `CRUD. Method delete`


## 83. CRUD. Service Layer
+ `UserService. Method findAll`
+ `UserService. Method findById`
+ `UserService. Method create`
+ `@Transactional annotation`
+ `UserService. Method update`
+ `UserService. Method delete`
+ `Test UserService functionality`
+ `Tips. Method delete`

## 84. Spring MVC Testing

+ `Аннотация @AutoConfigureMockMvc`
+ `Test findAll method`
+ `Transactions. spring.jpa.open-in-view property`
+ `Test create method`
+ `Problem with sending dates in params`

## 85. Type Converters
+ `1. spring.mvc.format properties`
+ `2. Аннотация @DateTimeFormat`
+ `3. Интерфейс WebMvcConfigurer`


# 16. Thymeleaf

## 86. Thymeleaf Starter. Введение
+ `View Resolvers`
+ `Thymeleaf Template Engine Intro`
+ `Настройка Thymeleaf в проекте`
+ `Использование Thymeleaf`
+ `Тестирование функционала`

## 87. CRUD. View Layer. Часть 1
+ `Создание users.html для метода findAll`
+ `Создание user.html для метода findById`
+ `Тестирование функционала`
+ `Добавление кнопки для метода delete`

## 88. CRUD. View Layer. Часть 2
+ `Создание registration endpoint`
+ `Создание registration.html`
+ `Тестирование функционала registration`
+ `redirect с сохранением введенных параметров`

## 89. Filter Query
+ `Add UserFilter - Controller & Service layers`
+ `Add UserFilter - users.html`
+ `Тестирование функционала`

## 90. Pagination. Best practices
+ `HTTP endpoints best practices`
+ `2 options of pagination implementation`
+ `offset-based pagination`
+ `PageableArgumentResolver`
+ `Building PageResponse`
+ `Тестирование функционала`


# 17. Validation Starter

## 91. Validation Starter. Введение
+ `Подключение validation starter`
+ `Validation annotations`
+ `How to use annotations in practice`
+ `@Valid & @Validated`
+ `BindingResult object`
+ `Show validation errors on the page`
+ `Тестирование функционала`

## 92. Custom validator
+ `Main parts in JSR 303 annotations`
+ `Custom annotation @UserInfo`
+ `Тестирование функционала`
+ `Configuration properties validation`
+ `Validation groups`

## 93. @ControllerAdvice & @ExceptionHandler
+ `@ExceptionHandler annotation`
+ `Тестирование функционала`
+ `@ControllerAdvice annotation`
+ `Класс ResponseEntityExceptionHandler`


# 18. REST

## 94. REST. Введение
+ `Проблемы Controller API`
+ `REST API`
+ `REST API Usages`

## 95. REST. Практика
+ `@ResponseBody & findAll method`
+ `findById method`
+ `@RequestBody & create method`
+ `update method`
+ `delete method`
+ `@RestController`
+ `@RestControllerAdvice`

## 96. Swagger. API docs
+ `Rest clients`
+ `Подключение springdoc`
+ `Сгенерированная документация для Rest Controllers`
+ `Swagger ui`
+ `Swagger annotations`

## 97. Upload image
+ `Добавление новой колонки image в таблице users`
+ `Создание ImageService`
+ `upload images from html pages. MultipartFile`
+ `Тестирование функционала`

## 98. Get image
+ `Реализация функционала на уровне service`
+ `Отображение картинки на html странице`
+ `Реализация функционала на уровне rest controller`
+ `Тестирование функционала`
+ `Отображение отсутствующей картинки`
+ `Класс ResponseEntity`

# 19. Security Starter

## 99. Security Starter. Введение
+ `Понятия Аутентификация и Авторизация`
+ `Servlet Filters mechanism`
+ `Spring Servlet Filters mechanism`
+ `Подключение Spring Security Starter`

## 100. Authentication Architecture
+ `Spring Security Model`
+` Spring Security Authentication Logic`
+ `Debug Security filters (default behaviour)`

## 101. DaoAuthenticationProvider
+ `DaoAuthenticationProvider source code`
+ `Add column password into users table`
+ `Update entity & enum`
+ `Implement UserDetailsService`
+ `Тестирование функциональности`

## 102. Form Login
+ `Default login page source code`
+ `Custom login page`
+ `Customise SecurityFilterChain`
+ `Тестирование функицонала`
+ `Class UsernamePasswordAuthenticationFilter`

## 103. HTTP Basic Authentication

+ `HTTP Basic Authentication principle`
+ `HTTP Basic encoder & decoder`
+ `Customise SecurityFilterChain to support HTTP Basic`
+ `BasicAuthenticationFilter source code`

## 104. PasswordEncoder
+ `Зачем шифровать пароли`
+ `List of password encoders`
+ `Implement password encode/decode in the app`
+ `Тестирование функционала`

## 105. Logout

+ `LogoutFilter source code`
+ `Customise logout in SecurityFilterChain`
+ `Add button Logout on pages`
+ `Тестирование функционала`

## 106. Authorization Architecture
+ `AuthorizationFilter source code and logic`
+ `AuthorizationFilter implementations`
+ `Customise authorizeHttpRequests in SecurityFilterChain`
+ `Тестирование функционала`

## 107. Method Security

+ `@PreAuthorize annotation`
+ `@PostAuthorize annotation`
+ `@EnableMethodSecurity annotation`
+ `@Secured annotation`
+ `Service layer authentication`
+ `@PreFilter & @PostFilter annotations`


## 108. Access to authenticated user

+ `Get current user via SecurityContextHolder`
+ `@CurrentSecutiryContext annotation`
+ `@AuthenticationPrincipal annotation`
+ `Thymeleaf and Spring Security integration`

## 109. CSRF Filter
+ `Cross-Site Request Forgery`
+ `How to solve CSRF problem`
+ `Synchronizer Token Pattern`
+ `When to use CSRF protection`
+ `CsrfFilter source code`
+ `How to work with CSRF token`
+ `Class CsrfRequestDataValueProcessor`
+ `Тестирование функционала`

## 110. Security Testing

+ `Исправление существующих тестов`
+ `spring-security-test dependency`
+ `1. Manually define a user in tests`
+ `2. @WithMockUser annotation`
+ `3. SecurityMockMvcRequestPostProcessor`

## 111. OAuth 2.0. Теория

+ `Текущий Authentication функционал в приложении`
+ `Что такое OAuth 2`
+ `Как внедрить OAuth 2 в приложении`
+ `OAuth 2 flow types`
+ `OAuth 2 Authorization Code Flow`
+ `OAuth 2 Implicit Flow`
+ `OpenID Connect (OIDC)`

## 112. OAuth 2.0. Практика

+ `Create a new project in GCP`
+ `Configure OAuth 2 in the project`
+ `Configure Login Page`
+ `Тестирование функционала`

## 113. OAuth 2.0. Authentication Principle

+ `Add UserInfoEndpoint config in SecurityFilterChain`
+ `Create oidcUserService`
+ `Тестирование функционала`

## 114. JWT. JSON Web Token


+ `How to extract info from JWT`
+ `JWT header`
+ `JWT payload`
+ `JWT signature`
+ `Code Book`

## 115. Swagger Authorization
+ `3 options to pass authorization in Swagger`
+ `springdoc properties to support OAuth 2`
+ `@SecurityScheme configuration`
+ `Тестирование функционала`



# 20. i18n & l10n


## 116. i18n. MessageSource

+ `spring.messages properties`
+ `IntelliJ IDEA UTF-8 settings`
+ `Creating MessageRestController`
+ `Тестирование функционала`

## 117. i18n. Thymeleaf

+ `Login page i18n`
+ `How to change the language`
+ `LocalChangeInterceptor bean`
+ `LocaleResolver bean`
+ `Тестирование функционала`

# 21. AOP Starter

## 118. AOP Starter. Введение
+ `Усложнение кода второстепенной логикой`
+ `Crosscutting concerns`
+ `AOP terminology`
+ `AOP approaches`

## 119. AOP. Pointcut

+ `spring-boot-starter-aop dependency`
+ `AspectJ annotations`
+ `@Pointcut`
+ `@within`
+ `within`
+ `this & target`
+ `@annotation`
+ `args`
+ `@args`
+ `bean`
+ `execution`

## 120. AOP. @Before Advice
+ `@Before annotation`
+ `Тестирование функционала`
+ `CglibAopProxy`
+ `Proxy interceptors`
+ `Spring AOP diagram`
+ `AopAutoConfiguration`

## 121. AOP. JoinPoint. Params

+ `JoinPoint object`
+ `Get access to proxy data from advice method params`
+ `Тестирование функционала`
+ `argNames`

## 122. AOP. @After Advices
+ `All types of advice`
+ `@AfterReturning annotation`
+ `@AfterThrowing annotation`
+ `@After annotation`
+ `Тестирование функционала`

## 123. AOP. @Around Advice
+ `TransactionInterceptor`
+ `@Around annotation`
+ `Тестирование функционала`

## 124. AOP. Best Practices
+ `1. Combine different Pointcut types`
+ `2. Move common Pointcuts to separate Aspect`
+ `3. Don t use @Around advice everywhere`
+ `4. Separate Pointcuts by business logic`
+ `Aspects order`


# 22. Заключение

## 125. Custom Spring Boot Starter
+ `Create a new Gradle module`
+ `Define starter properties`
+ `Create Autoconfiguration`
+ `File META-INF/spring.factories`
+ `Move Aspects from the old to the new module`
+ `How to use newly created starter`
+ `spring-boot-configuration-processor`
+ `Тестирование функционала`

## 126. Заключение. Путь развития

+ `Spring Framework Documentation`
+ `List of all main Spring Boot Starters`
+ `Java Road Map`

