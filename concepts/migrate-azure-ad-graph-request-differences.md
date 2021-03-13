---
title: Различия запросов между Azure AD Graph и Microsoft Graph
description: Описывает, как запросы Microsoft Graph отличаются от запросов Azure AD, что помогает перенести приложения в более новую службу..
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e30a0c98aaf7ec0d042787f511872d02529aaa5c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760667"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="fcf83-103">Различия запросов между Azure AD Graph и Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fcf83-103">Request differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="fcf83-104">Эта статья является *частью шага 1: просмотрите различия API* процесса переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="fcf83-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="fcf83-105">Microsoft Graph и API Azure AD Graph — это API REST, каждая из которых поддерживает соглашения ODATA для параметров запросов.</span><span class="sxs-lookup"><span data-stu-id="fcf83-105">Microsoft Graph and the Azure AD Graph API are both REST APIs and they each support ODATA conventions for query parameters.</span></span> <span data-ttu-id="fcf83-106">Однако синтаксис различается между этими двумя API.</span><span class="sxs-lookup"><span data-stu-id="fcf83-106">However, the syntax varies between these two APIs.</span></span>

<span data-ttu-id="fcf83-107">Используйте [обозреватель graph,](https://aka.ms/ge) чтобы попробовать эти шаблоны запросов в отношении собственных данных, так как это отличный способ узнать о различиях запросов и ответов.</span><span class="sxs-lookup"><span data-stu-id="fcf83-107">Use the [Graph Explorer](https://aka.ms/ge) to try these request patterns against your own data, as it's a great way to learn about the request and response differences.</span></span>

## <a name="basic-requests"></a><span data-ttu-id="fcf83-108">Основные запросы</span><span class="sxs-lookup"><span data-stu-id="fcf83-108">Basic requests</span></span>

<span data-ttu-id="fcf83-109">В следующей таблице выделяются основные различия запросов между двумя API:</span><span class="sxs-lookup"><span data-stu-id="fcf83-109">The following table highlights the main request differences between the two APIs:</span></span>

|<span data-ttu-id="fcf83-110">Сведения о запросе</span><span class="sxs-lookup"><span data-stu-id="fcf83-110">Request details</span></span>| <span data-ttu-id="fcf83-111">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="fcf83-111">Azure AD Graph</span></span> | <span data-ttu-id="fcf83-112">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fcf83-112">Microsoft Graph</span></span> |
|---|---|---|
|<span data-ttu-id="fcf83-113">Запрос синтаксиса</span><span class="sxs-lookup"><span data-stu-id="fcf83-113">Request syntax</span></span>| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|<span data-ttu-id="fcf83-114">Конечные &nbsp; точки службы:</span><span class="sxs-lookup"><span data-stu-id="fcf83-114">Service&nbsp;endpoints:</span></span>||
|<span data-ttu-id="fcf83-115">-&nbsp;Глобальный</span><span class="sxs-lookup"><span data-stu-id="fcf83-115">-&nbsp;Global</span></span>|`https://graph.windows.net`|`https://graph.microsoft.com`|
|<span data-ttu-id="fcf83-116">-&nbsp;США &nbsp; Gov &nbsp; L4</span><span class="sxs-lookup"><span data-stu-id="fcf83-116">-&nbsp;US&nbsp;Gov&nbsp;L4</span></span>|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|<span data-ttu-id="fcf83-117">-&nbsp;США &nbsp; Gov &nbsp; L5 &nbsp; (DOD)</span><span class="sxs-lookup"><span data-stu-id="fcf83-117">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span></span>|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|<span data-ttu-id="fcf83-118">-&nbsp;Германия</span><span class="sxs-lookup"><span data-stu-id="fcf83-118">-&nbsp;Germany</span></span>|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|<span data-ttu-id="fcf83-119">-&nbsp;Китай &nbsp; (21Vianet)</span><span class="sxs-lookup"><span data-stu-id="fcf83-119">-&nbsp;China&nbsp;(21Vianet)</span></span>| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|<span data-ttu-id="fcf83-120">{tenant_id}</span><span class="sxs-lookup"><span data-stu-id="fcf83-120">{tenant_id}</span></span>|<span data-ttu-id="fcf83-121">Укажите в запросе ID клиента.</span><span class="sxs-lookup"><span data-stu-id="fcf83-121">Specify the ID of the tenant in the request.</span></span>|<span data-ttu-id="fcf83-122">Необязательно указывать в запросе ИД клиента, так как он высвечен из маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="fcf83-122">It's optional to specify a tenant ID in the request as it is inferred from the access token.</span></span><br><br><span data-ttu-id="fcf83-123">Если указать ID клиента, он переходит между URL-адресом запроса `{version}` `{resource}` и url-адресом запроса.</span><span class="sxs-lookup"><span data-stu-id="fcf83-123">If you specify the tenant ID, it goes between the `{version}` and the `{resource}` in the request URL.</span></span>|
|<span data-ttu-id="fcf83-124">{version}</span><span class="sxs-lookup"><span data-stu-id="fcf83-124">{version}</span></span>|<span data-ttu-id="fcf83-125">Укажите версию выпуска Azure AD Graph в запросе с помощью требуемого параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="fcf83-125">Specify the release version of Azure AD Graph in the request using a required query parameter.</span></span>|<span data-ttu-id="fcf83-126">Укажите версию выпуска Microsoft Graph в запросе как часть пути URL-адреса сразу после конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="fcf83-126">Specify the release version of Microsoft Graph in the request as part of the URL path just after the service endpoint.</span></span>|

<span data-ttu-id="fcf83-127">Можно продолжать использовать те же параметры запроса в Microsoft Graph, что и Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="fcf83-127">You can continue to use the same query parameters in Microsoft Graph as Azure AD Graph.</span></span>

### <a name="example-request-comparison"></a><span data-ttu-id="fcf83-128">Сравнение примера запроса</span><span class="sxs-lookup"><span data-stu-id="fcf83-128">Example request comparison</span></span>

<span data-ttu-id="fcf83-129">Предположим, вам нужен список всех пользователей с именами, начиная с "Dan".</span><span class="sxs-lookup"><span data-stu-id="fcf83-129">Suppose you want a list of all users with names beginning with "Dan".</span></span>

<span data-ttu-id="fcf83-130">В Azure AD Graph можно использовать этот запрос:</span><span class="sxs-lookup"><span data-stu-id="fcf83-130">In Azure AD Graph, you might use this request:</span></span>

<span data-ttu-id="fcf83-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` или </span><span class="sxs-lookup"><span data-stu-id="fcf83-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` or</span></span>

`GET https://graph.windows.net/myOrganization/users?$filter=startswith(givenName,'Dan')&api-version=1.6`


<span data-ttu-id="fcf83-132">Этот запрос:</span><span class="sxs-lookup"><span data-stu-id="fcf83-132">This request:</span></span>

- <span data-ttu-id="fcf83-133">Целевые показатели версии 1.6 Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="fcf83-133">Targets version 1.6 of Azure AD Graph.</span></span>
- <span data-ttu-id="fcf83-134">Указывает `contoso.com` в качестве ID клиента.</span><span class="sxs-lookup"><span data-stu-id="fcf83-134">Specifies `contoso.com` as the tenant ID.</span></span> <span data-ttu-id="fcf83-135">Альтернатива показывает использование псевдонима на основе ID клиента в `myOrganization` маркере доступа.</span><span class="sxs-lookup"><span data-stu-id="fcf83-135">The alternative shows the use of an alias `myOrganization` based on the tenant ID in the access token.</span></span>
- <span data-ttu-id="fcf83-136">Вызывает ресурс пользователей.</span><span class="sxs-lookup"><span data-stu-id="fcf83-136">Calls the users resource.</span></span>
- <span data-ttu-id="fcf83-137">Параметр `$filter` запроса используется для ограничения ответа на заданные имена, которые начинаются `Dan` с .</span><span class="sxs-lookup"><span data-stu-id="fcf83-137">Uses the `$filter` query parameter to limit the response to given names that begin with `Dan`.</span></span>

<span data-ttu-id="fcf83-138">К результатам относятся пользователи с именами Daniel, Danforth, Danielle, Danerys и так далее.</span><span class="sxs-lookup"><span data-stu-id="fcf83-138">Results include users with names like Daniel, Danforth, Danielle, Danerys, and so on.</span></span>

<span data-ttu-id="fcf83-139">Аналогичный запрос для Microsoft Graph будет:</span><span class="sxs-lookup"><span data-stu-id="fcf83-139">A similar request for Microsoft Graph would be:</span></span>

`GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

<span data-ttu-id="fcf83-140">Здесь:</span><span class="sxs-lookup"><span data-stu-id="fcf83-140">Here:</span></span>

- <span data-ttu-id="fcf83-141">Версия `v1.0` .</span><span class="sxs-lookup"><span data-stu-id="fcf83-141">The version is `v1.0`.</span></span>
- <span data-ttu-id="fcf83-142">ID клиента высвечен из маркера доступа (не показан).</span><span class="sxs-lookup"><span data-stu-id="fcf83-142">The tenant ID is inferred from the access token (not shown).</span></span>
- <span data-ttu-id="fcf83-143">Параметр ресурса `$filter` и запроса такой же, как и запрос Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fcf83-143">The resource and `$filter` query parameter are the same as the Azure AD query.</span></span>

> <span data-ttu-id="fcf83-144">**ПРИМЕЧАНИЕ.** Если вы используете клиентскую библиотеку Azure AD Graph .NET, см. в заметке .NET client [libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span><span class="sxs-lookup"><span data-stu-id="fcf83-144">**NOTE**: If you're using the Azure AD Graph .NET client library, see [.NET client libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span></span>

### <a name="key-identifiers-objectid-vs-id"></a><span data-ttu-id="fcf83-145">Ключевые идентификаторы: objectId vs id</span><span class="sxs-lookup"><span data-stu-id="fcf83-145">Key identifiers: objectId vs id</span></span>

<span data-ttu-id="fcf83-146">В Azure AD Graph все типы ресурсов сущности имеют уникальный идентификатор (или ключ) под названием **objectId.**</span><span class="sxs-lookup"><span data-stu-id="fcf83-146">In Azure AD Graph, all entity resource types have a unique identifier (or key) called **objectId**.</span></span>  <span data-ttu-id="fcf83-147">По большей части (если иное не указано) этот идентификатор называется **идентификатором** в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fcf83-147">For the most part (unless otherwise stated) this same identifier is called **id** in Microsoft Graph.</span></span>

## <a name="default-properties-and-select"></a><span data-ttu-id="fcf83-148">Свойства и $select</span><span class="sxs-lookup"><span data-stu-id="fcf83-148">Default properties and $select</span></span>

<span data-ttu-id="fcf83-149">Используйте параметр `$select` запроса в запросах GET, чтобы настроить ответ, чтобы включить все необходимые свойства приложения.</span><span class="sxs-lookup"><span data-stu-id="fcf83-149">Use the `$select` query parameter, in GET requests, to customize the response to include all the properties that your app requires.</span></span>

<span data-ttu-id="fcf83-150">Операции получения  **или** списка Microsoft Graph для пользовательских или групповых ресурсов возвращают только подмножество всех свойств, известных как свойства по _умолчанию._</span><span class="sxs-lookup"><span data-stu-id="fcf83-150">Microsoft Graph **get** or **list** operations for user or group resources returns only a subset of all properties, known as the _default properties_.</span></span> <span data-ttu-id="fcf83-151">Свойства по умолчанию представляют наиболее часто используемые свойства для ресурса.</span><span class="sxs-lookup"><span data-stu-id="fcf83-151">The default properties represent the most commonly-used properties for a resource.</span></span> <span data-ttu-id="fcf83-152">С другой стороны, Azure AD Graph возвращает полный набор всех свойств для соответствующего ресурса.</span><span class="sxs-lookup"><span data-stu-id="fcf83-152">On the other hand, Azure AD Graph returns the full set of all properties for the respective resource.</span></span>

<span data-ttu-id="fcf83-153">Чтобы получить другие свойства в v1.0, приложение должно явно запрашивать их с помощью `$select` параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="fcf83-153">To get other properties in v1.0, your app needs to explicitly request them, using the `$select` query parameter.</span></span> <span data-ttu-id="fcf83-154">Это включает в себя все расширения схемы каталогов, которые может использовать ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="fcf83-154">This includes any directory schema extensions your app might be using.</span></span> <span data-ttu-id="fcf83-155">Лучше всего запрашивать только свойства, которые действительно нужны вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="fcf83-155">It's a best practice to only request the properties your app really needs.</span></span>

<span data-ttu-id="fcf83-156">Чтобы проиллюстрировать разницу, используйте Graph Explorer для запуска следующих запросов и сравнения различных ответов.</span><span class="sxs-lookup"><span data-stu-id="fcf83-156">To illustrate the difference, use Graph Explorer to run the following requests and compare the different responses.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

<span data-ttu-id="fcf83-157">Просмотрите ответы по каждому запросу.</span><span class="sxs-lookup"><span data-stu-id="fcf83-157">Review the responses from each query.</span></span> <span data-ttu-id="fcf83-158">Вы заметите, что сведения о адресе возвращаются бета-версией, но не версией /v1.0.</span><span class="sxs-lookup"><span data-stu-id="fcf83-158">You'll notice that address information is returned by the /beta version, but not the /v1.0 version.</span></span>  <span data-ttu-id="fcf83-159">Это потому, что свойства адресов не в наборе свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fcf83-159">That's because the address properties aren't in the default property set.</span></span>

<span data-ttu-id="fcf83-160">Если приложение полагается на свойства адресов, необходимо обновить запросы на v1.0, чтобы включить параметр `$select` запроса:</span><span class="sxs-lookup"><span data-stu-id="fcf83-160">If your app relies on the address properties, you need to update your v1.0 requests to include the `$select` query parameter:</span></span>

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

<span data-ttu-id="fcf83-161">Ответ на этот запрос будет включать свойства адресов.</span><span class="sxs-lookup"><span data-stu-id="fcf83-161">The response for this request would include the address properties.</span></span>  <span data-ttu-id="fcf83-162">Оно также включает **свойство displayName,** но только потому, что оно было задано параметром запроса.</span><span class="sxs-lookup"><span data-stu-id="fcf83-162">It also includes the **displayName** property, but only because it was specified by the query parameter.</span></span>

<span data-ttu-id="fcf83-163">Чтобы узнать больше о:</span><span class="sxs-lookup"><span data-stu-id="fcf83-163">To learn more about:</span></span>

- <span data-ttu-id="fcf83-164">Свойства по умолчанию для пользователя см. в [записи пользователей](/graph/api/resources/users?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="fcf83-164">Default properties on user, see [users](/graph/api/resources/users?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="fcf83-165">Параметр `$select` и другие поддерживаемые параметры запроса ODATA см. в руб. Параметры использования запросов [для настройки ответов.](./query-parameters.md)</span><span class="sxs-lookup"><span data-stu-id="fcf83-165">The `$select` parameter and other supported ODATA query parameters, see [Use query parameters to customize responses](./query-parameters.md).</span></span>
- <span data-ttu-id="fcf83-166">Эти и другие рекомендуемые оптимизации см. в [рекомендациях.](./best-practices-concept.md)</span><span class="sxs-lookup"><span data-stu-id="fcf83-166">This and other recommended optimizations, see [Best practices](./best-practices-concept.md).</span></span>

## <a name="relationships-and-navigation-properties"></a><span data-ttu-id="fcf83-167">Свойства отношений и навигации</span><span class="sxs-lookup"><span data-stu-id="fcf83-167">Relationships and navigation properties</span></span>

<span data-ttu-id="fcf83-168">Отношения (или свойства навигации) являются ключевой концепцией в Azure AD Graph и Microsoft Graph, создавая сеть связанных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fcf83-168">Relationships (or navigation properties) are a key concept in Azure AD Graph and Microsoft Graph, creating a network of related resources.</span></span> <span data-ttu-id="fcf83-169">Например, свойства **manager** и **directReports** расширяют пользовательский ресурс, чтобы обеспечить организационную иерархию.</span><span class="sxs-lookup"><span data-stu-id="fcf83-169">For example, the **manager** and **directReports** properties extend the user resource to provide organizational hierarchy.</span></span>

<span data-ttu-id="fcf83-170">Отношения также определяют членство, например группы, к которой принадлежит пользователь, члены, принадлежащие к группе или роли каталога, и так далее.</span><span class="sxs-lookup"><span data-stu-id="fcf83-170">Relationships also define memberships, such as the groups a user belongs to, the members belonging to a group or a directory role, and so on.</span></span>

<span data-ttu-id="fcf83-171">Запросы Azure AD Graph используются для `$link` указать отношения между ресурсами.</span><span class="sxs-lookup"><span data-stu-id="fcf83-171">Azure AD Graph requests use `$link` to indicate relationships between resources.</span></span>  <span data-ttu-id="fcf83-172">В Microsoft Graph вместо этого используется нотация ODATA 4.01. `$ref`</span><span class="sxs-lookup"><span data-stu-id="fcf83-172">In Microsoft Graph this uses the ODATA 4.01 `$ref` notation instead.</span></span>

<span data-ttu-id="fcf83-173">В следующей таблице показано несколько примеров:</span><span class="sxs-lookup"><span data-stu-id="fcf83-173">The following table shows several examples:</span></span>

| <span data-ttu-id="fcf83-174">Задача</span><span class="sxs-lookup"><span data-stu-id="fcf83-174">Task</span></span> | <span data-ttu-id="fcf83-175">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="fcf83-175">Azure AD Graph</span></span> | <span data-ttu-id="fcf83-176">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fcf83-176">Microsoft Graph</span></span> |
|------|----------------|-----------------|
| <span data-ttu-id="fcf83-177">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="fcf83-177">Add member</span></span>        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| <span data-ttu-id="fcf83-178">Ссылки участников списка</span><span class="sxs-lookup"><span data-stu-id="fcf83-178">List member links</span></span> | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| <span data-ttu-id="fcf83-179">Список участников</span><span class="sxs-lookup"><span data-stu-id="fcf83-179">List members</span></span>      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| <span data-ttu-id="fcf83-180">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="fcf83-180">Remove member</span></span>     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

<span data-ttu-id="fcf83-181">При переносе приложений в Microsoft Graph необходимо искать запросы, которые используются для связывания ресурсов; измените их `$link` на `$ref` использование.</span><span class="sxs-lookup"><span data-stu-id="fcf83-181">When migrating your apps to Microsoft Graph, look for requests that use `$link` to associate resources; change these to use `$ref` instead.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fcf83-182">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="fcf83-182">Next Steps</span></span>

- <span data-ttu-id="fcf83-183">Узнайте о [различиях функций](migrate-azure-ad-graph-feature-differences.md) службы между Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fcf83-183">Learn about [service feature differences](migrate-azure-ad-graph-feature-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="fcf83-184">Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.</span><span class="sxs-lookup"><span data-stu-id="fcf83-184">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>