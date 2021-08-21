# QLSV_EntityFramework
* Change your ConnectionString in DAL.App.Config and GUI.App.Config 
## App.Config
``` 
<connectionStrings>
  =====  SQL sever authentication
    <add name="QlsvContext" connectionString="data source=localhost,1433;initial catalog=DBName_in_SQLServer;user id = sa;pwd=your_pass;MultipleActiveResultSets=True;App=EntityFramework" providerName="System.Data.SqlClient" />
  ====== window authentication
    <add name="QlsvContext" connectionString="data source=.;Initial Catalog=DBName_in_SQLServer;Integrated Security=True;MultipleActiveResultSets=True;App=EntityFramework" providerName="System.Data.SqlClient" />
  </connectionStrings> 
```  
 ###### if "data source=localhost,1433" not working => try: "data source=."
