---
title: Запрос различий между Azure AD Graph и Microsoft Graph
description: Сведения о том, как запросы Microsoft Graph отличаются от запросов Azure AD, которые помогают перенести приложения в более новую службу..
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: ae393192961c61890e7dc3963a82727b6aea0557
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289108"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="2feb6-103">Запрос различий между Azure AD Graph и Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2feb6-103">Request differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="2feb6-104">Эта статья входит в *Шаг 1: Ознакомьтесь с различиями* в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="2feb6-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="2feb6-105">Microsoft Graph и API Graph для Azure AD — это интерфейсы API REST и каждая из них поддерживает соглашения ODATA для параметров запроса.</span><span class="sxs-lookup"><span data-stu-id="2feb6-105">Microsoft Graph and the Azure AD Graph API are both REST APIs and they each support ODATA conventions for query parameters.</span></span> <span data-ttu-id="2feb6-106">Тем не менее синтаксис различается для этих двух интерфейсов API.</span><span class="sxs-lookup"><span data-stu-id="2feb6-106">However, the syntax varies between these two APIs.</span></span>

<span data-ttu-id="2feb6-107">Используйте [проводник Graph](https://aka.ms/ge) , чтобы использовать эти шаблоны запросов для собственных данных, так как это отличный способ узнать о различиях в запросах и ответах.</span><span class="sxs-lookup"><span data-stu-id="2feb6-107">Use the [Graph Explorer](https://aka.ms/ge) to try these request patterns against your own data, as it's a great way to learn about the request and response differences.</span></span>

## <a name="basic-requests"></a><span data-ttu-id="2feb6-108">Основные запросы</span><span class="sxs-lookup"><span data-stu-id="2feb6-108">Basic requests</span></span>

<span data-ttu-id="2feb6-109">В следующей таблице показаны основные различия между двумя API-интерфейсами:</span><span class="sxs-lookup"><span data-stu-id="2feb6-109">The following table highlights the main request differences between the two APIs:</span></span>

|<span data-ttu-id="2feb6-110">Сведения о запросе</span><span class="sxs-lookup"><span data-stu-id="2feb6-110">Request details</span></span>| <span data-ttu-id="2feb6-111">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="2feb6-111">Azure AD Graph</span></span> | <span data-ttu-id="2feb6-112">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2feb6-112">Microsoft Graph</span></span> |
|---|---|---|
|<span data-ttu-id="2feb6-113">Синтаксис запроса</span><span class="sxs-lookup"><span data-stu-id="2feb6-113">Request syntax</span></span>| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|<span data-ttu-id="2feb6-114">&nbsp;Конечные точки служб:</span><span class="sxs-lookup"><span data-stu-id="2feb6-114">Service&nbsp;endpoints:</span></span>||
|<span data-ttu-id="2feb6-115">-&nbsp;Глобального</span><span class="sxs-lookup"><span data-stu-id="2feb6-115">-&nbsp;Global</span></span>|`https://graph.windows.net`|`https://graph.microsoft.com`|
|<span data-ttu-id="2feb6-116">-&nbsp;&nbsp;Gov &nbsp; 4 для США</span><span class="sxs-lookup"><span data-stu-id="2feb6-116">-&nbsp;US&nbsp;Gov&nbsp;L4</span></span>|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|<span data-ttu-id="2feb6-117">-&nbsp;Американский &nbsp; gov на &nbsp; уровне 5 &nbsp; (DoD)</span><span class="sxs-lookup"><span data-stu-id="2feb6-117">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span></span>|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|<span data-ttu-id="2feb6-118">-&nbsp;Германия</span><span class="sxs-lookup"><span data-stu-id="2feb6-118">-&nbsp;Germany</span></span>|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|<span data-ttu-id="2feb6-119">-&nbsp;Китай &nbsp; (21vianet)</span><span class="sxs-lookup"><span data-stu-id="2feb6-119">-&nbsp;China&nbsp;(21Vianet)</span></span>| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|<span data-ttu-id="2feb6-120">{tenant_id}</span><span class="sxs-lookup"><span data-stu-id="2feb6-120">{tenant_id}</span></span>|<span data-ttu-id="2feb6-121">Укажите идентификатор клиента в запросе.</span><span class="sxs-lookup"><span data-stu-id="2feb6-121">Specify the ID of the tenant in the request.</span></span>|<span data-ttu-id="2feb6-122">Необязательно указывать идентификатор клиента в запросе, так как он выводится из маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="2feb6-122">It's optional to specify a tenant ID in the request as it is inferred from the access token.</span></span><br><br><span data-ttu-id="2feb6-123">Если указать идентификатор клиента, он поместится между параметром `{version}` и `{resource}` в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="2feb6-123">If you specify the tenant ID, it goes between the `{version}` and the `{resource}` in the request URL.</span></span>|
|<span data-ttu-id="2feb6-124">Отслеживание</span><span class="sxs-lookup"><span data-stu-id="2feb6-124">{version}</span></span>|<span data-ttu-id="2feb6-125">Укажите в запросе окончательную версию Azure AD Graph, используя обязательный параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="2feb6-125">Specify the release version of Azure AD Graph in the request using a required query parameter.</span></span>|<span data-ttu-id="2feb6-126">Укажите версию Microsoft Graph в запросе в качестве части URL-пути сразу после конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="2feb6-126">Specify the release version of Microsoft Graph in the request as part of the URL path just after the service endpoint.</span></span>|

<span data-ttu-id="2feb6-127">Вы можете продолжать использовать одни и те же параметры запроса в Microsoft Graph как Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="2feb6-127">You can continue to use the same query parameters in Microsoft Graph as Azure AD Graph.</span></span>

### <a name="example-request-comparison"></a><span data-ttu-id="2feb6-128">Пример сравнения запросов</span><span class="sxs-lookup"><span data-stu-id="2feb6-128">Example request comparison</span></span>

<span data-ttu-id="2feb6-129">Предположим, что вам нужен список всех пользователей с именами, начинающимися с "" "").</span><span class="sxs-lookup"><span data-stu-id="2feb6-129">Suppose you want a list of all users with names beginning with "Dan".</span></span>

