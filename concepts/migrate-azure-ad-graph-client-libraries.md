---
title: Перенос Azure Active Directory (Azure AD) Graph приложений .NET в Microsoft Graph
description: Описывает, как перенести приложения Azure Active Directory (Azure AD) Graph API в API Microsoft Graph API.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: b774b14ffc480ca889392c31b2090c7578dfa207
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135965"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a>Перенос использования клиентской библиотеки .NET в Microsoft Graph

Эта статья является *частью шага 3: просмотрите* сведения о процессе переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)

Если ваше приложение в настоящее время использует Azure Active Directory (Azure AD) Graph клиентской библиотеке, переключиться на клиентскую библиотеку [Microsoft Graph .NET.](https://github.com/microsoftgraph/msgraph-sdk-dotnet)

>ПРИМЕЧАНИЕ. Клиентская библиотека Microsoft Graph .NET поддерживается только для платформа .NET Framework 4.5 и .NET Standard 1.1.  Однако для получения последних сведений о поддержке обратитесь в клиентскую библиотеку Microsoft Graph .NET.

Здесь мы посмотрим на некоторые общие действия по переносу в клиентскую библиотеку Microsoft Graph .NET:

- Создание клиента microsoft Graph с помощью маркера доступа (который можно приобрести с помощью библиотеки проверки подлинности Azure Active Directory (ADAL) или Microsoft Authentication Library (MSAL))
- Как сформулировать запросы
- Использование строителей запросов
- Обработка коллекций и paging  

## <a name="overview-of-the-migration-steps"></a>Обзор этапов миграции

Следующие действия предполагают, что ваше приложение уже использует ADAL для приобретения маркеров доступа для вызова Azure AD Graph, и что пока вы будете продолжать использовать ADAL. Переход на MSAL можно сделать в качестве отдельного шага, описанного при [миграции в MSAL.](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal)

1. Чтобы приобрести маркер доступа к Microsoft Graph, **обнови ресурсUrl** от `https://graph.windows.net` до `https://graph.microsoft.com` .

2. В приложении обновляйте ссылки на клиентскую библиотеку Microsoft Graph, изменяя:

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    Кому:

    ``` csharp
    using Microsoft.Graph;
    ```

3. Используйте диспетчер пакетов для скачивания и обновления зависимостей [Graph NuGet microsoft и](https://www.nuget.org/packages/Microsoft.Graph/) обновления.

4. Обновите конструктор клиента, чтобы создать `GraphServiceClient` , а не `ActiveDirectoryClient` .  В следующих фрагментах кода предполагается, что приложение использует метод `AcquireTokenAsyncForUser()` для приобретения новых маркеров. Определение этого метода можно найти в примере [active-directory-dotnet-graphapi-console.](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs)

    Изменение:

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () => await AcquireTokenAsyncForUser());
    ```

    Кому:

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    Для клиентской Graph Майкрософт значение `serviceRoot` также включает номер версии. В настоящее время это значение `https://graph.microsoft.com/v1.0` .

5. Обновив запросы на использование синтаксиса Graph клиента, изменяя:

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    Кому:

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    >Клиентская библиотека Azure AD Graph поддерживает синтаксис запросов на основе LINQ. Однако в клиентской Graph Майкрософт нет.  Следовательно, необходимо преобразовать соответствующие запросы в более reSTful выражение.  

    Чтобы сделать это, измените:

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    Кому:

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. Если код страницы через коллекции, внести следующие незначительные изменения. В следующем примере сравнивается и контрастирует извлечение группы и прогона через ее членов по 5 за раз. Несмотря на то, что для Graph Azure AD требуется построение выборщика для получения членов группы, microsoft Graph не имеет такого требования. Кроме этого, код является относительно похожим.  Чтобы быть кратким, отображаются только пользователи, не отображаются условия try/catch и error, а фрагменты кода — для однопотокого приложения консоли.

    Например, измените следующий код с помощью клиентской библиотеки Azure AD Graph .NET:

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

    К следующему коду с помощью клиентской библиотеки Microsoft Graph .NET:

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

7. Создайте и исправьте все ошибки в действиях ресурса, свойства, навигации и службы, обычно связанные с изменениями имен.

## <a name="see-also"></a>См. также

Приложение [C#](https://github.com/microsoftgraph/console-csharp-snippets-sample) консоли выделяет больше различий между клиентской библиотекой Microsoft Graph и Azure AD Graph клиентской библиотекой.

Клиентская Graph Azure AD поддерживает только платформу .NET.  Однако клиентская Graph Майкрософт поддерживает дополнительные [](/graph) платформы и языки, которые могут оказаться более полезными для ваших решений.

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как [развертывать, тестировать](./migrate-azure-ad-graph-deploy-test-extend.md) и расширять приложения, которые вы мигрировали в Microsoft Graph.
- Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.
