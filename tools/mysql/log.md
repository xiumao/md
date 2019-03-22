### general log

- 开启 general log 将所有到达MySQL Server的SQL语句记录下来。
- 一般不会开启开功能，因为log的量会非常庞大。但个别情况下可能会临时的开一会儿general log以供排障使用。 
- 相关参数一共有3：general_log、log_output、general_log_file
> show variables like 'general_log'; 
> set global general_log=on; -- 开启日志功能

> show variables like 'general_log_file';  -- 看看日志文件保存位置
> set global general_log_file='tmp/general.lg'; -- 设置日志文件保存位置

> show variables like 'log_output';  -- 看看日志输出类型  table或file
> set global log_output='table'; -- 设置输出类型为 table
> set global log_output='file';   -- 设置输出类型为file