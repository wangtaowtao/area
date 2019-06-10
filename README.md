> 中国地区Mysql建表语句
##  中国地区三级联动语句
CREATE TABLE `AREA` (
  `ID` bigint(20) NOT NULL AUTO_INCREMENT COMMENT 'id',  
  `FULLNAME` varchar(255) COLLATE utf8_bin NOT NULL COMMENT '全称',  
  `GRADE` int(11) NOT NULL COMMENT '层级',  
  `NAME` varchar(255) COLLATE utf8_bin NOT NULL COMMENT '名称',  
  `TREEPATH` varchar(255) COLLATE utf8_bin NOT NULL COMMENT '树路径',  
  `ISDELETE` int(11) DEFAULT NULL COMMENT '是否删除(1是 0否)',  
  `ORDERS` int(11) DEFAULT NULL COMMENT '排序',  
  `VERSION` float NOT NULL COMMENT '版本',  
  `CREATEDDATE` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP COMMENT '创建日期',  
  `LASTMODIFIEDDATE` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP COMMENT '更新日期',  
  `PARENT_ID` bigint(20) DEFAULT NULL COMMENT '地区父id',  
  PRIMARY KEY (`ID`)  
) ENGINE=InnoDB AUTO_INCREMENT=3510 DEFAULT CHARSET=utf8 COLLATE=utf8_bin;
