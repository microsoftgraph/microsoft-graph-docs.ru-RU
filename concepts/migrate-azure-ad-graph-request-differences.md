---
title: Запрос различий между Azure AD Graph и Microsoft Graph
description: Сведения о том, как запросы Microsoft Graph отличаются от запросов Azure AD, которые помогают перенести приложения в более новую службу..
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8130daf4037e6ef1a433ca537a8fecec996a34ce
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845920"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="23dda-103">Запрос различий между Azure AD Graph и Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="23dda-103">Request differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="23dda-104">Эта статья входит в *Шаг 1: Ознакомьтесь с различиями* в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="23dda-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="23dda-105">Microsoft Graph и API Graph для Azure AD — это интерфейсы API REST и каждая из них поддерживает соглашения ODATA для параметров запроса.</span><span class="sxs-lookup"><span data-stu-id="23dda-105">Microsoft Graph and the Azure AD Graph API are both REST APIs and they each support ODATA conventions for query parameters.</span></span> <span data-ttu-id="23dda-106">Тем не менее синтаксис различается для этих двух интерфейсов API.</span><span class="sxs-lookup"><span data-stu-id="23dda-106">However, the syntax varies between these two APIs.</span></span>

<span data-ttu-id="23dda-107">Используйте [проводник Graph](https://aka.ms/ge) , чтобы использовать эти шаблоны запросов для собственных данных, так как это отличный способ узнать о различиях в запросах и ответах.</span><span class="sxs-lookup"><span data-stu-id="23dda-107">Use the [Graph Explorer](https://aka.ms/ge) to try these request patterns against your own data, as it's a great way to learn about the request and response differences.</span></span>

## <a name="basic-requests"></a><span data-ttu-id="23dda-108">Основные запросы</span><span class="sxs-lookup"><span data-stu-id="23dda-108">Basic requests</span></span>

<span data-ttu-id="23dda-109">В следующей таблице показаны основные различия между двумя API-интерфейсами:</span><span class="sxs-lookup"><span data-stu-id="23dda-109">The following table highlights the main request differences between the two APIs:</span></span>

|<span data-ttu-id="23dda-110">Сведения о запросе</span><span class="sxs-lookup"><span data-stu-id="23dda-110">Request details</span></span>| <span data-ttu-id="23dda-111">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="23dda-111">Azure AD Graph</span></span> | <span data-ttu-id="23dda-112">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="23dda-112">Microsoft Graph</span></span> |
|---|---|---|
|<span data-ttu-id="23dda-113">Синтаксис запроса</span><span class="sxs-lookup"><span data-stu-id="23dda-113">Request syntax</span></span>| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|<span data-ttu-id="23dda-114">&nbsp;Конечные точки служб:</span><span class="sxs-lookup"><span data-stu-id="23dda-114">Service&nbsp;endpoints:</span></span>||
|<span data-ttu-id="23dda-115">-&nbsp;Глобального</span><span class="sxs-lookup"><span data-stu-id="23dda-115">-&nbsp;Global</span></span>|`https://graph.windows.net`|`https://graph.microsoft.com`|
|<span data-ttu-id="23dda-116">-&nbsp;&nbsp;Gov &nbsp; 4 для США</span><span class="sxs-lookup"><span data-stu-id="23dda-116">-&nbsp;US&nbsp;Gov&nbsp;L4</span></span>|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|<span data-ttu-id="23dda-117">-&nbsp;Американский &nbsp; gov на &nbsp; уровне 5 &nbsp; (DoD)</span><span class="sxs-lookup"><span data-stu-id="23dda-117">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span></span>|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|<span data-ttu-id="23dda-118">-&nbsp;Германия</span><span class="sxs-lookup"><span data-stu-id="23dda-118">-&nbsp;Germany</span></span>|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|<span data-ttu-id="23dda-119">-&nbsp;Китай &nbsp; (21vianet)</span><span class="sxs-lookup"><span data-stu-id="23dda-119">-&nbsp;China&nbsp;(21Vianet)</span></span>| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|<span data-ttu-id="23dda-120">{tenant_id}</span><span class="sxs-lookup"><span data-stu-id="23dda-120">{tenant_id}</span></span>|<span data-ttu-id="23dda-121">Укажите идентификатор клиента в запросе.</span><span class="sxs-lookup"><span data-stu-id="23dda-121">Specify the ID of the tenant in the request.</span></span>|<span data-ttu-id="23dda-122">Необязательно указывать идентификатор клиента в запросе, так как он выводится из маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="23dda-122">It's optional to specify a tenant ID in the request as it is inferred from the access token.</span></span><br><br><span data-ttu-id="23dda-123">Если указать идентификатор клиента, он поместится между параметром `{version}` и `{resource}` в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="23dda-123">If you specify the tenant ID, it goes between the `{version}` and the `{resource}` in the request URL.</span></span>|
|<span data-ttu-id="23dda-124">Отслеживание</span><span class="sxs-lookup"><span data-stu-id="23dda-124">{version}</span></span>|<span data-ttu-id="23dda-125">Укажите в запросе окончательную версию Azure AD Graph, используя обязательный параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="23dda-125">Specify the release version of Azure AD Graph in the request using a required query parameter.</span></span>|<span data-ttu-id="23dda-126">Укажите версию Microsoft Graph в запросе в качестве части URL-пути сразу после конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="23dda-126">Specify the release version of Microsoft Graph in the request as part of the URL path just after the service endpoint.</span></span>|

<span data-ttu-id="23dda-127">Вы можете продолжать использовать одни и те же параметры запроса в Microsoft Graph как Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="23dda-127">You can continue to use the same query parameters in Microsoft Graph as Azure AD Graph.</span></span>

### <a name="example-request-comparison"></a><span data-ttu-id="23dda-128">Пример сравнения запросов</span><span class="sxs-lookup"><span data-stu-id="23dda-128">Example request comparison</span></span>

<span data-ttu-id="23dda-129">Предположим, что вам нужен список всех пользователей с именами, начинающимися с "" "").</span><span class="sxs-lookup"><span data-stu-id="23dda-129">Suppose you want a list of all users with names beginning with "Dan".</span></span>

