<!-- markdownlint-disable MD002 MD025 MD041 -->

1. <span data-ttu-id="a3850-101">Откройте интерфейс командной строки (CLI) в каталоге, где расположен PartsInventoryConnector.csproj.</span><span class="sxs-lookup"><span data-stu-id="a3850-101">Open your command line interface (CLI) in the directory where PartsInventoryConnector.csproj is located.</span></span>
2. <span data-ttu-id="a3850-102">Запустите следующую команду, чтобы инициализировать секреты пользователя для проекта.</span><span class="sxs-lookup"><span data-stu-id="a3850-102">Run the following command to initialize the user secrets for the project.</span></span>

    ```dotnetcli
    dotnet user-secrets init
    ```

3. <span data-ttu-id="a3850-103">Запустите следующие команды для хранения вашего ID приложения, секрета приложения и ИД клиента в хранилище секрета пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3850-103">Run the following commands to store your app ID, app secret, and tenant ID in the user secret store.</span></span>
  
    ```dotnetcli
      dotnet user-secrets set appId "YOUR_APP_ID_HERE"
      dotnet user-secrets set appSecret "YOUR_APP_SECRET_HERE"
      dotnet user-secrets set tenantId "YOUR_TENANT_ID_HERE"
    ```
