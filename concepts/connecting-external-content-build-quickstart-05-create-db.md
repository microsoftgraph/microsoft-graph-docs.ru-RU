<!-- markdownlint-disable MD002 MD025 MD041 -->

1. <span data-ttu-id="66009-101">Откройте интерфейс командной строки (CLI) в каталоге, где расположен PartsInventoryConnector.csproj.</span><span class="sxs-lookup"><span data-stu-id="66009-101">Open your command line interface (CLI) in the directory where PartsInventoryConnector.csproj is located.</span></span>
2. <span data-ttu-id="66009-102">Выполните следующие команды:</span><span class="sxs-lookup"><span data-stu-id="66009-102">Run the following commands:</span></span>

  ```dotnetcli
  dotnet ef migrations add InitialCreate
  dotnet ef database update
  ```

> [!NOTE]
> <span data-ttu-id="66009-103">Запустите следующие команды, если схема изменяется в CSV-файле и отражают эти изменения в базе данных SQLite.</span><span class="sxs-lookup"><span data-stu-id="66009-103">Run the following commands if a schema changes in the CSV file, and reflect those changes into the SQLite database.</span></span>

```dotnetcli
dotnet ef database drop
dotnet ef database update
```
