# native-thymeleaf-spel-config-props-demo

Demo for `SpelEvaluationException: EL1008E: Property or field 'key' cannot be found on object of type 'java.util.LinkedHashMap$Entry' - maybe not public or not valid?` when using NestedConfigurationProperty as model in Thymeleaf and native image

```
2023-08-02T13:27:00.402Z ERROR 1 --- [nio-8080-exec-3] o.a.c.c.C.[.[.[/].[dispatcherServlet]    : Servlet.service() for servlet [dispatcherServlet] in context with path [] threw exception [Request processing failed: org.thymeleaf.exceptions.TemplateProcessingException: 
  Exception evaluating SpringEL expression: "app.key" (template: "view" - line 13, col 30)] with root cause

org.springframework.expression.spel.SpelEvaluationException: EL1008E: Property or field 'key' cannot be found on object of type 'java.util.LinkedHashMap$Entry' - maybe not public or not valid?
        at org.springframework.expression.spel.ast.PropertyOrFieldReference.readProperty(PropertyOrFieldReference.java:222) ~[na:na]
```