<span data-ttu-id="2feb6-130">В Azure AD Graph можно использовать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="2feb6-130">In Azure AD Graph, you might use this request:</span></span>

<span data-ttu-id="2feb6-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` также</span><span class="sxs-lookup"><span data-stu-id="2feb6-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` or</span></span>

`GET https://graph.windows.net/myOrganization/users?$filter=startswith(givenName,'Dan')&api-version=1.6`


<span data-ttu-id="2feb6-132">Этот запрос:</span><span class="sxs-lookup"><span data-stu-id="2feb6-132">This request:</span></span>

- <span data-ttu-id="2feb6-133">Targets версии 1,6 для Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="2feb6-133">Targets version 1.6 of Azure AD Graph.</span></span>
- <span data-ttu-id="2feb6-134">Задает `contoso.com` идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="2feb6-134">Specifies `contoso.com` as the tenant ID.</span></span> <span data-ttu-id="2feb6-135">В альтернативу показано использование псевдонима на `myOrganization` основе идентификатора клиента в маркере доступа.</span><span class="sxs-lookup"><span data-stu-id="2feb6-135">The alternative shows the use of an alias `myOrganization` based on the tenant ID in the access token.</span></span>
- <span data-ttu-id="2feb6-136">Вызывает ресурс Users.</span><span class="sxs-lookup"><span data-stu-id="2feb6-136">Calls the users resource.</span></span>
- <span data-ttu-id="2feb6-137">Использует `$filter` параметр запроса, чтобы ограничить ответ на заданные имена, начинающиеся с `Dan` .</span><span class="sxs-lookup"><span data-stu-id="2feb6-137">Uses the `$filter` query parameter to limit the response to given names that begin with `Dan`.</span></span>

<span data-ttu-id="2feb6-138">Результаты включают пользователей с именами, такими как Дэниэл, Данфорс, Даниелле, Данерис и т. д.</span><span class="sxs-lookup"><span data-stu-id="2feb6-138">Results include users with names like Daniel, Danforth, Danielle, Danerys, and so on.</span></span>

<span data-ttu-id="2feb6-139">Аналогичный запрос для Microsoft Graph выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="2feb6-139">A similar request for Microsoft Graph would be:</span></span>

`GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

<span data-ttu-id="2feb6-140">Существует</span><span class="sxs-lookup"><span data-stu-id="2feb6-140">Here:</span></span>

- <span data-ttu-id="2feb6-141">Версия `v1.0` .</span><span class="sxs-lookup"><span data-stu-id="2feb6-141">The version is `v1.0`.</span></span>
- <span data-ttu-id="2feb6-142">Идентификатор клиента извлекается из маркера доступа (не показан).</span><span class="sxs-lookup"><span data-stu-id="2feb6-142">The tenant ID is inferred from the access token (not shown).</span></span>
- <span data-ttu-id="2feb6-143">Параметр resource и `$filter` Query совпадает с запросом Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2feb6-143">The resource and `$filter` query parameter are the same as the Azure AD query.</span></span>

> <span data-ttu-id="2feb6-144">**Примечание**. Если вы используете клиентскую библиотеку .NET для Azure AD Graph, ознакомьтесь с разработкой клиентских [библиотек .NET](migrate-azure-ad-graph-client-libraries.md) для получения более подробных стратегий и помощи в переходе на клиентскую библиотеку Microsoft Graph .NET.</span><span class="sxs-lookup"><span data-stu-id="2feb6-144">**NOTE**: If you're using the Azure AD Graph .NET client library, see [.NET client libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span></span>

### <a name="key-identifiers-objectid-vs-id"></a><span data-ttu-id="2feb6-145">Идентификаторы ключа: objectId VS ID</span><span class="sxs-lookup"><span data-stu-id="2feb6-145">Key identifiers: objectId vs id</span></span>

<span data-ttu-id="2feb6-146">В Azure AD Graph все типы ресурсов сущностей имеют уникальный идентификатор (или ключ) с именем **ObjectID**.</span><span class="sxs-lookup"><span data-stu-id="2feb6-146">In Azure AD Graph, all entity resource types have a unique identifier (or key) called **objectId**.</span></span>  <span data-ttu-id="2feb6-147">Для большинства частей (если не указано иное) такой же идентификатор называется **идентификатором** в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2feb6-147">For the most part (unless otherwise stated) this same identifier is called **id** in Microsoft Graph.</span></span>

## <a name="default-properties-and-select"></a><span data-ttu-id="2feb6-148">Свойства по умолчанию и $select</span><span class="sxs-lookup"><span data-stu-id="2feb6-148">Default properties and $select</span></span>

<span data-ttu-id="2feb6-149">Используйте `$select` параметр запроса в запросах GET, чтобы настроить ответ на включение всех свойств, необходимых вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="2feb6-149">Use the `$select` query parameter, in GET requests, to customize the response to include all the properties that your app requires.</span></span>

<span data-ttu-id="2feb6-150">Операции **получения** или получения **списка** Microsoft Graph для ресурсов пользователей или групп возвращают только подмножество свойств, известных как _свойства по умолчанию_.</span><span class="sxs-lookup"><span data-stu-id="2feb6-150">Microsoft Graph **get** or **list** operations for user or group resources returns only a subset of all properties, known as the _default properties_.</span></span> <span data-ttu-id="2feb6-151">Свойства по умолчанию представляют наиболее часто используемые свойства ресурса.</span><span class="sxs-lookup"><span data-stu-id="2feb6-151">The default properties represent the most commonly-used properties for a resource.</span></span> <span data-ttu-id="2feb6-152">С другой стороны, Azure AD Graph возвращает полный набор всех свойств для соответствующего ресурса.</span><span class="sxs-lookup"><span data-stu-id="2feb6-152">On the other hand, Azure AD Graph returns the full set of all properties for the respective resource.</span></span>

<span data-ttu-id="2feb6-153">Чтобы получить другие свойства в версии 1.0, ваше приложение должно явно запрашивать их, используя `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="2feb6-153">To get other properties in v1.0, your app needs to explicitly request them, using the `$select` query parameter.</span></span> <span data-ttu-id="2feb6-154">Сюда входят все расширения схемы каталогов, которые может использовать ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="2feb6-154">This includes any directory schema extensions your app might be using.</span></span> <span data-ttu-id="2feb6-155">Рекомендуется запрашивать только те свойства, которые действительно необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="2feb6-155">It's a best practice to only request the properties your app really needs.</span></span>

<span data-ttu-id="2feb6-156">Чтобы продемонстрировать разницу, используйте проводник Graph для выполнения следующих запросов и сравнения различных ответов.</span><span class="sxs-lookup"><span data-stu-id="2feb6-156">To illustrate the difference, use Graph Explorer to run the following requests and compare the different responses.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

<span data-ttu-id="2feb6-157">Просмотрите ответы от каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="2feb6-157">Review the responses from each query.</span></span> <span data-ttu-id="2feb6-158">Вы заметите, что сведения об адресе возвращаются версией/Beta, но не версией/v1.0.</span><span class="sxs-lookup"><span data-stu-id="2feb6-158">You'll notice that address information is returned by the /beta version, but not the /v1.0 version.</span></span>  <span data-ttu-id="2feb6-159">Это вызвано тем, что свойства адреса не входят в набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2feb6-159">That's because the address properties aren't in the default property set.</span></span>

<span data-ttu-id="2feb6-160">Если ваше приложение использует свойства адреса, необходимо обновить запросы версии 1.0, чтобы включить `$select` параметр запроса:</span><span class="sxs-lookup"><span data-stu-id="2feb6-160">If your app relies on the address properties, you need to update your v1.0 requests to include the `$select` query parameter:</span></span>

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

<span data-ttu-id="2feb6-161">Ответ на этот запрос будет включать в себя свойства Address.</span><span class="sxs-lookup"><span data-stu-id="2feb6-161">The response for this request would include the address properties.</span></span>  <span data-ttu-id="2feb6-162">Он также включает свойство **DisplayName** , но только потому, что оно было задано с помощью параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="2feb6-162">It also includes the **displayName** property, but only because it was specified by the query parameter.</span></span>

