# spring-learn
spring框架学习
## spring-transaction
https://docs.spring.io/spring/docs/current/spring-framework-reference/data-access.html#spring-data-tier
```
  public interface PlatformTransactionManager {

    	TransactionStatus getTransaction(TransactionDefinition definition) throws TransactionException;

    	void commit(TransactionStatus status) throws TransactionException;

    	void rollback(TransactionStatus status) throws TransactionException;
 }
```