<span data-ttu-id="23dda-130">В Azure AD Graph можно использовать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="23dda-130">In Azure AD Graph, you might use this request:</span></span>

`https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6`

<span data-ttu-id="23dda-131">Этот запрос:</span><span class="sxs-lookup"><span data-stu-id="23dda-131">This request:</span></span>

- <span data-ttu-id="23dda-132">Targets версии 1,6 для Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="23dda-132">Targets version 1.6 of Azure AD Graph.</span></span>
- <span data-ttu-id="23dda-133">Задает `contoso.com` идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="23dda-133">Specifies `contoso.com` as the tenant ID.</span></span>
- <span data-ttu-id="23dda-134">Вызывает ресурс Users.</span><span class="sxs-lookup"><span data-stu-id="23dda-134">Calls the users resource.</span></span>
- <span data-ttu-id="23dda-135">Использует `$filter` параметр запроса, чтобы ограничить ответ на заданные имена, начинающиеся с `Dan` .</span><span class="sxs-lookup"><span data-stu-id="23dda-135">Uses the `$filter` query parameter to limit the response to given names that begin with `Dan`.</span></span>

<span data-ttu-id="23dda-136">Результаты включают пользователей с именами, такими как Дэниэл, Данфорс, Даниелле, Данерис и т. д.</span><span class="sxs-lookup"><span data-stu-id="23dda-136">Results include users with names like Daniel, Danforth, Danielle, Danerys, and so on.</span></span>

<span data-ttu-id="23dda-137">Аналогичный запрос для Microsoft Graph выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="23dda-137">A similar request for Microsoft Graph would be:</span></span>