<span data-ttu-id="2feb6-163">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="2feb6-163">To learn more about:</span></span>

- <span data-ttu-id="2feb6-164">Свойства по умолчанию для пользователя, обратитесь к разделу [Пользователи](/graph/api/resources/users?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="2feb6-164">Default properties on user, see [users](/graph/api/resources/users?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="2feb6-165">`$select`Параметр и другие поддерживаемые параметры запроса ODATA в разделе [Использование параметров запроса для настройки ответов](./query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="2feb6-165">The `$select` parameter and other supported ODATA query parameters, see [Use query parameters to customize responses](./query-parameters.md).</span></span>
- <span data-ttu-id="2feb6-166">Эта и другие Рекомендуемые [оптимизации приведены в разделе рекомендации.](./best-practices-concept.md)</span><span class="sxs-lookup"><span data-stu-id="2feb6-166">This and other recommended optimizations, see [Best practices](./best-practices-concept.md).</span></span>

## <a name="relationships-and-navigation-properties"></a><span data-ttu-id="2feb6-167">Отношения и свойства навигации</span><span class="sxs-lookup"><span data-stu-id="2feb6-167">Relationships and navigation properties</span></span>

<span data-ttu-id="2feb6-168">Отношения (или свойства навигации) являются ключевыми понятиями в Azure AD Graph и Microsoft Graph, создавая сеть связанных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2feb6-168">Relationships (or navigation properties) are a key concept in Azure AD Graph and Microsoft Graph, creating a network of related resources.</span></span> <span data-ttu-id="2feb6-169">Например, свойства **Manager** и **directReports** расширяют пользовательский ресурс для предоставления организационной иерархии.</span><span class="sxs-lookup"><span data-stu-id="2feb6-169">For example, the **manager** and **directReports** properties extend the user resource to provide organizational hierarchy.</span></span>

<span data-ttu-id="2feb6-170">Отношения также определяют членство, например группы, к которым принадлежит пользователь, членов, принадлежащих группе или роли каталога, и т. д.</span><span class="sxs-lookup"><span data-stu-id="2feb6-170">Relationships also define memberships, such as the groups a user belongs to, the members belonging to a group or a directory role, and so on.</span></span>

<span data-ttu-id="2feb6-171">Запросы Azure AD Graph используются `$link` для обозначения отношений между ресурсами.</span><span class="sxs-lookup"><span data-stu-id="2feb6-171">Azure AD Graph requests use `$link` to indicate relationships between resources.</span></span>  <span data-ttu-id="2feb6-172">В Microsoft Graph `$ref` вместо этого используется нотация ODATA 4,01.</span><span class="sxs-lookup"><span data-stu-id="2feb6-172">In Microsoft Graph this uses the ODATA 4.01 `$ref` notation instead.</span></span>

<span data-ttu-id="2feb6-173">В следующей таблице приведено несколько примеров.</span><span class="sxs-lookup"><span data-stu-id="2feb6-173">The following table shows several examples:</span></span>

| <span data-ttu-id="2feb6-174">Задача</span><span class="sxs-lookup"><span data-stu-id="2feb6-174">Task</span></span> | <span data-ttu-id="2feb6-175">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="2feb6-175">Azure AD Graph</span></span> | <span data-ttu-id="2feb6-176">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2feb6-176">Microsoft Graph</span></span> |
|------|----------------|-----------------|
| <span data-ttu-id="2feb6-177">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="2feb6-177">Add member</span></span>        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| <span data-ttu-id="2feb6-178">Ссылки на элементы списка</span><span class="sxs-lookup"><span data-stu-id="2feb6-178">List member links</span></span> | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| <span data-ttu-id="2feb6-179">Список участников</span><span class="sxs-lookup"><span data-stu-id="2feb6-179">List members</span></span>      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| <span data-ttu-id="2feb6-180">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="2feb6-180">Remove member</span></span>     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

<span data-ttu-id="2feb6-181">При переносе приложений в Microsoft Graph ищите запросы, которые используют `$link` для связи ресурсов, а вместо этого измените их для использования `$ref` .</span><span class="sxs-lookup"><span data-stu-id="2feb6-181">When migrating your apps to Microsoft Graph, look for requests that use `$link` to associate resources; change these to use `$ref` instead.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2feb6-182">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="2feb6-182">Next Steps</span></span>

- <span data-ttu-id="2feb6-183">Сведения о [различиях функций служб](migrate-azure-ad-graph-feature-differences.md) в Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2feb6-183">Learn about [service feature differences](migrate-azure-ad-graph-feature-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="2feb6-184">Снова просмотрите [Контрольный список](migrate-azure-ad-graph-planning-checklist.md) .</span><span class="sxs-lookup"><span data-stu-id="2feb6-184">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>