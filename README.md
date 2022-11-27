# 题目01：MyBatis通常是一个XML映射文件配合一个Dao接口，请问Dao接口的工作原理是什么？  
主要是使用SqlSession接口。有两种开发方式，一是基于Dao层接口实现类开发，调用session.selectOne接口。二是基于动态代理自动生成Dao层接口实现类， 调用session.getMapper接口。

# 题目02：请你用自己的理解，简单说说MyBatis内SQL语句的执行原理?  
关键点01：参数是如何注如SQL语句【2种形式】  
ParameterHandler  

关键点02：SQL语句执行经历了那些组件  
1. SqlSession  
2. Executor  
3. StatementHandler  
4. TypeHandler  

关键点03：结果集如和映射到对象  
ResultSetHandler  
