<!-- markdownlint-disable MD002 MD025 MD041 -->
<!--- # Introduction --->

Соединители Graph Microsoft позволяют добавлять собственные данные в microsoft Graph и использовать различные Microsoft 365 опытом.

В этом приложении .NET Core показано, как использовать API соединительных Graph Microsoft для создания соединительных связутелей клиентов и использования его для Поиск (Майкрософт). В этом руководстве используется пример инвентаризации частей приборов данных для организации Починка приборов Contoso.

## <a name="how-does-the-sample-work"></a>Как работает пример?

В примере создается Windows настольное приложение, которое получает маркер из платформа удостоверений Майкрософт и использует его для отправки запросов в API соединителов microsoft Graph. API соединителов отправляет свой ответ после проверки доступа.

![Схема, показывающая Windows, приобретаемое маркером и использующее его для доступа к API соединителов Microsoft Graph.](images/connectors-images/build1.png)

## <a name="prerequisites"></a>Необходимые условия

* Установите [Visual Studio 2019](https://visualstudio.microsoft.com/) с [SDK .NET Core 3.1](https://www.microsoft.com/net/download/core) на компьютере разработки.
* Убедитесь, что у вас есть [личная учетная запись Майкрософт](https://signup.live.com/)или учетная запись для работы или школы.
* Установите [основные инструменты Entity Framework в](/ef/core/miscellaneous/cli/dotnet) качестве глобального средства с помощью следующей команды:

    ```dotnetcli
    dotnet tool install --global dotnet-ef
    ```

* Установите средство для обновления базы данных SQLite. Например, браузер [DB для SQLite](https://sqlitebrowser.org/).
* Скачайте **ApplianceParts.csv** из примера репо соединиттеля [поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/PartsInventoryConnector/ApplianceParts.csv).

> [!TIP]
> Лучший способ скачивания файлов из GitHub — перейти на верхний уровень проекта. С зеленой **кнопки загрузки кода** справа выберите **Скачать ZIP**. Файл ZIP будет содержать содержимое репозитория.
