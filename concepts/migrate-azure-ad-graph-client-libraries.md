---
title: Перенос приложений Azure AD Graph .NET в Microsoft Graph
description: Описывает перенос приложений API API Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 286f631a9d5787d972e8d7db2559b0c359384c75
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761299"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a><span data-ttu-id="79527-103">Перенос использования клиентской библиотеки .NET в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="79527-103">Migrate .NET client library use to Microsoft Graph</span></span>

<span data-ttu-id="79527-104">Эта статья является *частью шага 3: просмотрите* сведения о процессе переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="79527-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="79527-105">Если ваше приложение в настоящее время использует клиентскую библиотеку Azure AD Graph, переключиться на клиентскую библиотеку [Microsoft Graph .NET.](https://github.com/microsoftgraph/msgraph-sdk-dotnet)</span><span class="sxs-lookup"><span data-stu-id="79527-105">If your app currently uses the Azure AD Graph client library, switch to the [Microsoft Graph .NET client library](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span></span>

><span data-ttu-id="79527-106">ПРИМЕЧАНИЕ. Клиентская библиотека Microsoft Graph .NET поддерживается только для платформа .NET Framework 4.5 и .NET Standard 1.1.</span><span class="sxs-lookup"><span data-stu-id="79527-106">NOTE: The Microsoft Graph .NET client library is only supported for .NET Framework 4.5 and .NET Standard 1.1.</span></span>  <span data-ttu-id="79527-107">Однако для получения последних сведений о поддержке обратитесь в клиентскую библиотеку Microsoft Graph .NET.</span><span class="sxs-lookup"><span data-stu-id="79527-107">However please consult Microsoft Graph .NET client library for the latest support information.</span></span>

<span data-ttu-id="79527-108">Здесь мы посмотрим на некоторые общие действия для переноса в клиентскую библиотеку Microsoft Graph .NET:</span><span class="sxs-lookup"><span data-stu-id="79527-108">Here, we'll look at some general steps to migrate over to the Microsoft Graph .NET client library:</span></span>

- <span data-ttu-id="79527-109">Создание клиента Microsoft Graph с помощью маркера доступа (который можно приобрести с помощью ADAL или MSAL)</span><span class="sxs-lookup"><span data-stu-id="79527-109">How to create a Microsoft Graph client, given an access token (that you can acquire using ADAL or MSAL)</span></span>
- <span data-ttu-id="79527-110">Как сформулировать запросы</span><span class="sxs-lookup"><span data-stu-id="79527-110">How to formulate requests</span></span>
- <span data-ttu-id="79527-111">Использование строителей запросов</span><span class="sxs-lookup"><span data-stu-id="79527-111">How to use query builders</span></span>
- <span data-ttu-id="79527-112">Обработка коллекций и paging</span><span class="sxs-lookup"><span data-stu-id="79527-112">How to handle collections and paging</span></span>  

## <a name="overview-of-the-migration-steps"></a><span data-ttu-id="79527-113">Обзор этапов миграции</span><span class="sxs-lookup"><span data-stu-id="79527-113">Overview of the migration steps</span></span>

<span data-ttu-id="79527-114">Следующие действия предполагают, что ваше приложение уже использует ADAL для приобретения маркеров доступа для вызова Azure AD Graph, и что пока вы будете продолжать использовать ADAL.</span><span class="sxs-lookup"><span data-stu-id="79527-114">The following steps assume your app is already using ADAL to acquire access tokens to call Azure AD Graph, and that for now you will continue to use ADAL.</span></span> <span data-ttu-id="79527-115">Переход на MSAL можно сделать в качестве отдельного шага, описанного при [миграции в MSAL.](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal)</span><span class="sxs-lookup"><span data-stu-id="79527-115">Switching to MSAL can be done as a separate step described in [migrating to MSAL](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal).</span></span>

1. <span data-ttu-id="79527-116">Чтобы приобрести маркер доступа к Microsoft Graph, **обнови ресурсUrl** от `https://graph.windows.net` до `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="79527-116">To acquire an access token to Microsoft Graph, update **resourceUrl** from `https://graph.windows.net` to `https://graph.microsoft.com`.</span></span>

