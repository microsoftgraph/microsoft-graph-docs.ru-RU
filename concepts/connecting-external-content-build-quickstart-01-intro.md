<!-- markdownlint-disable MD002 MD025 MD041 -->
<!--- # Introduction --->

<span data-ttu-id="cbff1-101">Соединители Graph Microsoft позволяют добавлять собственные данные в microsoft Graph и использовать различные Microsoft 365 опытом.</span><span class="sxs-lookup"><span data-stu-id="cbff1-101">Microsoft Graph connectors allow you to add your own data into Microsoft Graph and have it power various Microsoft 365 experiences.</span></span>

<span data-ttu-id="cbff1-102">В этом приложении .NET Core показано, как использовать API соединительных Graph Microsoft для создания соединительных окне клиентов и использования его для питания Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="cbff1-102">This .NET Core application shows you how to use the Microsoft Graph connectors API to create a customer connector and use it to power Microsoft Search.</span></span> <span data-ttu-id="cbff1-103">В этом руководстве используется пример инвентаризации частей приборов данных для организации Починка приборов Contoso.</span><span class="sxs-lookup"><span data-stu-id="cbff1-103">This tutorial uses a sample data appliance parts inventory for the Contoso Appliance Repair organization.</span></span>

## <a name="how-does-the-sample-work"></a><span data-ttu-id="cbff1-104">Как работает пример?</span><span class="sxs-lookup"><span data-stu-id="cbff1-104">How does the sample work?</span></span>

<span data-ttu-id="cbff1-105">В примере создается Windows настольное приложение, которое получает маркер из платформа удостоверений Майкрософт и использует его для отправки запросов в API соединителов microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cbff1-105">The sample creates a Windows desktop app that acquires a token from the Microsoft identity platform, and uses it to send requests to the Microsoft Graph connectors API.</span></span> <span data-ttu-id="cbff1-106">API соединителов отправляет свой ответ после проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="cbff1-106">The connectors API will send its response after the access is validated.</span></span>

![Схема, показывающая Windows, приобретаемое маркером и использующее его для доступа к API соединителов Microsoft Graph.](images/connectors-images/build1.png)

## <a name="prerequisites"></a><span data-ttu-id="cbff1-108">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="cbff1-108">Prerequisites</span></span>

* <span data-ttu-id="cbff1-109">Установите Visual Studio 2019 с [SDK .NET Core 3.1](https://www.microsoft.com/net/download/core) на компьютере разработки.</span><span class="sxs-lookup"><span data-stu-id="cbff1-109">Install Visual Studio 2019 with [.NET Core 3.1 SDK](https://www.microsoft.com/net/download/core) on your development computer.</span></span>
* <span data-ttu-id="cbff1-110">Убедитесь, что у вас есть [личная учетная запись Майкрософт](https://signup.live.com/)или учетная запись для работы или школы.</span><span class="sxs-lookup"><span data-stu-id="cbff1-110">Make sure that you have a [personal Microsoft account](https://signup.live.com/), or a work or school account.</span></span>
* <span data-ttu-id="cbff1-111">Установите [основные инструменты Entity Framework в](/ef/core/miscellaneous/cli/dotnet) качестве глобального средства с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="cbff1-111">Install the [Entity Framework Core Tools](/ef/core/miscellaneous/cli/dotnet) as a global tool using the following command:</span></span>

    ```dotnetcli
    dotnet tool install --global dotnet-ef
    ```

* <span data-ttu-id="cbff1-112">Установите средство для обновления базы данных SQLite.</span><span class="sxs-lookup"><span data-stu-id="cbff1-112">Install a tool to update a SQLite database.</span></span> <span data-ttu-id="cbff1-113">Например, браузер [DB для SQLite](https://sqlitebrowser.org/).</span><span class="sxs-lookup"><span data-stu-id="cbff1-113">For example, the [DB Browser for SQLite](https://sqlitebrowser.org/).</span></span>
* <span data-ttu-id="cbff1-114">Скачайте **файлApplianceParts.csv** из [](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/PartsInventoryConnector/ApplianceParts.csv) репо соединиттеля поиска и добавьте его в PartsInventoryConnector.csproj.</span><span class="sxs-lookup"><span data-stu-id="cbff1-114">Download the **ApplianceParts.csv** file from the [Search connector sample repo](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/PartsInventoryConnector/ApplianceParts.csv) and add it to the PartsInventoryConnector.csproj.</span></span>
