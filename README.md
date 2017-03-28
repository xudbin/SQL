# 从不同服务器另外一个数据库导入表
select * into test from openrowset('SQLOLEDB'
 ,'IP';'sa';'passwd'
 ,test.dbo.rsk)
 
 
 同一个服务器不同库导入数据
 select * into test from  table  
insert into test.dbo.rsk select POARS_SC.dbo.WaterWellDayDataReport.ReportDateTime,
POARS_SC.dbo.WaterWellDayDataReport.WellName,POARS_SC.dbo.WaterWellDayDataReport.DayImmitQuantity from POARS_SC.dbo.WaterWellDayDataReport
where  POARS_SC.dbo.WaterWellDayDataReport.ReportDateTime>='20161101'
