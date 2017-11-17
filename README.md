# Java8Demo
   
   
```java
    @Component(modules = {BackendModule.class, FrontendModule.class})
         interface MyComponent {
           MyWidget myWidget();

            @Component.Builder
           interface Builder {
             //一个没有参数的`build()`方法，返回MyComponent类型
             MyComponent build();
             Builder backendModule(BackendModule bm);
             Builder frontendModule(FrontendModule fm);
           }
         }
    ```