`https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

<span data-ttu-id="23dda-138">Существует</span><span class="sxs-lookup"><span data-stu-id="23dda-138">Here:</span></span>

- <span data-ttu-id="23dda-139">Версия `v1.0` .</span><span class="sxs-lookup"><span data-stu-id="23dda-139">The version is `v1.0`.</span></span>
- <span data-ttu-id="23dda-140">Идентификатор клиента извлекается из маркера доступа (не показан).</span><span class="sxs-lookup"><span data-stu-id="23dda-140">The tenant ID is inferred from the access token (not shown).</span></span>
- <span data-ttu-id="23dda-141">Параметр resource и `$filter` Query совпадает с запросом Azure AD.</span><span class="sxs-lookup"><span data-stu-id="23dda-141">The resource and `$filter` query parameter are the same as the Azure AD query.</span></span>

> <span data-ttu-id="23dda-142">**Примечание**. Если вы используете клиентскую библиотеку .NET для Azure AD Graph, ознакомьтесь с разработкой клиентских [библиотек .NET](migrate-azure-ad-graph-client-libraries.md) для получения более подробных стратегий и помощи в переходе на клиентскую библиотеку Microsoft Graph .NET.</span><span class="sxs-lookup"><span data-stu-id="23dda-142">**NOTE**: If you're using the Azure AD Graph .NET client library, see [.NET client libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span></span>

### <a name="key-identifiers-objectid-vs-id"></a><span data-ttu-id="23dda-143">Идентификаторы ключа: objectId VS ID</span><span class="sxs-lookup"><span data-stu-id="23dda-143">Key identifiers: objectId vs id</span></span>

<span data-ttu-id="23dda-144">В Azure AD Graph все типы ресурсов сущностей имеют уникальный идентификатор (или ключ) с именем **ObjectID**.</span><span class="sxs-lookup"><span data-stu-id="23dda-144">In Azure AD Graph, all entity resource types have a unique identifier (or key) called **objectId**.</span></span>  <span data-ttu-id="23dda-145">Для большинства частей (если не указано иное) такой же идентификатор называется **идентификатором** в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="23dda-145">For the most part (unless otherwise stated) this same identifier is called **id** in Microsoft Graph.</span></span>

## <a name="default-properties-and-select"></a><span data-ttu-id="23dda-146">Свойства по умолчанию и $select</span><span class="sxs-lookup"><span data-stu-id="23dda-146">Default properties and $select</span></span>

<span data-ttu-id="23dda-147">Используйте `$select` параметр запроса в запросах GET, чтобы настроить ответ на включение всех свойств, необходимых вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="23dda-147">Use the `$select` query parameter, in GET requests, to customize the response to include all the properties that your app requires.</span></span>

<span data-ttu-id="23dda-148">Операции **получения** или получения **списка** Microsoft Graph для ресурсов пользователей или групп возвращают только подмножество свойств, известных как _свойства по умолчанию_.</span><span class="sxs-lookup"><span data-stu-id="23dda-148">Microsoft Graph **get** or **list** operations for user or group resources returns only a subset of all properties, known as the _default properties_.</span></span> <span data-ttu-id="23dda-149">Свойства по умолчанию представляют наиболее часто используемые свойства ресурса.</span><span class="sxs-lookup"><span data-stu-id="23dda-149">The default properties represent the most commonly-used properties for a resource.</span></span> <span data-ttu-id="23dda-150">С другой стороны, Azure AD Graph возвращает полный набор всех свойств для соответствующего ресурса.</span><span class="sxs-lookup"><span data-stu-id="23dda-150">On the other hand, Azure AD Graph returns the full set of all properties for the respective resource.</span></span>

<span data-ttu-id="23dda-151">Чтобы получить другие свойства в версии 1.0, ваше приложение должно явно запрашивать их, используя `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="23dda-151">To get other properties in v1.0, your app needs to explicitly request them, using the `$select` query parameter.</span></span> <span data-ttu-id="23dda-152">Сюда входят все расширения схемы каталогов, которые может использовать ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="23dda-152">This includes any directory schema extensions your app might be using.</span></span> <span data-ttu-id="23dda-153">Рекомендуется запрашивать только те свойства, которые действительно необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="23dda-153">It's a best practice to only request the properties your app really needs.</span></span>

<span data-ttu-id="23dda-154">Чтобы продемонстрировать разницу, используйте проводник Graph для выполнения следующих запросов и сравнения различных ответов.</span><span class="sxs-lookup"><span data-stu-id="23dda-154">To illustrate the difference, use Graph Explorer to run the following requests and compare the different responses.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

<span data-ttu-id="23dda-155">Просмотрите ответы от каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="23dda-155">Review the responses from each query.</span></span> <span data-ttu-id="23dda-156">Вы заметите, что сведения об адресе возвращаются версией/Beta, но не версией/v1.0.</span><span class="sxs-lookup"><span data-stu-id="23dda-156">You'll notice that address information is returned by the /beta version, but not the /v1.0 version.</span></span>  <span data-ttu-id="23dda-157">Это вызвано тем, что свойства адреса не входят в набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="23dda-157">That's because the address properties aren't in the default property set.</span></span>

<span data-ttu-id="23dda-158">Если ваше приложение использует свойства адреса, необходимо обновить запросы версии 1.0, чтобы включить `$select` параметр запроса:</span><span class="sxs-lookup"><span data-stu-id="23dda-158">If your app relies on the address properties, you need to update your v1.0 requests to include the `$select` query parameter:</span></span>

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

<span data-ttu-id="23dda-159">Ответ на этот запрос будет включать в себя свойства Address.</span><span class="sxs-lookup"><span data-stu-id="23dda-159">The response for this request would include the address properties.</span></span>  <span data-ttu-id="23dda-160">Он также включает свойство **DisplayName** , но только потому, что оно было задано с помощью параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="23dda-160">It also includes the **displayName** property, but only because it was specified by the query parameter.</span></span>

<span data-ttu-id="23dda-161">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="23dda-161">To learn more about:</span></span>

