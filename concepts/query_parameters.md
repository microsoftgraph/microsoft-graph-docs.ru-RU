# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="f7c95-101">Настройка ответов с помощью параметров запроса</span><span class="sxs-lookup"><span data-stu-id="f7c95-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="f7c95-p101">В Microsoft Graph предусмотрены необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных. Поддерживаются указанные ниже параметры запросов.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following query parameters are supported.</span></span>

><span data-ttu-id="f7c95-104">**Примечание.** Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="f7c95-104">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

|<span data-ttu-id="f7c95-105">Имя</span><span class="sxs-lookup"><span data-stu-id="f7c95-105">Name</span></span>|<span data-ttu-id="f7c95-106">Описание</span><span class="sxs-lookup"><span data-stu-id="f7c95-106">Description</span></span>|<span data-ttu-id="f7c95-107">Пример</span><span class="sxs-lookup"><span data-stu-id="f7c95-107">Example</span></span>|
|:---------------|:--------|:-------|
|[<span data-ttu-id="f7c95-108">$count</span><span class="sxs-lookup"><span data-stu-id="f7c95-108">$count</span></span>](#count)|<span data-ttu-id="f7c95-109">Возвращает общее количество соответствующих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f7c95-109">Retrieves the total count of matching resources.</span></span>|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
|[<span data-ttu-id="f7c95-110">$expand</span><span class="sxs-lookup"><span data-stu-id="f7c95-110">$expand</span></span>](#expand)|<span data-ttu-id="f7c95-111">Получает связанные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="f7c95-111">Retrieves related resources.</span></span>|[`/groups?$expand=members`](https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0)
|[<span data-ttu-id="f7c95-112">$filter</span><span class="sxs-lookup"><span data-stu-id="f7c95-112">$filter</span></span>](#filter)|<span data-ttu-id="f7c95-113">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="f7c95-113">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[<span data-ttu-id="f7c95-114">$orderby</span><span class="sxs-lookup"><span data-stu-id="f7c95-114">$orderby</span></span>](#orderby)|<span data-ttu-id="f7c95-115">Упорядочивает результаты.</span><span class="sxs-lookup"><span data-stu-id="f7c95-115">Orders results.</span></span>|[`/users?$orderby=displayName desc`](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0)
|[<span data-ttu-id="f7c95-116">$search</span><span class="sxs-lookup"><span data-stu-id="f7c95-116">$search</span></span>](#search)| <span data-ttu-id="f7c95-p102">Возвращает результаты на основании условий поиска. В настоящее время поддерживается в коллекциях `messages` и `person`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p102">Returns results based on search criteria. Currently supported on `messages` and `person` collections.</span></span>|[`/me/messages?$search=pizza`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0)
|[<span data-ttu-id="f7c95-119">$select</span><span class="sxs-lookup"><span data-stu-id="f7c95-119">$select</span></span>](#select)|<span data-ttu-id="f7c95-120">Фильтрует свойства (столбцы).</span><span class="sxs-lookup"><span data-stu-id="f7c95-120">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`](https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[<span data-ttu-id="f7c95-121">$skip</span><span class="sxs-lookup"><span data-stu-id="f7c95-121">$skip</span></span>](#skip)|<span data-ttu-id="f7c95-p103">Применяется для индексации в результирующем наборе. Также используется некоторыми API для разбиения по страницам и может использоваться вместе с параметром `$top` для разбиения результатов по страницам вручную.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span>  | [`/me/messages?$skip=11`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0)
|[<span data-ttu-id="f7c95-124">$skipToken</span><span class="sxs-lookup"><span data-stu-id="f7c95-124">$skipToken</span></span>](#skiptoken)|<span data-ttu-id="f7c95-p104">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц. (Вместо этого параметра некоторые API используют `$skip`.)</span><span class="sxs-lookup"><span data-stu-id="f7c95-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `https://graph.microsoft.com/v1.0/users?$skiptoken=X%274453707402000100000017 ... 65612D643839392D343230372D613033662D306332623836633432363932B900000000000000000000%27`
|[<span data-ttu-id="f7c95-127">$top</span><span class="sxs-lookup"><span data-stu-id="f7c95-127">$top</span></span>](#top)|<span data-ttu-id="f7c95-128">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="f7c95-128">Sets the page size of results.</span></span> |[`/users?$top=2`](https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)

<span data-ttu-id="f7c95-129">Эти параметры совместимы с [языком запросов OData версии 4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="f7c95-129">These parameters are compatible with the [OData V4 query language][odata-query].</span></span> <span data-ttu-id="f7c95-130">Параметры, которые поддерживаются всеми API Microsoft Graph для конечной точки `v1.0`, могут значительно отличаться от таковых для конечной точки `beta`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-130">These parameters are compatible with the OData V4 query language. Not all parameters are supported across all Microsoft Graph APIs and support may differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="f7c95-p106">**Примечание.** В конечной точке `beta` префикс `$` является необязательным. Например, вместо `$filter` можно использовать `filter`. Дополнительные сведения и примеры см. в статье [Поддержка параметров запросов без префиксов $ в Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span><span class="sxs-lookup"><span data-stu-id="f7c95-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

## <a name="encoding-query-parameters"></a><span data-ttu-id="f7c95-134">Кодирование параметров запроса</span><span class="sxs-lookup"><span data-stu-id="f7c95-134">Encoding query parameters</span></span>

<span data-ttu-id="f7c95-135">К значениям параметров запросов нужно применить процентное кодирование.</span><span class="sxs-lookup"><span data-stu-id="f7c95-135">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="f7c95-136">Многие клиенты HTTP, браузеры и инструменты (например, [песочница Graph][graph-explorer]) помогут вам в этом.</span><span class="sxs-lookup"><span data-stu-id="f7c95-136">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="f7c95-137">Если запрос неудачный, одна из возможных причин — не удалось должным образом закодировать значения параметров запросов.</span><span class="sxs-lookup"><span data-stu-id="f7c95-137">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="f7c95-138">URL-адрес, который не было закодирован, выглядит так:</span><span class="sxs-lookup"><span data-stu-id="f7c95-138">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="f7c95-139">Закодированный должным образом URL-адрес выглядит так:</span><span class="sxs-lookup"><span data-stu-id="f7c95-139">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count"></a><span data-ttu-id="f7c95-140">count</span><span class="sxs-lookup"><span data-stu-id="f7c95-140">count</span></span>

<span data-ttu-id="f7c95-141">Параметр запроса `$count` позволяет включить общее количество элементов коллекции вместе со страницей значений, возвращенных из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f7c95-141">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="f7c95-142">Например, следующий запрос возвращает коллекцию `contacts` текущего пользователя, а также ряд элементов коллекции `contacts` в свойстве `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-142">For example, the following request will return both the `contacts` collection of the current user, and the number of items in the `contacts` collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="f7c95-143">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="f7c95-143">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="f7c95-144">**Примечание.** Параметр `$count` не поддерживается коллекциями ресурсов, производных от [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md), такими как коллекции [user](../api-reference/v1.0/resources/user.md) или [group](../api-reference/v1.0/resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="f7c95-144">**Note:** `$count` is not supported for collections of resources that derive from [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) like collections of [user](../api-reference/v1.0/resources/user.md) or [group](../api-reference/v1.0/resources/group.md).</span></span>

## <a name="expand"></a><span data-ttu-id="f7c95-145">expand</span><span class="sxs-lookup"><span data-stu-id="f7c95-145">expand</span></span>

<span data-ttu-id="f7c95-146">Многие ресурсы Microsoft Graph выводят как объявленные свойства ресурса, так и его связи с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="f7c95-146">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="f7c95-147">Эти связи также называются свойствами ссылки или навигации и могут ссылаться как на один ресурс, так и на коллекцию ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f7c95-147">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="f7c95-148">Например, папки почты, руководитель и подчиненные пользователя выводятся как связи.</span><span class="sxs-lookup"><span data-stu-id="f7c95-148">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="f7c95-p109">Как правило, в одном запросе можно отдельно (но не одновременно) запросить или свойства ресурса, или одно из отношений. С помощью строкового параметра запроса `$expand` в результаты можно включить расширенный ресурс или коллекцию, на которые ссылается одно отношение (свойство навигации).</span><span class="sxs-lookup"><span data-stu-id="f7c95-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="f7c95-151">В приведенном ниже примере возвращаются сведения о корневом каталоге, а также дочерние элементы верхнего уровня на диске.</span><span class="sxs-lookup"><span data-stu-id="f7c95-151">The following example gets root drive information along with the top level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="f7c95-152">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="f7c95-152">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="f7c95-p110">Кроме того, некоторые коллекции ресурсов позволяют указывать свойства, которые должны быть возвращены в расширенных ресурсах, с помощью параметра `$select`. В следующем примере выполняется то же запрос, что и в предыдущем, но используется оператор [`$select`](#select), с помощью которого для расширенных дочерних элементов возвращаются только свойства `id` и `name`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select) statement to limit the properties returned for the expanded child items to the `id` and `name` properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="f7c95-155">[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="f7c95-155">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span></span>

> <span data-ttu-id="f7c95-p111">**Примечание.** Не все отношения и ресурсы поддерживают параметр запроса `$expand`. Например, можно расширить отношения пользователя `directReports`, `manager` и `memberOf`, но не отношения `events`, `messages` или `photo`. Не все ресурсы и отношения поддерживают использование параметра `$select` для расширенных элементов.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the `directReports`, `manager`, and `memberOf` relationships on a user, but you cannot expand its `events`, `messages`, or `photo` relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="f7c95-159">Ресурсы Azure AD, производные от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такие как [user](../api-reference/v1.0/resources/user.md) и [group](../api-reference/v1.0/resources/group.md), поддерживают параметр `$expand` только в `beta`, и обычно он возвращает не более 20 элементов расширенных отношений.</span><span class="sxs-lookup"><span data-stu-id="f7c95-159">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter"></a><span data-ttu-id="f7c95-160">filter</span><span class="sxs-lookup"><span data-stu-id="f7c95-160">filter</span></span>

<span data-ttu-id="f7c95-161">Параметр запроса `$filter` позволяет получить только подмножество объектов коллекции.</span><span class="sxs-lookup"><span data-stu-id="f7c95-161">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="f7c95-162">Например, чтобы найти пользователей, чье отображаемое имя начинается с буквы J, используйте `startswith`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-162">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="f7c95-163">[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="f7c95-163">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span></span>

<span data-ttu-id="f7c95-164">Поддержка операторов `$filter` зависит от того, какой API Microsoft Graph используется.</span><span class="sxs-lookup"><span data-stu-id="f7c95-164">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="f7c95-165">В большинстве случаев поддерживаются следующие операторы:</span><span class="sxs-lookup"><span data-stu-id="f7c95-165">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="f7c95-166">`eq` (равняется);</span><span class="sxs-lookup"><span data-stu-id="f7c95-166">equals (`eq`)</span></span>
- <span data-ttu-id="f7c95-167">`ne` (не равняется);</span><span class="sxs-lookup"><span data-stu-id="f7c95-167">not equals (`ne`)</span></span>
- <span data-ttu-id="f7c95-168">`gt` (больше чем);</span><span class="sxs-lookup"><span data-stu-id="f7c95-168">Greater than (>`gt`)</span></span>
- <span data-ttu-id="f7c95-169">`ge` (не меньше чем);</span><span class="sxs-lookup"><span data-stu-id="f7c95-169">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="f7c95-170">`lt` (меньше чем), `le` (не больше чем);</span><span class="sxs-lookup"><span data-stu-id="f7c95-170">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="f7c95-171">`and` (и);</span><span class="sxs-lookup"><span data-stu-id="f7c95-171">and (`and`)</span></span>
- <span data-ttu-id="f7c95-172">`or` (или);</span><span class="sxs-lookup"><span data-stu-id="f7c95-172"> or `or`.</span></span>
- <span data-ttu-id="f7c95-173">`not` (не).</span><span class="sxs-lookup"><span data-stu-id="f7c95-173">not (`not`)</span></span>
 
<span data-ttu-id="f7c95-174">Часто поддерживается строковый оператор `startswith`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-174">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="f7c95-175">Некоторые API поддерживают лямбда-оператор `any`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-175">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="f7c95-176">Примеры использования см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="f7c95-176">For some  usage examples, see the following table.</span></span> <span data-ttu-id="f7c95-177">Дополнительные сведения о синтаксисе `$filter` см. в [статье о протоколе OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="f7c95-177">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="f7c95-178">Приведенная ниже таблица содержит несколько примеров использования параметра запроса `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-178">The following table shows some examples using the `$filter` query parameter.</span></span>

><span data-ttu-id="f7c95-179">**Примечание.** Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="f7c95-179">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

|<span data-ttu-id="f7c95-180">Описание</span><span class="sxs-lookup"><span data-stu-id="f7c95-180">Description</span></span>|<span data-ttu-id="f7c95-181">Пример</span><span class="sxs-lookup"><span data-stu-id="f7c95-181">Example</span></span>|
|:--------|:-------|
|  <span data-ttu-id="f7c95-182">Поиск пользователей с именем Mary по нескольким свойствам.</span><span class="sxs-lookup"><span data-stu-id="f7c95-182">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| <span data-ttu-id="f7c95-183">Получение всех событий для вошедшего пользователя, которые начинаются после 01.07.2017 г.</span><span class="sxs-lookup"><span data-stu-id="f7c95-183">Get all of the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| <span data-ttu-id="f7c95-184">Получение всех сообщений с определенного адреса, полученных вошедшим пользователем.</span><span class="sxs-lookup"><span data-stu-id="f7c95-184">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| <span data-ttu-id="f7c95-185">Получение всех сообщений, полученных вошедшим пользователем в апреле 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f7c95-185">Get all emails received by the signed-in user in April 2017</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| <span data-ttu-id="f7c95-186">Получение всех непрочитанных сообщений в папке "Входящие" вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7c95-186">Get all unread mails in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| <span data-ttu-id="f7c95-187">Получение списка всех групп Office 365 в организации.</span><span class="sxs-lookup"><span data-stu-id="f7c95-187">List all Office 365 groups in an organization</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |

> <span data-ttu-id="f7c95-p114">**Примечание.** Ресурсы Azure AD не поддерживают следующие операторы `$filter`: `ne`, `gt`, `ge`, `lt`, `le` и `not`. В настоящее время строковый оператор `contains` не поддерживается ни одним ресурсом Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p114">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="orderby"></a><span data-ttu-id="f7c95-190">orderby</span><span class="sxs-lookup"><span data-stu-id="f7c95-190">orderby</span></span>

<span data-ttu-id="f7c95-191">Параметр запроса `$orderby` позволяет указать порядок сортировки элементов, возвращаемых из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f7c95-191">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="f7c95-192">Например, следующий запрос возвращает список пользователей в организации, упорядоченный по отображаемому имени:</span><span class="sxs-lookup"><span data-stu-id="f7c95-192">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[<span data-ttu-id="f7c95-193">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="f7c95-193">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName&method=GET&version=v1.0)

<span data-ttu-id="f7c95-p115">Вы также можете сортировать данные по объектам сложного типа. В следующем запросе сообщения сортируются по полю `address` свойства `from` сложного типа `emailAddress`:</span><span class="sxs-lookup"><span data-stu-id="f7c95-p115">You can also sort by complex type entities. The following request gets messages and sorts them by the `address` field of the `from` property, which is of the complex type `emailAddress`:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="f7c95-196">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="f7c95-196">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="f7c95-197">Чтобы отсортировать результаты по возрастанию или убыванию, добавьте `asc` или `desc` к имени поля, используя пробел для разделения, например: `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-197">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space, for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="f7c95-198">Некоторые API позволяют упорядочивать результаты по нескольким свойствам.</span><span class="sxs-lookup"><span data-stu-id="f7c95-198">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="f7c95-199">Например, приведенный ниже запрос позволяет упорядочить сообщения в папке "Входящие" пользователя сначала по имени отправителей по убыванию (от Я до А), а затем — по возрастанию (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="f7c95-199">With some APIs, you can order results on multiple properties. For example, the following request orders the messages in the user's Inbox first by the name of the person who sent it in descending order (Z to A) and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```
[<span data-ttu-id="f7c95-200">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="f7c95-200">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > <span data-ttu-id="f7c95-201">**Примечание.** Ресурсы Azure AD, производные от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такие как [user](../api-reference/v1.0/resources/user.md) и [group](../api-reference/v1.0/resources/group.md), не позволяют объединять параметр `$orderby` с выражениями `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-201">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search"></a><span data-ttu-id="f7c95-202">поиск</span><span class="sxs-lookup"><span data-stu-id="f7c95-202">search</span></span>

<span data-ttu-id="f7c95-203">Параметр запроса `$search` позволяет ограничить результаты запроса с помощью условия поиска.</span><span class="sxs-lookup"><span data-stu-id="f7c95-203">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="f7c95-p117">**Примечание.** Сейчас можно выполнять поиск **только** в коллекциях [message](../api-reference/v1.0/resources/message.md) и [person](../api-reference/v1.0/resources/person.md). Запрос `$search` возвращает до 250 результатов. В поисковых запросах невозможно указать [`$filter`](#filter) или [`$orderby`](#orderby).</span><span class="sxs-lookup"><span data-stu-id="f7c95-p117">**Note:** You can currently search **only** [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter) or [`$orderby`](#orderby) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="f7c95-207">Использование параметра $search в коллекциях `message`</span><span class="sxs-lookup"><span data-stu-id="f7c95-207">Using $search on `message` collections</span></span>

<span data-ttu-id="f7c95-p118">Условия поиска сообщений указываются с использованием [расширенного синтаксиса запросов (AQS)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7). Результаты сортируются по дате и времени отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p118">Search criteria on messages are expressed using [Advanced Query Syntax (AQS)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7). The results are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="f7c95-210">Вы можете указать следующие свойства для объекта `message` в условии `$search`:</span><span class="sxs-lookup"><span data-stu-id="f7c95-210">You can specify the following properties on a `message` in a `$search` criterion: , , , , , , , , , , , , </span></span>

- `attachments`
- `bccRecipients`
- `body`
- `category`
- `ccRecipients`
- `content`
- `from`
- `hasAttachments`
- `participants`
- `receivedDateTime`
- `sender`
- `subject`
- `toRecipients`

<span data-ttu-id="f7c95-211">Если для поиска в сообщениях указано только значение, используются такие свойства поиска по умолчанию: `from`, `subject` и `body`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-211">If you do a search on messages and specify only a value, the search is carried out on the default search properties of `from`, `subject` and `body`.</span></span>

<span data-ttu-id="f7c95-212">Следующий пример кода возвращает все сообщения из папки "Входящие" вошедшего пользователя, содержащие слово pizza в любом из трех свойств поиска по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="f7c95-212">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="f7c95-213">Следующий пример кода выполняет поиск всех сообщений в папке "Входящие" пользователя, отправленных с определенного электронного адреса: </span><span class="sxs-lookup"><span data-stu-id="f7c95-213">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

### <a name="using-search-on-person-collections"></a><span data-ttu-id="f7c95-214">Использование параметра $search в коллекциях `person`</span><span class="sxs-lookup"><span data-stu-id="f7c95-214">Using $search on `person` collections</span></span>

<span data-ttu-id="f7c95-p119">API People Microsoft Graph можно использовать для получения сведений о наиболее релевантных для пользователя людях. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. API People поддерживает параметр запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p119">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="f7c95-p120">Поиск людей выполняется по свойствам `displayName` и `emailAddress` ресурса [person](../api-reference/v1.0/resources/person.md). В поиске применяется алгоритм нечетких соответствий. Возвращаются результаты, основанные на точном совпадении, а также на выводы, связанные с целью поиска. Предположим, в коллекции `people` вошедшего в систему пользователя есть пользователь с отображаемым именем Tyler Lee и электронным адресом tylerle@example.com. Во всех приведенных ниже примерах поиск возвращает результаты, содержащие имя Tyler.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p120">Searches on people occur on both the `displayName` and `emailAddress` properties of the [person](../api-reference/v1.0/resources/person.md) resource. Searches implement a fuzzy matching algorithm. They will return results based on an exact match and also on inferences about the intent of the search. For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the `people` collection of the signed-in user. All of the following searches will return results that contain Tyler.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

<span data-ttu-id="f7c95-p121">Можно также выполнить поиск людей, которым интересна определенная тема. Поиск выполняется на основе заключений, выведенных из переписки пользователя по электронной почте. Например, приведенный ниже поиск возвращает список людей, релевантных для вошедшего в систему пользователя, которые в беседах с ним интересовались пиццей. Обратите внимание, что фраза для поиска заключена в кавычки.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p121">You can also perform searches for people who are interested in a particular topic. Searches are performed based on inferences derived from the user's mail conversations. For example, the following search will return a collection of people relevant to the signed-in user who have expressed an interest in pizza in communications with that user. Note that the search phrase is enclosed in quotes.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

<span data-ttu-id="f7c95-227">И, наконец, в одном запросе можно объединить поиск людей и тем, используя вместе два вида выражений поиска.</span><span class="sxs-lookup"><span data-stu-id="f7c95-227">Finally, you can combine both people searches and topic searches in the same request by combining the two types of search expression.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```
<span data-ttu-id="f7c95-228">В этом запросе фактически выполняется два поиска: нечеткий поиск по свойствам `displayName` и `emailAddress` людей, релевантных для вошедшего пользователя, и поиск по теме "pizza" в отношении этих людей.</span><span class="sxs-lookup"><span data-stu-id="f7c95-228">This request essentially conducts two searches: a fuzzy search against `displayName` and `emailAddress` properties of the signed-in user's relevant people and a topic search for "pizza" against the user's relevant people. The results are then ranked, ordered, and returned. Note that the search is not restrictive; you may get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span> <span data-ttu-id="f7c95-229">Результаты ранжируются, упорядочиваются и возвращаются.</span><span class="sxs-lookup"><span data-stu-id="f7c95-229">The results are then ranked, ordered, and returned.</span></span> <span data-ttu-id="f7c95-230">Обратите внимание, что поиск не имеет ограничений, поэтому результаты могут содержать список пользователей с нечетким соответствием имени "tyl" или пользователей, интересующихся темой "pizza", или и тех, и других.</span><span class="sxs-lookup"><span data-stu-id="f7c95-230">Note that the search is not restrictive; you might get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span>

<span data-ttu-id="f7c95-231">Дополнительные сведения об API поиска людей см. в статье [Получение сведений о релевантных людях](./people_example.md).</span><span class="sxs-lookup"><span data-stu-id="f7c95-231">To learn more about the People API, see [Get information about relevant people](./people_example.md).</span></span>  

## <a name="select"></a><span data-ttu-id="f7c95-232">select</span><span class="sxs-lookup"><span data-stu-id="f7c95-232">select</span></span>

<span data-ttu-id="f7c95-233">Параметр запроса `$select` позволяет возвратить набор свойств, отличный от набора по умолчанию, для отдельного ресурса или коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f7c95-233">Use the `$select` query parameter to return a set of properties different than the default set for an individual resource or a collection of resources. With $select you can specify a subset or a superset of the default properties.</span></span> <span data-ttu-id="f7c95-234">С помощью параметра $select можно указать подмножество или супермножество свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f7c95-234">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="f7c95-235">Например, при получении сообщений вошедшего пользователя можно указать, что необходимо вернуть только свойства `from` и `subject`:</span><span class="sxs-lookup"><span data-stu-id="f7c95-235">For example, when retrieving the messages of the signed-in user, you can specify that only the `from` and `subject` properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[<span data-ttu-id="f7c95-236">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="f7c95-236">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$select=from,subject&method=GET&version=v1.0)

> <span data-ttu-id="f7c95-237">**Важно!** Как правило, параметр `$select` рекомендуется использовать, чтобы запрос возвращал только те свойства, которые необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="f7c95-237">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="f7c95-238">Это особенно касается запросов, которые могут возвращать большой результирующий набор.</span><span class="sxs-lookup"><span data-stu-id="f7c95-238">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="f7c95-239">Ограничение набора свойств, возвращаемых в каждой строке, позволяет уменьшить сетевую нагрузку и повысить производительность вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="f7c95-239">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="f7c95-p125">В `v1.0` некоторые ресурсы Azure AD, производные от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такие как [user](../api-reference/v1.0/resources/user.md) и [group](../api-reference/v1.0/resources/group.md), возвращают при чтении ограниченное подмножество свойств по умолчанию. С этими ресурсами параметр `$select` необходимо использовать для возврата свойств, не входящих в набор по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p125">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip"></a><span data-ttu-id="f7c95-242">skip</span><span class="sxs-lookup"><span data-stu-id="f7c95-242">skip</span></span>

<span data-ttu-id="f7c95-p126">Параметр запроса `$skip` позволяет задать количество элементов, которое необходимо пропустить в начале коллекции. Например, следующий запрос возвращает события пользователя, отсортированные по дате создания, начиная с 21-го события в коллекции:</span><span class="sxs-lookup"><span data-stu-id="f7c95-p126">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[<span data-ttu-id="f7c95-245">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="f7c95-245">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$orderby=createdDateTime&$skip=20&method=GET&version=v1.0)

> <span data-ttu-id="f7c95-246">**Примечание.** Некоторые API Microsoft Graph, например для почты и календарей Outlook (`message`, `event`, `calendar`), используют `$skip` для разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="f7c95-246">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (`message`, `event`, and `calendar`), use `$skip` to implement paging.</span></span> <span data-ttu-id="f7c95-247">Если результаты запроса занимают несколько страниц, эти API возвращают свойство `@odata:nextLink` с URL-адресом, содержащим параметр `$skip`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-247">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="f7c95-248">Этот URL-адрес можно использовать для возврата следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="f7c95-248">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="f7c95-249">Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="f7c95-249">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken"></a><span data-ttu-id="f7c95-250">skipToken</span><span class="sxs-lookup"><span data-stu-id="f7c95-250">skipToken</span></span>

<span data-ttu-id="f7c95-p128">Некоторые запросы возвращают несколько страниц данных. Это происходит из-за разбиения по страницам на стороне сервера или из-за использования параметра [`$top`](#top), который ограничивает размер возвращаемых страниц. Многие API Microsoft Graph используют параметр запроса `skipToken` для ссылки на следующие страницы результатов. Параметр `$skiptoken` содержит непрозрачный маркер, который ссылается на следующую страницу результатов и возвращается в URL-адресе, указанном в свойстве `@odata.nextLink`. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="f7c95-p128">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top"></a><span data-ttu-id="f7c95-255">top</span><span class="sxs-lookup"><span data-stu-id="f7c95-255">top</span></span>

<span data-ttu-id="f7c95-256">Параметр запроса `$top` позволяет задать размер страницы в результирующем наборе.</span><span class="sxs-lookup"><span data-stu-id="f7c95-256">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="f7c95-257">Если результирующий набор будет содержать больше одной страницы элементов, тело отклика будет содержать параметр `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-257">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="f7c95-258">Этот параметр содержит URL-адрес, с помощью которого можно получить следующую страницу результатов.</span><span class="sxs-lookup"><span data-stu-id="f7c95-258">If there are more items remaining in the result set, the response body will contain an  parameter. This parameter contains a URL that you can use to get the next page of results. To learn more, see Paging.</span></span> <span data-ttu-id="f7c95-259">Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="f7c95-259">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="f7c95-260">Например, следующий запрос возвращает первые пять сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="f7c95-260">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[<span data-ttu-id="f7c95-261">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="f7c95-261">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=5&method=GET&version=v1.0)


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="f7c95-262">Обработка ошибок параметров запроса</span><span class="sxs-lookup"><span data-stu-id="f7c95-262">Error handling for query parameters</span></span>

<span data-ttu-id="f7c95-p130">Некоторые запросы возвращают сообщение об ошибке, если указанный параметр запроса не поддерживается. Например, невозможно использовать `$expand` для связи `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="f7c95-p130">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

<span data-ttu-id="f7c95-265">При этом необходимо отметить, что указанные в запросе параметры могут просто не сработать.</span><span class="sxs-lookup"><span data-stu-id="f7c95-265">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="f7c95-266">Это может произойти, если не поддерживаются либо сами параметры, либо их сочетание.</span><span class="sxs-lookup"><span data-stu-id="f7c95-266">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="f7c95-267">В таких случаях необходимо проверить возвращенные запросом данные и определить, дали ли указанные параметры запроса желаемый результат.</span><span class="sxs-lookup"><span data-stu-id="f7c95-267">However, it is important to note that query parameters specified in a request may fail silently. This can be true for unsupported query parameters as well as for unsupported combinations of query parameters. In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356