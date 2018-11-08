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
TransactionDefinition
定义了事务的传播性、隔离性、超时时间和只读属性
```
  public interface TransactionStatus extends SavepointManager {

      boolean isNewTransaction();

      boolean hasSavepoint();

      void setRollbackOnly();

      boolean isRollbackOnly();

      void flush();

      boolean isCompleted();

  }
```
