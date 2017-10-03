# learn-activiti
activiti demo
调用部署方法:  会把指定路径的bpmn 文件 存储到activiti 工作流引擎的数据库表中:
1.ACT_GE_BYTEARRAY		他存储的是二进制的数据文件（也就是bpmn.xml）
2.ACT_RE_DEPLOYMENT	他存储的是部署的结果信息(比如 部署编号..)
3.ACT_RE_PROCDEF		他存储的是流程定义信息

ACT_RE_PROCDEF表:   processdefinition<流程定义>
  ID_  流程定义ID     
  KEY_ 流程定义KEY
  DEPLOYMENT_ID_ 部署ID <关联ACT_RE_DEPLOYMENT表>
  SUSPENSION_STATE_ 流程定义是否为挂起状态   1为可用状态  2为挂起状态
