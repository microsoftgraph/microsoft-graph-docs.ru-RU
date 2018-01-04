# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="58c8c-101">Настройка ответов с помощью параметров запроса</span><span class="sxs-lookup"><span data-stu-id="58c8c-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="58c8c-p101">В Microsoft Graph предусмотрены необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных. Поддерживаются указанные ниже параметры запросов.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following query parameters are supported.</span></span>

><span data-ttu-id="58c8c-104">**Примечание.** Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="58c8c-104">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="58c8c-105">Имя</span><span class="sxs-lookup"><span data-stu-id="58c8c-105">Name</span></span>                     | <span data-ttu-id="58c8c-106">Описание</span><span class="sxs-lookup"><span data-stu-id="58c8c-106">Description</span></span> | <span data-ttu-id="58c8c-107">Пример</span><span class="sxs-lookup"><span data-stu-id="58c8c-107">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="58c8c-108">$count</span><span class="sxs-lookup"><span data-stu-id="58c8c-108">$count</span></span>](#count-parameter)         | <span data-ttu-id="58c8c-109">Возвращает общее количество соответствующих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="58c8c-109">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="58c8c-110">$expand</span><span class="sxs-lookup"><span data-stu-id="58c8c-110">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="58c8c-111">Получает связанные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="58c8c-111">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="58c8c-112">$filter</span><span class="sxs-lookup"><span data-stu-id="58c8c-112">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="58c8c-113">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="58c8c-113">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="58c8c-114">$format</span><span class="sxs-lookup"><span data-stu-id="58c8c-114">$format</span></span>](#format-parameter)       | <span data-ttu-id="58c8c-115">Возвращает результаты в указанном формате мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="58c8c-115">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="58c8c-116">$orderby</span><span class="sxs-lookup"><span data-stu-id="58c8c-116">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="58c8c-117">Упорядочивает результаты.</span><span class="sxs-lookup"><span data-stu-id="58c8c-117">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="58c8c-118">$search</span><span class="sxs-lookup"><span data-stu-id="58c8c-118">$search</span></span>](#search-parameter)       | <span data-ttu-id="58c8c-p102">Возвращает результаты на основании условий поиска. В настоящее время поддерживается в коллекциях **messages** и **person**.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p102">Returns results based on search criteria. Currently supported on **** and **** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="58c8c-121">$select</span><span class="sxs-lookup"><span data-stu-id="58c8c-121">$select</span></span>](#select-parameter)       | <span data-ttu-id="58c8c-122">Фильтрует свойства (столбцы).</span><span class="sxs-lookup"><span data-stu-id="58c8c-122">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="58c8c-123">$skip</span><span class="sxs-lookup"><span data-stu-id="58c8c-123">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="58c8c-p103">Применяется для индексации в результирующем наборе. Также используется некоторыми API для разбиения по страницам и может использоваться вместе с параметром `$top` для разбиения результатов по страницам вручную.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="58c8c-126">$skipToken</span><span class="sxs-lookup"><span data-stu-id="58c8c-126">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="58c8c-p104">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц. (Вместо этого параметра некоторые API используют `$skip`.)</span><span class="sxs-lookup"><span data-stu-id="58c8c-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|
| [<span data-ttu-id="58c8c-129">$top</span><span class="sxs-lookup"><span data-stu-id="58c8c-129">$top</span></span>](#top-parameter)             | <span data-ttu-id="58c8c-130">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="58c8c-130">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]



<span data-ttu-id="58c8c-131">Эти параметры совместимы с [языком запросов OData версии 4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="58c8c-131">These parameters are compatible with the [OData V4 query language][odata-query].</span></span> <span data-ttu-id="58c8c-132">Параметры, которые поддерживаются всеми API Microsoft Graph для конечной точки `v1.0`, могут значительно отличаться от таковых для конечной точки `beta`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-132">Not all parameters are supported across all Microsoft Graph APIs, and support might differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="58c8c-p106">**Примечание.** В конечной точке `beta` префикс `$` является необязательным. Например, вместо `$filter` можно использовать `filter`. Дополнительные сведения и примеры см. в статье [Поддержка параметров запросов без префиксов $ в Microsoft Graph]((http://dev.office.com/queryparametersinMicrosoftGraph)).</span><span class="sxs-lookup"><span data-stu-id="58c8c-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph]((http://dev.office.com/queryparametersinMicrosoftGraph)).</span></span>

## <a name="encoding-query-parameters"></a><span data-ttu-id="58c8c-136">Кодирование параметров запроса</span><span class="sxs-lookup"><span data-stu-id="58c8c-136">Encoding query parameters</span></span>

<span data-ttu-id="58c8c-137">К значениям параметров запросов нужно применить процентное кодирование.</span><span class="sxs-lookup"><span data-stu-id="58c8c-137">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="58c8c-138">Многие клиенты HTTP, браузеры и инструменты (например, [песочница Graph][graph-explorer]) помогут вам в этом.</span><span class="sxs-lookup"><span data-stu-id="58c8c-138">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="58c8c-139">Если запрос неудачный, одна из возможных причин — не удалось должным образом закодировать значения параметров запросов.</span><span class="sxs-lookup"><span data-stu-id="58c8c-139">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="58c8c-140">URL-адрес, который не было закодирован, выглядит так:</span><span class="sxs-lookup"><span data-stu-id="58c8c-140">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="58c8c-141">Закодированный должным образом URL-адрес выглядит так:</span><span class="sxs-lookup"><span data-stu-id="58c8c-141">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a><span data-ttu-id="58c8c-142">Параметр count</span><span class="sxs-lookup"><span data-stu-id="58c8c-142">count parameter</span></span>

<span data-ttu-id="58c8c-143">Параметр запроса `$count` позволяет включить общее количество элементов коллекции вместе со страницей значений, возвращенных из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58c8c-143">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="58c8c-144">Например, приведенный ниже запрос возвращает коллекцию **contact** текущего пользователя, а также ряд элементов коллекции **contact** в свойстве `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-144">For example, the following request will return both the **** collection of the current user, and the number of items in the **** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="58c8c-145">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="58c8c-145">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="58c8c-146">**Примечание.** Параметр `$count` не поддерживается коллекциями ресурсов, производных от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такими как коллекции [users](../api-reference/v1.0/resources/user.md) или [groups](../api-reference/v1.0/resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="58c8c-146">Note:  is not supported for collections of resources that derive from    like collections of users or groups.</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="58c8c-147">Параметр expand</span><span class="sxs-lookup"><span data-stu-id="58c8c-147">expand parameter</span></span>

<span data-ttu-id="58c8c-148">Многие ресурсы Microsoft Graph возвращают как объявленные свойства ресурса, так и его связи с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="58c8c-148">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="58c8c-149">Эти связи также называются свойствами ссылки или навигации и могут ссылаться как на один ресурс, так и на коллекцию ресурсов.</span><span class="sxs-lookup"><span data-stu-id="58c8c-149">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="58c8c-150">Например, папки почты, руководитель и подчиненные пользователя выводятся как связи.</span><span class="sxs-lookup"><span data-stu-id="58c8c-150">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="58c8c-p109">Как правило, в одном запросе можно отдельно (но не одновременно) запросить или свойства ресурса, или одно из отношений. С помощью строкового параметра запроса `$expand` в результаты можно включить расширенный ресурс или коллекцию, на которые ссылается одно отношение (свойство навигации).</span><span class="sxs-lookup"><span data-stu-id="58c8c-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="58c8c-153">В приведенном ниже примере возвращаются сведения о корневом каталоге, а также дочерние элементы верхнего уровня на диске.</span><span class="sxs-lookup"><span data-stu-id="58c8c-153">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="58c8c-154">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="58c8c-154">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="58c8c-p110">Кроме того, некоторые коллекции ресурсов позволяют указывать свойства, которые должны быть возвращены в расширенных ресурсах, благодаря параметру `$select`. В следующем примере выполняется тот же запрос, что и в предыдущем, но используется оператор [`$select`](#select-parameter), с помощью которого для расширенных дочерних элементов возвращаются только свойства **id** и **name**.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **** and **** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="58c8c-157">[Попробовать в песочнице Graph][expand-example]</span><span class="sxs-lookup"><span data-stu-id="58c8c-157">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="58c8c-p111">**Примечание.** Не все связи и ресурсы поддерживают параметр запроса `$expand`. Например, можно расширить связи пользователя **directReports**, **manager** и **memberOf**, но не связи **events**, **messages** или **photo**. Не все ресурсы и связи поддерживают использование параметра `$select` для расширенных элементов.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the ****, ****, and **** relationships on a user, but you cannot expand its ****, ****, or **** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="58c8c-161">Ресурсы Azure AD, производные от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такие как [user](../api-reference/v1.0/resources/user.md) и [group](../api-reference/v1.0/resources/group.md), поддерживают параметр `$expand` только в `beta`, и обычно он возвращает не более 20 элементов расширенных отношений.</span><span class="sxs-lookup"><span data-stu-id="58c8c-161">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="58c8c-162">Параметр filter</span><span class="sxs-lookup"><span data-stu-id="58c8c-162">PivotTable filter parameter</span></span>

<span data-ttu-id="58c8c-163">Параметр запроса `$filter` позволяет получить только подмножество объектов коллекции.</span><span class="sxs-lookup"><span data-stu-id="58c8c-163">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="58c8c-164">Например, чтобы найти пользователей, чье отображаемое имя начинается с буквы J, используйте `startswith`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-164">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="58c8c-165">[Попробовать в песочнице Graph][filter-example]</span><span class="sxs-lookup"><span data-stu-id="58c8c-165">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="58c8c-166">Поддержка операторов `$filter` зависит от того, какой API Microsoft Graph используется.</span><span class="sxs-lookup"><span data-stu-id="58c8c-166">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="58c8c-167">В большинстве случаев поддерживаются следующие операторы:</span><span class="sxs-lookup"><span data-stu-id="58c8c-167">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="58c8c-168">`eq` (равняется);</span><span class="sxs-lookup"><span data-stu-id="58c8c-168">equals (`eq`)</span></span>
- <span data-ttu-id="58c8c-169">`ne` (не равняется);</span><span class="sxs-lookup"><span data-stu-id="58c8c-169">not equals (`ne`)</span></span>
- <span data-ttu-id="58c8c-170">`gt` (больше чем);</span><span class="sxs-lookup"><span data-stu-id="58c8c-170">greater than (`gt`)</span></span>
- <span data-ttu-id="58c8c-171">`ge` (не меньше чем);</span><span class="sxs-lookup"><span data-stu-id="58c8c-171">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="58c8c-172">`lt` (меньше чем), `le` (не больше чем);</span><span class="sxs-lookup"><span data-stu-id="58c8c-172">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="58c8c-173">`and` (и);</span><span class="sxs-lookup"><span data-stu-id="58c8c-173">and (`and`)</span></span>
- <span data-ttu-id="58c8c-174">`or` (или);</span><span class="sxs-lookup"><span data-stu-id="58c8c-174">or (`or`)</span></span>
- <span data-ttu-id="58c8c-175">`not` (не).</span><span class="sxs-lookup"><span data-stu-id="58c8c-175">not (`not`)</span></span>
 
<span data-ttu-id="58c8c-176">Часто поддерживается строковый оператор `startswith`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-176">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="58c8c-177">Некоторые API поддерживают лямбда-оператор `any`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-177">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="58c8c-178">Примеры использования см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="58c8c-178">For some  usage examples, see the following table.</span></span> <span data-ttu-id="58c8c-179">Дополнительные сведения о синтаксисе `$filter` см. в [статье о протоколе OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="58c8c-179">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="58c8c-180">Приведенная ниже таблица содержит несколько примеров использования параметра запроса `$filter`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-180">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="58c8c-181">**Примечание.** Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="58c8c-181">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="58c8c-182">Описание</span><span class="sxs-lookup"><span data-stu-id="58c8c-182">Description</span></span> | <span data-ttu-id="58c8c-183">Пример</span><span class="sxs-lookup"><span data-stu-id="58c8c-183">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="58c8c-184">Поиск пользователей с именем Mary по нескольким свойствам.</span><span class="sxs-lookup"><span data-stu-id="58c8c-184">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="58c8c-185">Получение всех событий для вошедшего пользователя, которые начинаются после 01.07.2017 г.</span><span class="sxs-lookup"><span data-stu-id="58c8c-185">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="58c8c-186">Получение всех сообщений с определенного адреса, полученных вошедшим пользователем.</span><span class="sxs-lookup"><span data-stu-id="58c8c-186">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="58c8c-187">Получение всех сообщений, полученных вошедшим пользователем в апреле 2017 г.</span><span class="sxs-lookup"><span data-stu-id="58c8c-187">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="58c8c-188">Получение всех непрочитанных сообщений в папке "Входящие" вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="58c8c-188">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="58c8c-189">Получение списка всех групп Office 365 в организации.</span><span class="sxs-lookup"><span data-stu-id="58c8c-189">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="58c8c-p114">**Примечание.** Ресурсы Azure AD не поддерживают следующие операторы `$filter`: `ne`, `gt`, `ge`, `lt`, `le` и `not`. В настоящее время строковый оператор `contains` не поддерживается ни одним ресурсом Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p114">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="58c8c-192">Параметр format</span><span class="sxs-lookup"><span data-stu-id="58c8c-192">format parameter</span></span>

<span data-ttu-id="58c8c-193">Параметр запроса `$format` позволяет указать формат мультимедиа для элементов, возвращаемых из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58c8c-193">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="58c8c-194">Например, указанный ниже запрос возвращает список пользователей организации в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58c8c-194">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="58c8c-195">[Попробовать в песочнице Graph][format-example]</span><span class="sxs-lookup"><span data-stu-id="58c8c-195">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="58c8c-196">**Примечание.** Параметр запросов `$format` поддерживает ряд форматов (например, Atom, XML и JSON), но результаты могут не возвращаться во всех форматах.</span><span class="sxs-lookup"><span data-stu-id="58c8c-196">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="58c8c-197">Параметр orderby</span><span class="sxs-lookup"><span data-stu-id="58c8c-197">orderby parameter</span></span>

<span data-ttu-id="58c8c-198">Параметр запроса `$orderby` позволяет указать порядок сортировки элементов, возвращаемых из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58c8c-198">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="58c8c-199">Например, следующий запрос возвращает список пользователей в организации, упорядоченный по отображаемому имени:</span><span class="sxs-lookup"><span data-stu-id="58c8c-199">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="58c8c-200">[Попробовать в песочнице Graph][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="58c8c-200">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="58c8c-p115">Вы также можете сортировать данные по объектам сложного типа. Приведенный ниже запрос позволяет получить сообщения и отсортировать их по полю **address** свойства **from**, принадлежащего к сложному типу **emailAddress**.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p115">You can also sort by complex type entities. The following example gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="58c8c-203">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="58c8c-203">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="58c8c-204">Чтобы отсортировать результаты по возрастанию или убыванию, добавьте `asc` или `desc` к имени поля, используя пробел для разделения, например: `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-204">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="58c8c-205">Некоторые API позволяют упорядочивать результаты по нескольким свойствам.</span><span class="sxs-lookup"><span data-stu-id="58c8c-205">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="58c8c-206">Например, приведенный ниже запрос позволяет упорядочить сообщения в папке "Входящие" пользователя сначала по имени отправителей по убыванию (от Я до А), а затем — по возрастанию (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="58c8c-206">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="58c8c-207">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="58c8c-207">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > <span data-ttu-id="58c8c-208">**Примечание.** Ресурсы Azure AD, производные от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такие как [user](../api-reference/v1.0/resources/user.md) и [group](../api-reference/v1.0/resources/group.md), не позволяют объединять параметр `$orderby` с выражениями `$filter`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-208">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="58c8c-209">Параметр search</span><span class="sxs-lookup"><span data-stu-id="58c8c-209">search parameter</span></span>

<span data-ttu-id="58c8c-210">Параметр запроса `$search` позволяет ограничить результаты запроса с помощью условия поиска.</span><span class="sxs-lookup"><span data-stu-id="58c8c-210">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="58c8c-p117">**Примечание.** Сейчас можно выполнять поиск **только** в коллекциях [message](../api-reference/v1.0/resources/message.md) и [person](../api-reference/v1.0/resources/person.md). Запрос `$search` возвращает до 250 результатов. В поисковых запросах невозможно указать [`$filter`](#filter-parameter) или [`$orderby`](#orderby-parameter).</span><span class="sxs-lookup"><span data-stu-id="58c8c-p117">**Note:** You can currently search **only** [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="58c8c-214">Использование параметра $search в коллекциях message</span><span class="sxs-lookup"><span data-stu-id="58c8c-214">Using $search on  collections</span></span>

<span data-ttu-id="58c8c-215">Приложения Office 365, такие как Outlook и SharePoint, поддерживают синтаксис KQL (Keyword Query Language) для поиска.</span><span class="sxs-lookup"><span data-stu-id="58c8c-215">Office 365 applications, such as Outlook and SharePoint, support the Keyword Query Language (KQL) syntax to do searches.</span></span> <span data-ttu-id="58c8c-216">Благодаря этому возможно использование общего домена обнаружения для соответствующих хранилищ данных.</span><span class="sxs-lookup"><span data-stu-id="58c8c-216">This provides the convenience of a common discovery domain for their data stores.</span></span> 

<span data-ttu-id="58c8c-217">При поиске в коллекциях message результаты сортируются по дате и времени отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="58c8c-217">When you search message collections, the results are sorted by the date and time that the message was sent.</span></span> 

<span data-ttu-id="58c8c-218">Вы можете указать следующие свойства для объекта **message** в условии `$search`:</span><span class="sxs-lookup"><span data-stu-id="58c8c-218">You can specify the following properties on a **** in a `$search` criterion:</span></span>

- <span data-ttu-id="58c8c-219">**attachments**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-219">**attachments**</span></span>
- <span data-ttu-id="58c8c-220">**bccRecipients**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-220">**bccRecipients**</span></span>
- <span data-ttu-id="58c8c-221">**body**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-221">**body**</span></span>
- <span data-ttu-id="58c8c-222">**category**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-222">**Category**</span></span>
- <span data-ttu-id="58c8c-223">**ccRecipients**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-223">**ccRecipients**</span></span>
- <span data-ttu-id="58c8c-224">**content**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-224">**content**</span></span>
- <span data-ttu-id="58c8c-225">**from**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-225">**from**</span></span>
- <span data-ttu-id="58c8c-226">**hasAttachments**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-226">**hasAttachments**</span></span>
- <span data-ttu-id="58c8c-227">**participants**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-227">**participants**</span></span>
- <span data-ttu-id="58c8c-228">**receivedDateTime**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-228">**receivedDateTime**</span></span>
- <span data-ttu-id="58c8c-229">**sender**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-229">**sender**</span></span>
- <span data-ttu-id="58c8c-230">**subject**;</span><span class="sxs-lookup"><span data-stu-id="58c8c-230">**subject**</span></span>
- <span data-ttu-id="58c8c-231">**toRecipients**.</span><span class="sxs-lookup"><span data-stu-id="58c8c-231">**toRecipients**</span></span>

<span data-ttu-id="58c8c-232">Если при поиске сообщений указано только значение, поиск выполняется по свойствам поиска по умолчанию: **from**, **subject** и **body**.</span><span class="sxs-lookup"><span data-stu-id="58c8c-232">If you do a search on messages and specify only a value, the search is carried out on the default search properties of **from**, **subject** and **body**.</span></span>

<span data-ttu-id="58c8c-233">Следующий пример кода возвращает все сообщения из папки "Входящие" вошедшего пользователя, содержащие слово "pizza" в любом из трех свойств поиска по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="58c8c-233">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="58c8c-234">[Попробовать в песочнице Graph][search-example]</span><span class="sxs-lookup"><span data-stu-id="58c8c-234">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="58c8c-235">Следующий пример кода выполняет поиск всех сообщений в папке "Входящие" пользователя, отправленных с определенного электронного адреса:</span><span class="sxs-lookup"><span data-stu-id="58c8c-235">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```
<span data-ttu-id="58c8c-236">Дополнительные сведения о KQL (например, касательно синтаксиса, поддерживаемых операторов, подсказок для поиска) вы найдете в таких статьях:</span><span class="sxs-lookup"><span data-stu-id="58c8c-236">For more information about KQL such as the syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="58c8c-237">[Руководство по синтаксису языка запросов по ключевым словам (KQL)]((https://docs.microsoft.com/ru-RU/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference));</span><span class="sxs-lookup"><span data-stu-id="58c8c-237">[Keyword Query Language (KQL) syntax reference]((https://docs.microsoft.com/ru-RU/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference))</span></span>

- <span data-ttu-id="58c8c-238">
  [Свойства сообщений и операторы поиска для обнаружения электронных данных на месте в Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx).</span><span class="sxs-lookup"><span data-stu-id="58c8c-238">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="58c8c-239">Использование параметра $search в коллекциях person</span><span class="sxs-lookup"><span data-stu-id="58c8c-239">Using $search on  collections</span></span>

<span data-ttu-id="58c8c-p119">API People Microsoft Graph можно использовать для получения сведений о наиболее релевантных для пользователя людях. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. API People поддерживает параметр запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p119">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="58c8c-243">Поиск людей выполняется по свойствам **displayName** и **emailAddress** ресурса [person](../api-reference/v1.0/resources/person.md).</span><span class="sxs-lookup"><span data-stu-id="58c8c-243">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](../api-reference/v1.0/resources/person.md) resource.</span></span> <span data-ttu-id="58c8c-244">В поиске применяется алгоритм нечетких соответствий.</span><span class="sxs-lookup"><span data-stu-id="58c8c-244">Searches implement a fuzzy matching algorithm.</span></span> <span data-ttu-id="58c8c-245">Возвращаются результаты, основанные на точном совпадении, а также на выводы, связанные с целью поиска.</span><span class="sxs-lookup"><span data-stu-id="58c8c-245">They will return results based on an exact match and also on inferences about the intent of the search.</span></span> <span data-ttu-id="58c8c-246">Предположим, в коллекции **people** вошедшего пользователя есть пользователь с отображаемым именем Tyler Lee и электронным адресом tylerle@example.com.</span><span class="sxs-lookup"><span data-stu-id="58c8c-246">For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="58c8c-247">Все приведенные ниже примеры запросов поиска возвращают результаты, содержащие имя Tyler.</span><span class="sxs-lookup"><span data-stu-id="58c8c-247">All of the following searches will return results that contain Tyler.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

<span data-ttu-id="58c8c-p121">Можно также выполнить поиск людей, которым интересна определенная тема. Поиск выполняется на основе заключений, выведенных из переписки пользователя по электронной почте. Например, приведенный ниже поиск возвращает список людей, релевантных для вошедшего в систему пользователя, которые в беседах с ним интересовались пиццей. Обратите внимание, что фраза для поиска заключена в кавычки.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p121">You can also perform searches for people who are interested in a particular topic. Searches are performed based on inferences derived from the user's mail conversations. For example, the following search will return a collection of people relevant to the signed-in user who have expressed an interest in pizza in communications with that user. Note that the search phrase is enclosed in quotes.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

<span data-ttu-id="58c8c-252">И, наконец, в одном запросе можно объединить поиск людей и тем, используя вместе два вида выражений поиска.</span><span class="sxs-lookup"><span data-stu-id="58c8c-252">Finally, you can combine both people searches and topic searches in the same request by combining the two types of search expression.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```

<span data-ttu-id="58c8c-253">В этом запросе фактически выполняется два поиска: поиск нечетких соответствий по свойствам **displayName** и **emailAddress** в отношении людей, релевантных для вошедшего пользователя, и поиск по теме "pizza" в отношении этих людей.</span><span class="sxs-lookup"><span data-stu-id="58c8c-253">This request essentially conducts two searches: a fuzzy search against **** and **** properties of the signed-in user's relevant people, and a topic search for "pizza" against the user's relevant people.</span></span> <span data-ttu-id="58c8c-254">Результаты ранжируются, упорядочиваются и возвращаются.</span><span class="sxs-lookup"><span data-stu-id="58c8c-254">The results are then ranked, ordered, and returned.</span></span> <span data-ttu-id="58c8c-255">Обратите внимание, что поиск не имеет ограничений, поэтому результаты могут содержать список пользователей с нечетким соответствием имени "tyl" или пользователей, интересующихся темой "pizza", или и тех, и других.</span><span class="sxs-lookup"><span data-stu-id="58c8c-255">Note that the search is not restrictive; you might get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span>

<span data-ttu-id="58c8c-256">Дополнительные сведения об API поиска людей см. в статье [Получение сведений о релевантных людях](./people_example.md).</span><span class="sxs-lookup"><span data-stu-id="58c8c-256">To learn more about the People API, see [Get information about relevant people](./people_example.md).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="58c8c-257">Параметр select</span><span class="sxs-lookup"><span data-stu-id="58c8c-257">select parameter</span></span>

<span data-ttu-id="58c8c-258">Параметр запроса `$select` позволяет возвратить набор свойств, отличный от набора по умолчанию, для отдельного ресурса или коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="58c8c-258">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="58c8c-259">С помощью параметра $select можно указать подмножество или супермножество свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58c8c-259">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="58c8c-260">Например, при получении сообщений вошедшего пользователя можно указать, что необходимо вернуть только свойства **from** и **subject**:</span><span class="sxs-lookup"><span data-stu-id="58c8c-260">For example, when retrieving the messages of the signed-in user, you can specify that only the **** and **** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="58c8c-261">[Попробовать в песочнице Graph][select-example]</span><span class="sxs-lookup"><span data-stu-id="58c8c-261">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="58c8c-262">**Важно!** Как правило, параметр `$select` рекомендуется использовать, чтобы запрос возвращал только те свойства, которые необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="58c8c-262">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="58c8c-263">Это особенно касается запросов, которые могут возвращать большой результирующий набор.</span><span class="sxs-lookup"><span data-stu-id="58c8c-263">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="58c8c-264">Ограничение набора свойств, возвращаемых в каждой строке, позволяет уменьшить сетевую нагрузку и повысить производительность вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="58c8c-264">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="58c8c-p125">В `v1.0` некоторые ресурсы Azure AD, производные от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такие как [user](../api-reference/v1.0/resources/user.md) и [group](../api-reference/v1.0/resources/group.md), возвращают при чтении ограниченное подмножество свойств по умолчанию. С этими ресурсами параметр `$select` необходимо использовать для возврата свойств, не входящих в набор по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p125">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="58c8c-267">Параметр skip</span><span class="sxs-lookup"><span data-stu-id="58c8c-267">skip parameter</span></span>

<span data-ttu-id="58c8c-p126">Параметр запроса `$skip` позволяет задать количество элементов, которое необходимо пропустить в начале коллекции. Например, следующий запрос возвращает события пользователя, отсортированные по дате создания, начиная с 21-го события в коллекции:</span><span class="sxs-lookup"><span data-stu-id="58c8c-p126">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="58c8c-270">[Попробовать в песочнице Graph][skip-example]</span><span class="sxs-lookup"><span data-stu-id="58c8c-270">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="58c8c-271">**Примечание.** Некоторые API Microsoft Graph, например для почты и календарей Outlook (**message**, **event** и **calendar**), используют `$skip` для разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="58c8c-271">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (****, ****, and ****), use `$skip` to implement paging.</span></span> <span data-ttu-id="58c8c-272">Если результаты запроса занимают несколько страниц, эти API возвращают свойство `@odata:nextLink` с URL-адресом, содержащим параметр `$skip`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-272">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="58c8c-273">Этот URL-адрес можно использовать для возврата следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="58c8c-273">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="58c8c-274">[Подробнее…](./paging.md)</span><span class="sxs-lookup"><span data-stu-id="58c8c-274">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="58c8c-275">Параметр skipToken</span><span class="sxs-lookup"><span data-stu-id="58c8c-275">skipToken parameter</span></span>

<span data-ttu-id="58c8c-p128">Некоторые запросы возвращают несколько страниц данных. Это происходит из-за разбиения по страницам на стороне сервера или из-за использования параметра [`$top`](#top-parameter), который ограничивает размер возвращаемых страниц. Многие API Microsoft Graph используют параметр запроса `skipToken` для ссылки на следующие страницы результатов. Параметр `$skiptoken` содержит непрозрачный маркер, который ссылается на следующую страницу результатов и возвращается в URL-адресе, указанном в свойстве `@odata.nextLink`. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="58c8c-p128">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="58c8c-280">Параметр top</span><span class="sxs-lookup"><span data-stu-id="58c8c-280">top parameter</span></span>

<span data-ttu-id="58c8c-281">Параметр запроса `$top` позволяет задать размер страницы в результирующем наборе.</span><span class="sxs-lookup"><span data-stu-id="58c8c-281">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="58c8c-282">Если результирующий набор будет содержать больше одной страницы элементов, тело отклика будет содержать параметр `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-282">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="58c8c-283">Этот параметр содержит URL-адрес, с помощью которого можно получить следующую страницу результатов.</span><span class="sxs-lookup"><span data-stu-id="58c8c-283">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="58c8c-284">Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="58c8c-284">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="58c8c-285">Например, следующий запрос возвращает первые пять сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="58c8c-285">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="58c8c-286">[Попробовать в песочнице Graph][top-example]</span><span class="sxs-lookup"><span data-stu-id="58c8c-286">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="58c8c-287">Обработка ошибок параметров запроса</span><span class="sxs-lookup"><span data-stu-id="58c8c-287">Error handling for query parameters</span></span>

<span data-ttu-id="58c8c-p130">Некоторые запросы возвращают сообщение об ошибке, если указанный параметр запроса не поддерживается. Например, невозможно использовать `$expand` для связи `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="58c8c-p130">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="58c8c-290">При этом необходимо отметить, что указанные в запросе параметры могут просто не сработать.</span><span class="sxs-lookup"><span data-stu-id="58c8c-290">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="58c8c-291">Это может произойти, если не поддерживаются либо сами параметры, либо их сочетание.</span><span class="sxs-lookup"><span data-stu-id="58c8c-291">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="58c8c-292">В таких случаях необходимо проверить возвращенные запросом данные и определить, дали ли указанные параметры запроса желаемый результат.</span><span class="sxs-lookup"><span data-stu-id="58c8c-292">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0


