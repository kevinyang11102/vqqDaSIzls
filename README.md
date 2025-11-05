## 前言

随着法律服务市场的快速发展，律师事务所对于案件管理系统的需求日益增长。为满足这一需求，我们基于Spring Boot框架，开发了一款律师事务所案件管理系统。该系统不仅提高了律师事务所的工作效率，也为律师提供了更加便捷的案件管理服务。

## 内容介绍

本项目是一款基于Spring Boot的律师事务所案件管理系统，主要包括以下功能模块：

1. 案件管理：律师可以在此模块中添加、查询、修改、删除案件信息，包括案件名称、当事人、案由、诉讼阶段等。

2. 客户管理：律师可以管理自己的客户信息，包括客户姓名、联系方式、企业名称等，方便后续案件跟进。

3. 文书管理：律师可以在此模块中上传、下载、查看案件相关文书，如起诉状、答辩状、代理词等。

4. 日程管理：律师可以安排自己的日程，设置案件开庭时间、会议时间等，系统将自动提醒。

5. 财务管理：律师可以管理案件的收费情况，包括收费标准、已收款项、未收款项等。

6. 统计分析：系统将自动统计律师的案件数量、收费情况等数据，方便律师了解自己的工作情况。

## 技术介绍

- 语言：Java
- 使用框架：Spring Boot
- 前端技术：JS、Vue、css3
- 开发工具：IDEA/Eclipse
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven: apache-maven 3.8.1-bin
- 前端环境：Node.js 12/14/16

## 核心代码

```java
@Service
public class CaseService {

    @Autowired
    private CaseRepository caseRepository;

    public List<Case> getAllCases() {
        return caseRepository.findAll();
    }

    public Case getCaseById(Long id) {
        return caseRepository.findById(id).orElse(null);
    }

    public Case addCase(Case caseToAdd) {
        return caseRepository.save(caseToAdd);
    }

    public Case updateCase(Long id, Case caseDetails) {
        Case caseToUpdate = caseRepository.findById(id).orElse(null);
        caseToUpdate.setClient(caseDetails.getClient());
        caseToUpdate.setCaseName(caseDetails.getCaseName());
        caseToUpdate.setLawsuitStage(caseDetails.getLawsuitStage());
        return caseRepository.save(caseToUpdate);
    }

    public void deleteCase(Long id) {
        caseRepository.deleteById(id);
    }
}
```

## 免费源码获取

```
8000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/324071/32/4704/222637/689eadefFe8bca0a0/6503fed19a69ff41.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/326510/21/4796/81499/689eadceFbbec9d38/9bba10f11c90defc.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/319188/36/25535/186081/689eadcfF2c5077da/7decc68da3e437be.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/301947/13/11189/50163/689eadd0F0503092f/99cb2f590cbe5544.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/294329/6/6976/50365/689eadd0F0ef491bd/94ccd22b413ca651.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/320382/22/25419/116488/689eadd1Ff046e614/aa02e6b8a63146cb.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/327674/5/4801/78292/689eadd1F23f1ab33/615b1541ce1c33e2.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/307686/11/26809/41773/689eadd2F9d6724cf/5ce269feecd92279.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/317073/24/25307/47006/689eadd2F2d383e24/770aa09b2a201cf1.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/327196/11/4867/56310/689eadd3F01bbf692/84904c13c62ef2f2.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
