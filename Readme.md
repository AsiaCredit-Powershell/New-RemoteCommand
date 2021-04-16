
   .DESCRIPTION
   Функция получает список компов в домене и выполняет внутри них введенные команды

   .PARAMETER -FilterCompName
   Принимает string - наименование или часть наименования компа

   .PARAMETER -Command
   Принимает string - комманда для выполнения (Если есть кириллица или проблелы - команду с производными втыкай в кавычки) 
        
   .EXAMPLE
   New-RemoteCommand -FilterCompName sdv5 -Command "Get-ChildItem c:\"
   Возвращает каталоги диска C:\ на машине SDV5 