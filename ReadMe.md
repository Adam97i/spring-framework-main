
## 阅读步骤
- 选中部分代码全局搜索即可找到对应源码


## 快捷键
| 方法名                         | 说明     | 快捷键              | 推荐增加    |
|-----------------------------|--------|------------------|---------|
| Go to Declaration or Usages | 进入代码调用 | Ctrl + B         | Alt + E |
| Back                        | 返回调用   | Ctrl + Alt + ←   | Alt + Q |  
| Find in files               | 全局搜索   | Ctrl + Shift + F | Alt + W | 





## 容器



```java
// 注解容器初始化
public class AnnotationConfigApplicationContext

// bean定义
public interface BeanDefinition extends AttributeAccessor, BeanMetadataElement 
    

// 获得bean 
// 单例模式下先创建bean的依赖，再通过缓冲池获得单例bean，不存在则 createBean
// 原型模式则返回新的实例
protected <T> T doGetBean
        
// 单例模式下用三级缓存解决循环依赖
protected Object getSingleton

// 创建bean实例，赋值，初始化 
// bean的生命周期 instance -> populate -> initialize -> destroy
protected Object doCreateBean

// bean工厂
public interface BeanFactory

```

## SpringMVC

```java

// springMVC  handlerAdapter适配器模式
public interface HandlerAdapter 

protected HandlerExecutionChain getHandler(HttpServletRequest request) throws Exception 

protected HandlerAdapter getHandlerAdapter(Object handler) throws ServletException 

```

## 事务

```java

// 事务
public @interface Transactional 
// 事务隔离级别
public enum Isolation 
// 事务传播方式
public interface TransactionDefinition 

```