- <span data-ttu-id="23dda-162">Свойства по умолчанию для пользователя, обратитесь к разделу [Пользователи](/graph/api/resources/users?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="23dda-162">Default properties on user, see [users](/graph/api/resources/users?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="23dda-163">`$select`Параметр и другие поддерживаемые параметры запроса ODATA в разделе [Использование параметров запроса для настройки ответов](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="23dda-163">The `$select` parameter and other supported ODATA query parameters, see [Use query parameters to customize responses](/graph/query-parameters).</span></span>
- <span data-ttu-id="23dda-164">Эта и другие Рекомендуемые [оптимизации приведены в разделе рекомендации.](/graph/best-practices-concept)</span><span class="sxs-lookup"><span data-stu-id="23dda-164">This and other recommended optimizations, see [Best practices](/graph/best-practices-concept).</span></span>

## <a name="relationships-and-navigation-properties"></a><span data-ttu-id="23dda-165">Отношения и свойства навигации</span><span class="sxs-lookup"><span data-stu-id="23dda-165">Relationships and navigation properties</span></span>

<span data-ttu-id="23dda-166">Отношения (или свойства навигации) являются ключевыми понятиями в Azure AD Graph и Microsoft Graph, создавая сеть связанных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="23dda-166">Relationships (or navigation properties) are a key concept in Azure AD Graph and Microsoft Graph, creating a network of related resources.</span></span> <span data-ttu-id="23dda-167">Например, свойства **Manager** и **directReports** расширяют пользовательский ресурс для предоставления организационной иерархии.</span><span class="sxs-lookup"><span data-stu-id="23dda-167">For example, the **manager** and **directReports** properties extend the user resource to provide organizational hierarchy.</span></span>

<span data-ttu-id="23dda-168">Отношения также определяют членство, например группы, к которым принадлежит пользователь, членов, принадлежащих группе или роли каталога, и т. д.</span><span class="sxs-lookup"><span data-stu-id="23dda-168">Relationships also define memberships, such as the groups a user belongs to, the members belonging to a group or a directory role, and so on.</span></span>

<span data-ttu-id="23dda-169">Запросы Azure AD Graph используются `$link` для обозначения отношений между ресурсами.</span><span class="sxs-lookup"><span data-stu-id="23dda-169">Azure AD Graph requests use `$link` to indicate relationships between resources.</span></span>  <span data-ttu-id="23dda-170">В Microsoft Graph `$ref` вместо этого используется нотация ODATA 4,01.</span><span class="sxs-lookup"><span data-stu-id="23dda-170">In Microsoft Graph this uses the ODATA 4.01 `$ref` notation instead.</span></span>

<span data-ttu-id="23dda-171">В следующей таблице приведено несколько примеров.</span><span class="sxs-lookup"><span data-stu-id="23dda-171">The following table shows several examples:</span></span>

| <span data-ttu-id="23dda-172">Task</span><span class="sxs-lookup"><span data-stu-id="23dda-172">Task</span></span> | <span data-ttu-id="23dda-173">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="23dda-173">Azure AD Graph</span></span> | <span data-ttu-id="23dda-174">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="23dda-174">Microsoft Graph</span></span> |
|------|----------------|-----------------|
| <span data-ttu-id="23dda-175">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="23dda-175">Add member</span></span>        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| <span data-ttu-id="23dda-176">Ссылки на элементы списка</span><span class="sxs-lookup"><span data-stu-id="23dda-176">List member links</span></span> | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| <span data-ttu-id="23dda-177">Список участников</span><span class="sxs-lookup"><span data-stu-id="23dda-177">List members</span></span>      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| <span data-ttu-id="23dda-178">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="23dda-178">Remove member</span></span>     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

<span data-ttu-id="23dda-179">При переносе приложений в Microsoft Graph ищите запросы, которые используют `$link` для связи ресурсов, а вместо этого измените их для использования `$ref` .</span><span class="sxs-lookup"><span data-stu-id="23dda-179">When migrating your apps to Microsoft Graph, look for requests that use `$link` to associate resources; change these to use `$ref` instead.</span></span>

## <a name="next-steps"></a><span data-ttu-id="23dda-180">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="23dda-180">Next Steps</span></span>

- <span data-ttu-id="23dda-181">Сведения о [различиях функций служб](migrate-azure-ad-graph-feature-differences.md) в Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="23dda-181">Learn about [service feature differences](migrate-azure-ad-graph-feature-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="23dda-182">Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="23dda-182">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="23dda-183">Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .</span><span class="sxs-lookup"><span data-stu-id="23dda-183">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