2. <span data-ttu-id="79527-117">В приложении обновляйте ссылки на клиентскую библиотеку Microsoft Graph, изменяя:</span><span class="sxs-lookup"><span data-stu-id="79527-117">In your app, update references to the Microsoft Graph client library by changing:</span></span>

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    <span data-ttu-id="79527-118">Кому:</span><span class="sxs-lookup"><span data-stu-id="79527-118">To:</span></span>

    ``` csharp
    using Microsoft.Graph;
    ```

3. <span data-ttu-id="79527-119">Используйте диспетчер пакетов для загрузки и обновления пакета [Microsoft Graph NuGet](https://www.nuget.org/packages/Microsoft.Graph/) и обновления зависимостей.</span><span class="sxs-lookup"><span data-stu-id="79527-119">Use your package manager to download and update the [Microsoft Graph NuGet package](https://www.nuget.org/packages/Microsoft.Graph/) and update dependencies.</span></span>

4. <span data-ttu-id="79527-120">Обновите конструктор клиента, чтобы создать `GraphServiceClient` , а не `ActiveDirectoryClient` .</span><span class="sxs-lookup"><span data-stu-id="79527-120">Update your client constructor to create a `GraphServiceClient`, rather than `ActiveDirectoryClient`.</span></span>  <span data-ttu-id="79527-121">В следующих фрагментах кода предполагается, что приложение использует метод `AcquireTokenAsyncForUser()` для приобретения новых маркеров.</span><span class="sxs-lookup"><span data-stu-id="79527-121">The following code snippets assume your app is using the `AcquireTokenAsyncForUser()` method to acquire new tokens.</span></span> <span data-ttu-id="79527-122">Определение этого метода можно найти в примере [active-directory-dotnet-graphapi-console.](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs)</span><span class="sxs-lookup"><span data-stu-id="79527-122">You can find a definition for this method as part of the [active-directory-dotnet-graphapi-console sample](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span></span>

    <span data-ttu-id="79527-123">Изменение:</span><span class="sxs-lookup"><span data-stu-id="79527-123">Change:</span></span>

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () => await AcquireTokenAsyncForUser());
    ```

    <span data-ttu-id="79527-124">Кому:</span><span class="sxs-lookup"><span data-stu-id="79527-124">To:</span></span>

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    <span data-ttu-id="79527-125">Для клиентской библиотеки Microsoft Graph значение `serviceRoot` также включает номер версии.</span><span class="sxs-lookup"><span data-stu-id="79527-125">For Microsoft Graph client library, the `serviceRoot` value also includes the version number.</span></span> <span data-ttu-id="79527-126">В настоящее время это значение `https://graph.microsoft.com/v1.0` .</span><span class="sxs-lookup"><span data-stu-id="79527-126">Currently, that value is `https://graph.microsoft.com/v1.0`.</span></span>

5. <span data-ttu-id="79527-127">Обновив запросы на использование синтаксиса строителя клиентских запросов Microsoft Graph, изменяя:</span><span class="sxs-lookup"><span data-stu-id="79527-127">Update requests to use the Microsoft Graph client request builder syntax, by changing:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    <span data-ttu-id="79527-128">Кому:</span><span class="sxs-lookup"><span data-stu-id="79527-128">To:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    ><span data-ttu-id="79527-129">Клиентская библиотека Azure AD Graph поддерживает синтаксис запросов на основе LINQ.</span><span class="sxs-lookup"><span data-stu-id="79527-129">The Azure AD Graph client library supported LINQ-based query syntax.</span></span> <span data-ttu-id="79527-130">Однако клиентская библиотека Microsoft Graph этого не делает.</span><span class="sxs-lookup"><span data-stu-id="79527-130">However, the Microsoft Graph client library does not.</span></span>  <span data-ttu-id="79527-131">Следовательно, необходимо преобразовать соответствующие запросы в более reSTful выражение.</span><span class="sxs-lookup"><span data-stu-id="79527-131">Consequently, you'll need to convert the relevant queries to a more RESTful expression.</span></span>  

    <span data-ttu-id="79527-132">Чтобы сделать это, измените:</span><span class="sxs-lookup"><span data-stu-id="79527-132">To do so, change:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    <span data-ttu-id="79527-133">Кому:</span><span class="sxs-lookup"><span data-stu-id="79527-133">To:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. <span data-ttu-id="79527-134">Если код страницы через коллекции, внести следующие незначительные изменения.</span><span class="sxs-lookup"><span data-stu-id="79527-134">If your code pages through collections, make the following minor adjustments.</span></span> <span data-ttu-id="79527-135">В следующем примере сравнивается и контрастирует извлечение группы и прогона через ее членов по 5 за раз.</span><span class="sxs-lookup"><span data-stu-id="79527-135">The following example compares and contrasts fetching a group and paging through its members, 5 at a time.</span></span> <span data-ttu-id="79527-136">Хотя для кода Azure AD Graph требуется конструкция выборщика для получения участников группы, Microsoft Graph не имеет такого требования.</span><span class="sxs-lookup"><span data-stu-id="79527-136">While the code for Azure AD Graph requires a fetcher construct in order to fetch a group's members, Microsoft Graph has no such requirement.</span></span> <span data-ttu-id="79527-137">Кроме этого, код является относительно похожим.</span><span class="sxs-lookup"><span data-stu-id="79527-137">Other than that, the code is relatively similar.</span></span>  <span data-ttu-id="79527-138">Чтобы быть кратким, отображаются только пользователи, не отображаются условия try/catch и error, а фрагменты кода — для однопотокого приложения консоли.</span><span class="sxs-lookup"><span data-stu-id="79527-138">To be concise, only user members are displayed, try/catch and error conditions are not shown, and the code snippets are for a single-threaded console app.</span></span>

    <span data-ttu-id="79527-139">Например, измените следующий код с помощью клиентской библиотеки Azure AD Graph .NET:</span><span class="sxs-lookup"><span data-stu-id="79527-139">As an example, change the following code using the Azure AD Graph .NET client library:</span></span>

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

    <span data-ttu-id="79527-140">К следующему коду с помощью клиентской библиотеки Microsoft Graph .NET:</span><span class="sxs-lookup"><span data-stu-id="79527-140">To the following code using the Microsoft Graph .NET client library:</span></span>

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

7. <span data-ttu-id="79527-141">Создайте и исправьте все ошибки в действиях ресурса, свойства, навигации и службы, обычно связанные с изменениями имен.</span><span class="sxs-lookup"><span data-stu-id="79527-141">Build and fix any resource, property, navigation, and service action errors, generally related to name changes.</span></span>

## <a name="see-also"></a><span data-ttu-id="79527-142">См. также</span><span class="sxs-lookup"><span data-stu-id="79527-142">See also</span></span>

<span data-ttu-id="79527-143">Фрагменты [C#](https://github.com/microsoftgraph/console-csharp-snippets-sample) консоли больше подчеркивают различия между клиентской библиотекой Microsoft Graph и клиентской библиотекой Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="79527-143">The [C# console snippets app](https://github.com/microsoftgraph/console-csharp-snippets-sample) highlights more of the differences between Microsoft Graph client library and Azure AD Graph client library.</span></span>

<span data-ttu-id="79527-144">Клиентская библиотека Azure AD Graph поддерживает только платформу .NET.</span><span class="sxs-lookup"><span data-stu-id="79527-144">The Azure AD Graph client library supports only the .NET platform.</span></span>  <span data-ttu-id="79527-145">Однако клиентская библиотека Microsoft Graph поддерживает дополнительные [платформы](/graph) и языки, которые могут оказаться более полезными для ваших решений.</span><span class="sxs-lookup"><span data-stu-id="79527-145">However, Microsoft Graph client library supports additional [platforms and languages](/graph) that you may find more useful for your solutions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="79527-146">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="79527-146">Next Steps</span></span>

- <span data-ttu-id="79527-147">Узнайте, как [развертывать, тестировать](./migrate-azure-ad-graph-deploy-test-extend.md) и расширять приложения, перенесенные в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="79527-147">Learn how to [deploy, test, and extend](./migrate-azure-ad-graph-deploy-test-extend.md) apps you've migrated to Microsoft Graph.</span></span>
- <span data-ttu-id="79527-148">Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.</span><span class="sxs-lookup"><span data-stu-id="79527-148">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>
