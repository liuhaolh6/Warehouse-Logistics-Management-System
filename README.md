库房物流管理系统
一个用于管理库存、订单、供应商和物流的综合系统，旨在优化库存管理、提高订单处理效率、降低物流成本，并确保供应链的顺畅运作。
功能
库存管理：实时查询库存数量、位置和状态；自动更新库存数量，支持入库、出库和调拨操作；设置库存上下限，当库存低于或高于设定值时发出警报；支持定期盘点和不定期盘点，记录盘点结果和差异。
订单管理：支持手动和自动创建订单；包括订单分配、拣货、包装和发货；实时跟踪订单状态，提供物流信息；记录历史订单，支持查询和分析。
供应商管理：存储供应商的基本信息和联系方式；支持采购订单的创建、审批和跟踪；评估供应商的绩效，包括交货时间、质量等。
物流管理：实时跟踪货物运输状态；管理运输计划、运输方式和成本；优化配送路线，提高配送效率。
报表和分析：生成库存报表，包括库存数量、价值等；生成订单报表，分析订单处理效率；生成物流报表，分析运输成本和效率；提供数据分析工具，帮助决策。
技术栈
前端：HTML5, CSS3, JavaScript, Vue.js
后端：Java (Spring Boot)
数据库：MySQL
中间件：RabbitMQ (消息队列), Redis (缓存)
部署：Docker, Kubernetes
安装与运行
前端
cd src/frontend，npm install，npm start
后端
cd src/backend，mvn install，mvn spring-boot:run
数据库
docker run --name warehouse-db -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=warehouse -p 3306:3306 -d mysql:5.7
