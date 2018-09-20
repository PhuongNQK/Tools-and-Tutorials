# Designing classes
- Generic Command pattern: https://www.cuttingedge.it/blogs/steven/pivot/entry.php?id=91

# Designing APIs and Communication Mechanism
## REST APIs
- Naming conventions:
    - https://restfulapi.net/resource-naming/
    - https://blog.mwaysolutions.com/2014/06/05/10-best-practices-for-better-restful-api/

## Streaming broker
- Kafka vs. RabbitMQ: https://content.pivotal.io/blog/understanding-when-to-use-rabbitmq-or-apache-kafka

# Designing Apps
## Principles
Define your business model
- What do you want to sell?
- What is your processing stack and the level of customisability?
    - Data analytic: https://www.forbes.com/sites/danwoods/2017/10/31/leveraging-analytics-stacks-how-the-clickfox-platform-supports-all-levels-of-productization/#783f954a7623
- Data model should be based on business model.

[Creating Truly Modular Code with No Dependencies](https://www.toptal.com/software/creating-modular-code-with-no-dependencies?utm_campaign=blog_post_creating_modular_code_with_no_dependencies&utm_medium=email&utm_source=blog_subscribers&utm_campaign=Toptal%20Engineering%20Blog&utm_source=hs_email&utm_medium=email&utm_content=56572931&_hsenc=p2ANqtz-9Eul1wY5UWzCGl9MdOsxz1kWuWphbXURUx6JST-lwufzmv6pn733g2aY9W4FH12EgOpLKbp30aYA3K-SBjllv356vCww&_hsmi=56572931)

Should that be a Microservice?
- [Keep These Six Factors in Mind](https://content.pivotal.io/blog/should-that-be-a-microservice-keep-these-six-factors-in-mind)
- [Part 2: Multiple Rates of Change](https://content.pivotal.io/blog/should-that-be-a-microservice-part-2-multiple-rates-of-change?utm_source=pivotal-newsletter&utm_medium=email-link&utm_campaign=external-newsletter&mkt_tok=eyJpIjoiWkRJeE0yTTRPR00wWlRJMiIsInQiOiJ0QmxpNHNFM1JcL3REWDZcL2p5c1dqZlwvWjV3WURJM0NVbzBWckJkR3UwcVZzUnRwRFRJYm1hK0Jld0NKcVdjSEpJMnMwXC9aXC9vYVBadlRyVnRpR1FCRUZBR0x5N1FnY25TaG16UFpKdlRlbUZ4YTdlTURlZmtHU09zK0ZRWUFNZjVyIn0%3D) 
- [Part 3: Independent Life Cycles](https://content.pivotal.io/blog/should-that-be-a-microservice-part-3-independent-life-cycles)

Utilize abstraction layers for flexibility. E.g.
- Instead of using Apache Flink / Apache Spark directly, we can use Apache Beam
- Instead of using Hadoop directly, we can use Apache Ignite

## Concepts
- API vs. SPI: https://stackoverflow.com/questions/2954372/difference-between-spi-and-api
- SPI: https://www.developer.com/java/article.php/3848881/Service-Provider-Interface-Creating-Extensible-Java-Applications.htm
- DDD: https://cemicrosoft.wordpress.com/2013/08/05/domain-oriented-n-layer-architecture/
- Microservices & DevOps: https://www.red-gate.com/blog/database-devops/thinking-microservices-need-devops-first-nebbia?utm_source=simpletalk&utm_medium=pubemail&utm_content=20180417-slota3&utm_term=simpletalkmain
- Future Thinking design: https://www.oecd.org/site/schoolingfortomorrowknowledgebase/futuresthinking/overviewofmethodologies.htm

## Templates
- ASP.NET Boilerplate:
    - https://aspnetboilerplate.com/
    - https://github.com/aspnetzero/documents
- A frontend Framework for building admin applications running in the browser on top of REST services, using ES6, React and Material Design: https://marmelab.com/admin-on-rest/

## Samples
- Calling RESTful APIs in Unity3D: https://www.red-gate.com/simple-talk/dotnet/c-programming/calling-restful-apis-unity3d/?utm_source=simpletalk&utm_medium=pubemail&utm_content=20180417-slota2&utm_term=simpletalkmain
- Salesforce data model: https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/data_model.htm

# Designing Solutions
## Principles
- Which is the preferred deployment model from the customer's perspective: on-prem, in cloud (GCP, Azure, AWS), or hybrid (Azure Stack from Microsoft, OpenStack from Ubuntu)?
- Any application porting is needed? Feasible? E.g. 
  - An application may need porting from Red Hat to Ubuntu due to lack of official support: https://stackoverflow.com/questions/30947478/how-does-one-install-marklogic-8-on-ubuntu-14-04
- Open to polyglotting:
  - http://memeagora.blogspot.com/2006/12/polyglot-programming.html
  - http://www.jamesserra.com/archive/2015/07/what-is-polyglot-persistence/
- Define API for integration between different subsystems / components:
  - REST vs. GraphQL: https://dev-blog.apollodata.com/graphql-vs-rest-5d425123e34b
  - REST:
    - Swagger: http://swagger.io/
  - GraphQL:
    - https://www.multidots.com/graphql-efficient-alternative-rest/
    - Wrapping a REST API in GraphQL: https://graphql.org/blog/rest-api-graphql-wrapper/
    - Play with GraphQL: https://launchpad.graphql.com/1jzxrj179
    - Getting Started with GraphQL and Spring Boot: http://www.baeldung.com/spring-graphql
    - GraphQL Java implementation: https://github.com/graphql-java/graphql-java
    - Hide Elastic Search REST API behind GraphQL: https://github.com/graphql-compose/graphql-compose-elasticsearch

## Scalability and High Availability
- Lessons learned:
    - How do large Web sites handle the load of millions of visitors a day? https://computer.howstuffworks.com/internet/basics/question342.htm
    - How I built an app with 500,000 users in 5 days on a $100/month server? https://medium.com/unboxd/how-i-built-an-app-with-500-000-users-in-5-days-on-a-100-server-77deeb238e83
    - Cloud-native architecture with serverless microservices — the Smart Parking story: https://cloudplatform.googleblog.com/2018/04/Cloud-native-architecture-with-serverless-microservices-the-Smart-Parking-story.html

# Common App Frameworks
- Java SpringBoot
- ASP.NET Core 


