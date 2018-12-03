<style>
.s-right{
    width:100%
    float:right;
    margin-right:0px;
   
}

.s-left{
    float:left;
    width: 300px;
    
}
</style>

# 杨洪竞 <sub>/ Hongjing Yang</sub>

## Java 开发工程师

 <span> 
 关于我

  <ul>
    <li>
       <span class='s-left'>学历：本科</span><span class="s-right">邮箱: 1501587673@qqcom</span>
    </li>
    <li>
       <span class='s-left'>专业：信息工程</span><span class="s-right">电话: 13558707986</span>
    </li>
    <li>
        <span class='s-left'>学校：西南林业大学</span> <span class="s-right">github:https://github.com/yanghj7425</span>
    </li>
  </ul>
</span>

### 个人技能

#### 后台

<ul>
    <li> Java：Spring MVC、security、mybatis、MQ、Spring 框架、读过 Spring 源码</li>
    <li> 熟悉liunx 命令：能编写 Shell 脚本编写</li>
    <li> python：可以编写一些处理数据的脚本、rabbitMQ 消费者等</li>
    <li> 数据库：熟悉 MySQL、SQL 优化</li>
</ul>

### 个人优势

有 c、python 和 java 的项目经历。熟悉 Oracle 、MySQL、Liunx、Shell、MyBatis、MQ 、SpringMVC、翻译了 Spring framework 文档。看过《重构》、《设计模式》、《Effective java》、《Think in Java》、《Spring 实战》、《高性能 MySQL》、《Java 高并发设计》、《深入分析 Java Web》等书。能在项目中使用重构技巧和设计模式，曾用代理和策略模式重构了接手的模块。读过 Spring 源码，这个主要是对 Spring 是怎么实现的感兴趣。<br>
最后：github 和博客里有上面有上面所述信息。

#### 常用工具

- JMeter：压力测试
- PostMan: 测试接口
- svn、git: 版本控制
- markdown: 编写文档，这份简历就是 markdown 编写

### 工作经历

#### <span class='s-left'>上海梦创双杨数据科技股份有限公司 </span> <span class='s-right'>2018/4 - 今</span>

 <ul>
    <li>
        项目名称：党建项目
    </li>
    <li>
        项目简介：国家党校的项目
    </li>
    <li>
        我的职责：提供党员积分、人员管理、资源预约、活动管理接口、Docker 测试环境。
        <ul>
          <li> 积分：这里有个坑…… 总之之前存储过程做的事情（本来就不推荐用存储过程更何况我司用的 MySql）用 python 改写了之后 30 个线程一起干以前七八个小时的事情现在 50 分钟左右。原因很简单，近千万的数据再加上锁表。其实现在还有一部分是锁表的过程，但是我也总不能老跟"前辈"说，这个过程会锁表……
          </li>
          <li>
            资源：也有坑，资源要审核。但是系统里面很多东西都要走审核流程，所以一个方法里面 80% 都在 if ，如比如一个 400 多行的方法里面……。解决方法，单独写一个模块控制审核，对外暴露接口（工作量……）。
          </li>
        </ul>
    </li>
 </ul>

#### <span class='s-left'>四川久远银海软件股份有限公司</span> <span class="s-right">2016/11-2018/3/31</span>

  <ul>
    <li>
        项目名称：网上申报
    </li>
    <li>
        项目简介：单位人员发生变动时提供社保相关功能的停保和续保.
    </li>
    <li>
        我的职责：业务比较复杂、查询类功能、单位批量参保信息导入/导出、重做登录权限模块和功能授权模块。有的功能都是 Java -> ibaits -> 存储过程（ORACLE）-> dblink 这个流程；有的是走 webService 。
    </li>
    <br>
    <li>
       项目名称: 自助查询一体机
    </li>
    <li>
       项目简介: 提供社保业务的查询,和社保卡的挂失,相关证明打印
    </li>
    <li>
        我的职责:润乾报表打印、一体机本地化配置、社保卡和身份证数据的读取还有一些查询功能。第一版,负责医保相关功能查询和登录效验；第二版主要是重构Java代码，根据不同类型的功能划分后台代码模块。后期，加日志记录功能；优化代码提高可扩展性:实现不同区域的设备配置不同的功能.
    </li>
  </ul>

- 备注: 数据库 Oracle、Java、ssm 框架

#### <span class='s-left'> 云南这里信息技术有限公司 </span><span class="s-right">2016/9-2016/11</span>

- _项目名称_ : 档案定位
- _项目简介_ : 通过传感器,标记每个位置的档案.若有档案被取走或者归还,则发送信号给嵌入式设备,嵌入式设备通过网关把数据发送到服务器,由服务器入库.然后网页显示档案信息.
- _我的职责_ : 信息采集电路设计,C 语言实现对采集到的信号进行解析并发送到网关,Java 通过 Spring 的 Executor 按约定的时间采集数据存入 MySQL.
- 备注 : C 语言、汇编、MySQL、Java、ssm 框架。

## 项目经历

### 网上申报

- 这个项目是 10 多年的老项目了（存储过程的注释有写日期），主要学的就是业务，重新封装了框架的 POI，原来的对于这个项目不太灵活（与业务耦合性太高），封装后导入/导出的时候就自己封装的 POI，封装后，对于不同的表单只需在实体类上添加相应的注解。
- 重做登陆和权限模块模块: Spring Security 做的权限。通过修改用户组和角色表，达到给用户默认权限以及灵活的控制权限。主要是用户的管理员有很多是老党员，不太擅长操作电脑。所以要重做，主要是数据清理和提供默认权限。系统升级前的老数据用 PL/SQL 程序调整，

### 自助查询一体机

- 是 N 手项目也是试点项目。几乎是驻场开发，第一版的时候主要负责润乾报表打印、登陆、日志记录、电子证明下载。用户打印已签章的证明后，电子原件上传 FTP 并记录操作日志。

### <span class='s-left'> 在校期间</span> <span class="s-right">2014-2017</span>

大二进了学院实验室(主要是嵌入式方向，但是感觉编程都会)、参加了几个比赛。帮土木工程学院做了门户网站（两人合作）、贪吃蛇、捕鱼达人、五子棋、俄罗斯方块(C 语言)、摇摇棒、调频发射器、调频收音机、光立方、智能小车。总之大学还算比较充实……
