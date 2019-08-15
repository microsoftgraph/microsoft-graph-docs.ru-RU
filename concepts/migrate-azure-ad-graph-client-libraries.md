---
title: Перенос приложений .NET для Azure AD Graph в Microsoft Graph
description: Описывается перенос приложений API Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc48be3712b0d3b03e9799559aac4d6ae812b5d0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422179"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a>Миграция использования клиентской библиотеки .NET в Microsoft Graph

Эта статья входит в *Шаг 3: Ознакомьтесь со сведениями о* [процессе миграции приложений](migrate-azure-ad-graph-planning-checklist.md).

Если ваше приложение использует клиентскую библиотеку Azure AD Graph, переключитесь на [клиентскую библиотеку Microsoft Graph .NET](https://github.com/microsoftgraph/msgraph-sdk-dotnet).

>NOTE: клиентская библиотека Microsoft Graph .NET поддерживается только для .NET Framework 4,5 и .NET Standard 1,1.  Тем не менее, ознакомьтесь со статьей клиентская библиотека .NET для Microsoft Graph, чтобы получить последние сведения о поддержке.

В этой статье мы рассмотрим некоторые общие действия для перехода на клиентскую библиотеку Microsoft Graph .NET:

- Создание клиента Microsoft Graph с помощью маркера доступа (который можно получить с помощью ADAL или MSAL)
- Как формулировать запросы
- Использование построителей запросов
- Обработка коллекций и разбиения по страницам  

## <a name="overview-of-the-migration-steps"></a>Обзор этапов миграции

В следующих шагах предполагается, что ваше приложение уже использует ADAL для получения маркеров доступа для вызова Azure AD Graph, и теперь вы будете продолжать использовать ADAL. Переключение на MSAL можно выполнить в отдельном действии, описанном в статье [Переход на MSAL](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal).

1. Чтобы получить маркер доступа к Microsoft Graph, обновите **resourceurl экземпляром** с `https://graph.windows.net` " `https://graph.microsoft.com`на".

2. В приложении обновите ссылки на клиентскую библиотеку Microsoft Graph, изменив следующие компоненты:

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    Кому:

    ``` csharp
    using Microsoft.Graph;
    ```

3. С помощью диспетчера пакетов Скачайте и обновите [пакет NuGet для Microsoft Graph](https://www.nuget.org/packages/Microsoft.Graph/) и зависимости обновлений.

4. Обновите свой конструктор клиента, чтобы `GraphServiceClient`создать объект a `ActiveDirectoryClient`, а не.  Следующие фрагменты кода предполагают, что ваше приложение использует `AcquireTokenAsyncForUser()` метод для получения новых маркеров. Определение этого метода можно найти в [образце Active Directory — DotNet — графапи — Console](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).

    Настройки

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

    Для клиентской библиотеки Microsoft Graph `serviceRoot` значение также включает номер версии. В настоящее время это `https://graph.microsoft.com/v1.0`значение.

5. Обновление запросов на использование синтаксиса построителя запросов клиентов Microsoft Graph путем изменения следующих параметров:

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    Кому:

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    [!NOTE]
    В клиентской библиотеке Azure AD Graph поддерживался синтаксис запросов на основе LINQ. Однако клиентская библиотека Microsoft Graph не поддерживает эту функции.  Следовательно, вам потребуется преобразовать нужные запросы в другое выражение для RESTFUL.  

    Для этого измените следующее:

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    Кому:

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. Если страницы кода проходят через коллекции, внесите следующие небольшие изменения. В следующем примере сравниваются и сравниваются получение группы и разбиение по страницам с разбивкой по 5 за раз. Хотя код для Azure AD Graph требует конструкцию для извлечения членов группы, у Microsoft Graph нет такого требования. Кроме того, код является относительно похожим.  Чтобы быть кратким, отображаются только пользовательские элементы, условия try/catch и условия ошибок не отображаются, а фрагменты кода предназначены для однопотоковой консоли приложения.

    Например, измените следующий код с помощью клиентской библиотеки .NET для Azure AD Graph:

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

    Следующий код с помощью клиентской библиотеки .NET Microsoft Graph:

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

7. Построение и устранение ошибок ресурсов, свойств, навигации и действий служб, обычно связанных с изменением имен.

## <a name="see-also"></a>См. также

[Приложение фрагментов кода консоли C#](https://github.com/microsoftgraph/console-csharp-snippets-sample) выделяет дополнительные различия между клиентской библиотекой Microsoft Graph и клиентской библиотекой Azure AD Graph.

Клиентская библиотека Azure AD Graph поддерживает только платформу .NET.  Тем не менее, клиентская библиотека Microsoft Graph поддерживает дополнительные [платформы и языки](/graph) , которые могут оказаться более удобными для ваших решений.

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как [развертывать, тестировать и расширять](/graph/migrate-azure-ad-graph-deploy-test-extend) приложения, перенесенные в Microsoft Graph.
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .
