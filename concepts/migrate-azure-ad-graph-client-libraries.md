---
title: Перенос приложений .NET для Azure AD Graph в Microsoft Graph
description: Описывается перенос приложений API Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 884802fafcccf4408b84da96f6c4f94818e31b16
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234042"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a><span data-ttu-id="54bb8-103">Миграция использования клиентской библиотеки .NET в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="54bb8-103">Migrate .NET client library use to Microsoft Graph</span></span>

<span data-ttu-id="54bb8-104">Эта статья входит в *Шаг 3: Ознакомьтесь со сведениями о* [процессе миграции приложений](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="54bb8-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="54bb8-105">Если ваше приложение использует клиентскую библиотеку Azure AD Graph, переключитесь на [клиентскую библиотеку Microsoft Graph .NET](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span><span class="sxs-lookup"><span data-stu-id="54bb8-105">If your app currently uses the Azure AD Graph client library, switch to the [Microsoft Graph .NET client library](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span></span>

><span data-ttu-id="54bb8-106">NOTE: клиентская библиотека Microsoft Graph .NET поддерживается только для .NET Framework 4,5 и .NET Standard 1,1.</span><span class="sxs-lookup"><span data-stu-id="54bb8-106">NOTE: The Microsoft Graph .NET client library is only supported for .NET Framework 4.5 and .NET Standard 1.1.</span></span>  <span data-ttu-id="54bb8-107">Тем не менее, ознакомьтесь со статьей клиентская библиотека .NET для Microsoft Graph, чтобы получить последние сведения о поддержке.</span><span class="sxs-lookup"><span data-stu-id="54bb8-107">However please consult Microsoft Graph .NET client library for the latest support information.</span></span>

<span data-ttu-id="54bb8-108">В этой статье мы рассмотрим некоторые общие действия для перехода на клиентскую библиотеку Microsoft Graph .NET:</span><span class="sxs-lookup"><span data-stu-id="54bb8-108">Here, we'll look at some general steps to migrate over to the Microsoft Graph .NET client library:</span></span>

- <span data-ttu-id="54bb8-109">Создание клиента Microsoft Graph с помощью маркера доступа (который можно получить с помощью ADAL или MSAL)</span><span class="sxs-lookup"><span data-stu-id="54bb8-109">How to create a Microsoft Graph client, given an access token (that you can acquire using ADAL or MSAL)</span></span>
- <span data-ttu-id="54bb8-110">Как формулировать запросы</span><span class="sxs-lookup"><span data-stu-id="54bb8-110">How to formulate requests</span></span>
- <span data-ttu-id="54bb8-111">Использование построителей запросов</span><span class="sxs-lookup"><span data-stu-id="54bb8-111">How to use query builders</span></span>
- <span data-ttu-id="54bb8-112">Обработка коллекций и разбиения по страницам</span><span class="sxs-lookup"><span data-stu-id="54bb8-112">How to handle collections and paging</span></span>  

## <a name="overview-of-the-migration-steps"></a><span data-ttu-id="54bb8-113">Обзор этапов миграции</span><span class="sxs-lookup"><span data-stu-id="54bb8-113">Overview of the migration steps</span></span>

<span data-ttu-id="54bb8-114">В следующих шагах предполагается, что ваше приложение уже использует ADAL для получения маркеров доступа для вызова Azure AD Graph, и теперь вы будете продолжать использовать ADAL.</span><span class="sxs-lookup"><span data-stu-id="54bb8-114">The following steps assume your app is already using ADAL to acquire access tokens to call Azure AD Graph, and that for now you will continue to use ADAL.</span></span> <span data-ttu-id="54bb8-115">Переключение на MSAL можно выполнить в отдельном действии, описанном в статье [Переход на MSAL](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal).</span><span class="sxs-lookup"><span data-stu-id="54bb8-115">Switching to MSAL can be done as a separate step described in [migrating to MSAL](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal).</span></span>

1. <span data-ttu-id="54bb8-116">Чтобы получить маркер доступа к Microsoft Graph, обновите **resourceurl экземпляром** с `https://graph.windows.net` " `https://graph.microsoft.com`на".</span><span class="sxs-lookup"><span data-stu-id="54bb8-116">To acquire an access token to Microsoft Graph, update **resourceUrl** from `https://graph.windows.net` to `https://graph.microsoft.com`.</span></span>

2. <span data-ttu-id="54bb8-117">В приложении обновите ссылки на клиентскую библиотеку Microsoft Graph, изменив следующие компоненты:</span><span class="sxs-lookup"><span data-stu-id="54bb8-117">In your app, update references to the Microsoft Graph client library by changing:</span></span>

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    <span data-ttu-id="54bb8-118">Кому:</span><span class="sxs-lookup"><span data-stu-id="54bb8-118">To:</span></span>

    ``` csharp
    using Microsoft.Graph;
    ```

3. <span data-ttu-id="54bb8-119">С помощью диспетчера пакетов Скачайте и обновите [пакет NuGet для Microsoft Graph](https://www.nuget.org/packages/Microsoft.Graph/) и зависимости обновлений.</span><span class="sxs-lookup"><span data-stu-id="54bb8-119">Use your package manager to download and update the [Microsoft Graph NuGet package](https://www.nuget.org/packages/Microsoft.Graph/) and update dependencies.</span></span>

4. <span data-ttu-id="54bb8-120">Обновите свой конструктор клиента, чтобы `GraphServiceClient`создать объект a `ActiveDirectoryClient`, а не.</span><span class="sxs-lookup"><span data-stu-id="54bb8-120">Update your client constructor to create a `GraphServiceClient`, rather than `ActiveDirectoryClient`.</span></span>  <span data-ttu-id="54bb8-121">Следующие фрагменты кода предполагают, что ваше приложение использует `AcquireTokenAsyncForUser()` метод для получения новых маркеров.</span><span class="sxs-lookup"><span data-stu-id="54bb8-121">The following code snippets assume your app is using the `AcquireTokenAsyncForUser()` method to acquire new tokens.</span></span> <span data-ttu-id="54bb8-122">Определение этого метода можно найти в [образце Active Directory — DotNet — графапи — Console](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span><span class="sxs-lookup"><span data-stu-id="54bb8-122">You can find a definition for this method as part of the [active-directory-dotnet-graphapi-console sample](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span></span>

    <span data-ttu-id="54bb8-123">Настройки</span><span class="sxs-lookup"><span data-stu-id="54bb8-123">Change:</span></span>

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () => await AcquireTokenAsyncForUser());
    ```

    <span data-ttu-id="54bb8-124">Кому:</span><span class="sxs-lookup"><span data-stu-id="54bb8-124">To:</span></span>

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    <span data-ttu-id="54bb8-125">Для клиентской библиотеки Microsoft Graph `serviceRoot` значение также включает номер версии.</span><span class="sxs-lookup"><span data-stu-id="54bb8-125">For Microsoft Graph client library, the `serviceRoot` value also includes the version number.</span></span> <span data-ttu-id="54bb8-126">В настоящее время это `https://graph.microsoft.com/v1.0`значение.</span><span class="sxs-lookup"><span data-stu-id="54bb8-126">Currently, that value is `https://graph.microsoft.com/v1.0`.</span></span>

5. <span data-ttu-id="54bb8-127">Обновление запросов на использование синтаксиса построителя запросов клиентов Microsoft Graph путем изменения следующих параметров:</span><span class="sxs-lookup"><span data-stu-id="54bb8-127">Update requests to use the Microsoft Graph client request builder syntax, by changing:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    <span data-ttu-id="54bb8-128">Кому:</span><span class="sxs-lookup"><span data-stu-id="54bb8-128">To:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    ><span data-ttu-id="54bb8-129">В клиентской библиотеке Azure AD Graph поддерживался синтаксис запросов на основе LINQ.</span><span class="sxs-lookup"><span data-stu-id="54bb8-129">The Azure AD Graph client library supported LINQ-based query syntax.</span></span> <span data-ttu-id="54bb8-130">Однако клиентская библиотека Microsoft Graph не поддерживает эту функции.</span><span class="sxs-lookup"><span data-stu-id="54bb8-130">However, the Microsoft Graph client library does not.</span></span>  <span data-ttu-id="54bb8-131">Следовательно, вам потребуется преобразовать нужные запросы в другое выражение для RESTFUL.</span><span class="sxs-lookup"><span data-stu-id="54bb8-131">Consequently, you'll need to convert the relevant queries to a more RESTful expression.</span></span>  

    <span data-ttu-id="54bb8-132">Для этого измените следующее:</span><span class="sxs-lookup"><span data-stu-id="54bb8-132">To do so, change:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    <span data-ttu-id="54bb8-133">Кому:</span><span class="sxs-lookup"><span data-stu-id="54bb8-133">To:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. <span data-ttu-id="54bb8-134">Если страницы кода проходят через коллекции, внесите следующие небольшие изменения.</span><span class="sxs-lookup"><span data-stu-id="54bb8-134">If your code pages through collections, make the following minor adjustments.</span></span> <span data-ttu-id="54bb8-135">В следующем примере сравниваются и сравниваются получение группы и разбиение по страницам с разбивкой по 5 за раз.</span><span class="sxs-lookup"><span data-stu-id="54bb8-135">The following example compares and contrasts fetching a group and paging through its members, 5 at a time.</span></span> <span data-ttu-id="54bb8-136">Хотя код для Azure AD Graph требует конструкцию для извлечения членов группы, у Microsoft Graph нет такого требования.</span><span class="sxs-lookup"><span data-stu-id="54bb8-136">While the code for Azure AD Graph requires a fetcher construct in order to fetch a group's members, Microsoft Graph has no such requirement.</span></span> <span data-ttu-id="54bb8-137">Кроме того, код является относительно похожим.</span><span class="sxs-lookup"><span data-stu-id="54bb8-137">Other than that, the code is relatively similar.</span></span>  <span data-ttu-id="54bb8-138">Чтобы быть кратким, отображаются только пользовательские элементы, условия try/catch и условия ошибок не отображаются, а фрагменты кода предназначены для однопотоковой консоли приложения.</span><span class="sxs-lookup"><span data-stu-id="54bb8-138">To be concise, only user members are displayed, try/catch and error conditions are not shown, and the code snippets are for a single-threaded console app.</span></span>

    <span data-ttu-id="54bb8-139">Например, измените следующий код с помощью клиентской библиотеки .NET для Azure AD Graph:</span><span class="sxs-lookup"><span data-stu-id="54bb8-139">As an example, change the following code using the Azure AD Graph .NET client library:</span></span>

    ```csharp
    Group retrievedGroup = client.Groups.
        Where(g => g.ObjectId.Equals(id)).ExecuteAsync().Result;
    IGroupFetcher retrievedGroupFetcher = (IGroupFetcher) retrievedGroup;

    var membersPage = retrievedGroupFetcher.Members.Take(5).ExecuteAsync().Result;
    Console.WriteLine(" Members:");
    do
    {
        List<IDirectoryObject> members = membersPage.CurrentPage.ToList();
        foreach (IDirectoryObject member in members)
        {
            if (member is User)
            {
                User memberUser = (User)member;
                Console.WriteLine("        User: {0} ", memberUser.DisplayName);
            }
        }
        membersPage = membersPage.GetNextPageAsync().Result;
    } while (membersPage != null);

    ```

    <span data-ttu-id="54bb8-140">Следующий код с помощью клиентской библиотеки .NET Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="54bb8-140">To the following code using the Microsoft Graph .NET client library:</span></span>

    ```csharp
    var membersPage = client.Groups[id].Members.Request().Top(5).GetAsync().Result;
    Console.WriteLine(" Members:");
    do
    {
        List<DirectoryObject> members = membersPage.CurrentPage.ToList();
        foreach (DirectoryObject member in members)
        {
            if (member is User)
            {
                User memberUser = (User)member;
                Console.WriteLine("        User: {0} ", memberUser.DisplayName);
            }
        }
        if (membersPage.NextPageRequest != null)
            membersPage = membersPage.NextPageRequest.GetAsync().Result;
        else membersPage = null;
    } while (membersPage != null);

    ```

7. <span data-ttu-id="54bb8-141">Построение и устранение ошибок ресурсов, свойств, навигации и действий служб, обычно связанных с изменением имен.</span><span class="sxs-lookup"><span data-stu-id="54bb8-141">Build and fix any resource, property, navigation, and service action errors, generally related to name changes.</span></span>

## <a name="see-also"></a><span data-ttu-id="54bb8-142">См. также</span><span class="sxs-lookup"><span data-stu-id="54bb8-142">See also</span></span>

<span data-ttu-id="54bb8-143">[Приложение фрагментов кода консоли C#](https://github.com/microsoftgraph/console-csharp-snippets-sample) выделяет дополнительные различия между клиентской библиотекой Microsoft Graph и клиентской библиотекой Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="54bb8-143">The [C# console snippets app](https://github.com/microsoftgraph/console-csharp-snippets-sample) highlights more of the differences between Microsoft Graph client library and Azure AD Graph client library.</span></span>

<span data-ttu-id="54bb8-144">Клиентская библиотека Azure AD Graph поддерживает только платформу .NET.</span><span class="sxs-lookup"><span data-stu-id="54bb8-144">The Azure AD Graph client library supports only the .NET platform.</span></span>  <span data-ttu-id="54bb8-145">Тем не менее, клиентская библиотека Microsoft Graph поддерживает дополнительные [платформы и языки](/graph) , которые могут оказаться более удобными для ваших решений.</span><span class="sxs-lookup"><span data-stu-id="54bb8-145">However, Microsoft Graph client library supports additional [platforms and languages](/graph) that you may find more useful for your solutions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="54bb8-146">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="54bb8-146">Next Steps</span></span>

- <span data-ttu-id="54bb8-147">Узнайте, как [развертывать, тестировать и расширять](/graph/migrate-azure-ad-graph-deploy-test-extend) приложения, перенесенные в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="54bb8-147">Learn how to [deploy, test, and extend](/graph/migrate-azure-ad-graph-deploy-test-extend) apps you've migrated to Microsoft Graph.</span></span>
- <span data-ttu-id="54bb8-148">Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="54bb8-148">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="54bb8-149">Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .</span><span class="sxs-lookup"><span data-stu-id="54bb8-149">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
