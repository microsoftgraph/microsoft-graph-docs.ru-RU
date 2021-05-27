<!-- markdownlint-disable MD002 MD025 MD041 -->

1. Откройте интерфейс командной строки (CLI) в каталоге, где расположен PartsInventoryConnector.csproj.
2. Выполните следующие команды:

  ```dotnetcli
  dotnet ef migrations add InitialCreate
  dotnet ef database update
  ```

> [!NOTE]
> Запустите следующие команды, если схема изменяется в CSV-файле и отражают эти изменения в базе данных SQLite.

```dotnetcli
dotnet ef database drop
dotnet ef database update
```
