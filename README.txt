构建数据库
CREATE TABLE `info` (
  `id` int NOT NULL AUTO_INCREMENT,
  `year` int DEFAULT NULL COMMENT '年份',
  `month` int DEFAULT NULL COMMENT '月份',
  `room_number` int DEFAULT NULL COMMENT '房间号',
  `build_type` int NOT NULL DEFAULT '1' COMMENT '建筑类型（默认1 代表我住的那一栋）',
  `electric` decimal(19,2) DEFAULT NULL COMMENT '电表数',
  `water` decimal(19,2) DEFAULT NULL COMMENT '水表数',
  `create_time` datetime DEFAULT NULL COMMENT '录入时间',
  `update_time` datetime DEFAULT NULL ON UPDATE CURRENT_TIMESTAMP COMMENT '修改时间',
  `room_price` int NOT NULL DEFAULT '0' COMMENT '房租价',
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=5 DEFAULT CHARSET=utf8;
