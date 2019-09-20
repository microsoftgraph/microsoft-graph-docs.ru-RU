---
title: 'Разбиение данных Microsoft Graph по страницам в приложении '
description: 'свойство odata.nextLink в ответе, содержащем URL-адрес следующей страницы результатов. '
author: piotrci
localization_priority: Priority
scenarios: getting-started
ms.custom: graphiamtop20
ms.openlocfilehash: 16c165be9afe53a6540f1c5fe7faa41d88cb21b3
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37054105"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a><span data-ttu-id="f52db-103">Разбиение данных Microsoft Graph по страницам в приложении</span><span class="sxs-lookup"><span data-stu-id="f52db-103">Paging Microsoft Graph data in your app</span></span> 

<span data-ttu-id="f52db-p101">Некоторые запросы к Microsoft Graph возвращают несколько страниц данных. Это происходит из-за разбиения по страницам на стороне сервера или из-за использования параметра `$top`, который ограничивает размер страниц в запросе. Когда результирующий набор занимает несколько страниц, Microsoft Graph в ответ возвращает свойство `@odata.nextLink`, содержащее URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="f52db-p101">Some queries against Microsoft Graph return multiple pages of data either due to server-side paging or due to the use of the `$top` query parameter to specifically limit the page size in a request. When a result set spans multiple pages, Microsoft Graph returns an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> 

<span data-ttu-id="f52db-106">Например, в приведенном ниже URL-адресе запрашивается список всех пользователей в организации, при этом с помощью параметра запроса `$top` указан размер страницы — 5:</span><span class="sxs-lookup"><span data-stu-id="f52db-106">For example, the following URL requests all the users in an organization with a page size of 5, specified with the `$top` query parameter:</span></span>

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

<span data-ttu-id="f52db-107">Если результат содержит более пяти пользователей, Microsoft Graph возвращает свойство `@odata:nextLink` (как показанный ниже пример) вместе с первой страницей пользователей.</span><span class="sxs-lookup"><span data-stu-id="f52db-107">If the result contains more than five users, Microsoft Graph will return an `@odata:nextLink` property similar to the following along with the first page of users.</span></span>

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

<span data-ttu-id="f52db-108">Следующую страницу результатов можно получить, отправив значение URL-адреса свойства `@odata:nextLink` в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f52db-108">You can retrieve the next page of results by sending the URL value of the `@odata:nextLink` property to Microsoft Graph.</span></span> 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

<span data-ttu-id="f52db-109">В каждом ответе Microsoft Graph будет возвращать ссылку на следующую страницу данных в свойстве `@odata:nextLink`, пока не будут прочитаны все страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="f52db-109">Microsoft Graph will continue to return a reference to the next page of data in the `@odata:nextLink` property with each response until all pages of the result have been read.</span></span>

><span data-ttu-id="f52db-110">**Важно!** При запросе следующей страницы результатов в свойство `@odata:nextLink` следует включить полный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="f52db-110">**Important:** You should include the entire URL in the `@odata:nextLink` property in your request for the next page of results.</span></span> <span data-ttu-id="f52db-111">В зависимости от API, к которому выполняется запрос, значение URL-адреса `@odata:nextLink` будет содержать один из двух параметров запроса: `$skiptoken` или `$skip`.</span><span class="sxs-lookup"><span data-stu-id="f52db-111">Depending on the API that the query is being performed against, the `@odata:nextLink` URL value will contain either a `$skiptoken` or a `$skip` query parameter.</span></span> <span data-ttu-id="f52db-112">URL-адрес также содержит все остальные параметры, имеющиеся в исходном запросе.</span><span class="sxs-lookup"><span data-stu-id="f52db-112">The URL also contains all the other query parameters present in the original request.</span></span> <span data-ttu-id="f52db-113">Не пытайтесь извлечь значение `$skiptoken` или `$skip` и использовать его в другом запросе.</span><span class="sxs-lookup"><span data-stu-id="f52db-113">Do not try to extract the `$skiptoken` or `$skip` value and use it in a different request.</span></span> 

<span data-ttu-id="f52db-114">Для различных API Microsoft Graph характерны свои особенности разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="f52db-114">Paging behavior varies across different Microsoft Graph APIs.</span></span> <span data-ttu-id="f52db-115">При работе со страницами данных необходимо учитывать следующее:</span><span class="sxs-lookup"><span data-stu-id="f52db-115">Consider the following when working with paged data:</span></span>

- <span data-ttu-id="f52db-116">Разные API могут иметь различные максимальные размеры страницы и размеры страницы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f52db-116">Different APIs might have different default and maximum page sizes.</span></span>
- <span data-ttu-id="f52db-117">Различные API могут работать по-разному, если указанный (с помощью параметра запроса `$top`) размер страницы превышает максимальное значение для соответствующего API.</span><span class="sxs-lookup"><span data-stu-id="f52db-117">Different APIs might behave differently if you specify a page size (via the `$top` query parameter) that exceeds the maximum page size for that API.</span></span> <span data-ttu-id="f52db-118">В зависимости от API запрошенный размер страницы может быть проигнорирован, может быть возвращен максимальный размер страницы для соответствующего API или же Microsoft Graph может вернуть ошибку.
</span><span class="sxs-lookup"><span data-stu-id="f52db-118">Depending on the API, the requested page size might be ignored, it might default to the maximum page size for that API, or Microsoft Graph might return an error.</span></span> 
- <span data-ttu-id="f52db-p105">Некоторые ресурсы и отношения не поддерживают разбиение по страницам, например запросы к [directoryRoles](/graph/api/resources/directoryrole?view=graph-rest-1.0).
Сюда относится считывание самих объектов ролей, а также участников ролей.</span><span class="sxs-lookup"><span data-stu-id="f52db-p105">Not all resources or relationships support paging. For example, queries against [directoryRoles](/graph/api/resources/directoryrole?view=graph-rest-1.0) do not support paging. This includes reading role objects themselves as well as role members.</span></span>

## <a name="learn-more-about-paging"></a><span data-ttu-id="f52db-122">Подробнее о разбиении данных</span><span class="sxs-lookup"><span data-stu-id="f52db-122">Learn more about:</span></span>
<span data-ttu-id="f52db-123">Следующее видео познакомит вас с разбиением данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f52db-123">The following video introduces you to paging in Microsoft Graph.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/DB_NoC9a1JI]