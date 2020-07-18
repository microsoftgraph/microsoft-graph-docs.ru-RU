---
title: Настройка ответов с помощью параметров запроса
description: В Microsoft Graph предусмотрены необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных.
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 3788478ff71ae103b912c5dd2a856c8fb85d23dc
ms.sourcegitcommit: 90aaba4e965945cb6550cf625cbc03287f39e531
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148517"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="58d0b-103">Настройка ответов с помощью параметров запроса</span><span class="sxs-lookup"><span data-stu-id="58d0b-103">Use query parameters to customize responses</span></span>

<span data-ttu-id="58d0b-104">В Microsoft Graph поддерживаются необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных.</span><span class="sxs-lookup"><span data-stu-id="58d0b-104">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="58d0b-105">Поддержка определенных параметров запросов варьируется для разных операций API и в зависимости от API может отличаться в конечных точках версии 1.0 и бета-версии.</span><span class="sxs-lookup"><span data-stu-id="58d0b-105">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span> 

> [!TIP] 
> <span data-ttu-id="58d0b-106">В конечной точке бета-версии префикс `$` является необязательным.</span><span class="sxs-lookup"><span data-stu-id="58d0b-106">On the beta endpoint, the `$` prefix is optional.</span></span> <span data-ttu-id="58d0b-107">Например, вместо `$filter` можно использовать `filter`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-107">For example, instead of `$filter`, you can use `filter`.</span></span> <span data-ttu-id="58d0b-108">В конечной точке версии 1 префикс `$` является необязательным только для подмножества API-интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-108">On the v1 endpoint, the `$` prefix is optional for only a subset of APIs.</span></span> <span data-ttu-id="58d0b-109">Для простоты всегда включайте `$`, если используется конечная точка версии 1.</span><span class="sxs-lookup"><span data-stu-id="58d0b-109">For simplicity, always include `$` if using the v1 endpoint.</span></span>

<span data-ttu-id="58d0b-110">Параметрами запроса могут быть системные параметры запроса OData или другие параметры запроса.</span><span class="sxs-lookup"><span data-stu-id="58d0b-110">Query parameters can be OData system query options or other query parameters.</span></span> 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a><span data-ttu-id="58d0b-111">Системные параметры запроса OData</span><span class="sxs-lookup"><span data-stu-id="58d0b-111">OData system query options</span></span>
<span data-ttu-id="58d0b-112">API Microsoft Graph может поддерживать один или несколько из указанных ниже системных параметров запроса OData.</span><span class="sxs-lookup"><span data-stu-id="58d0b-112">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="58d0b-113">Эти параметры запроса совместимы с [языком запросов OData версии 4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="58d0b-113">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="58d0b-114">**Примечание.** OData 4.0 поддерживает системные параметры запросов только в операциях GET.</span><span class="sxs-lookup"><span data-stu-id="58d0b-114">**Note:** OData 4.0 supports system query options in only GET operations.</span></span>

<span data-ttu-id="58d0b-115">Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="58d0b-115">Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="58d0b-116">Имя</span><span class="sxs-lookup"><span data-stu-id="58d0b-116">Name</span></span>                     | <span data-ttu-id="58d0b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="58d0b-117">Description</span></span> | <span data-ttu-id="58d0b-118">Пример</span><span class="sxs-lookup"><span data-stu-id="58d0b-118">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="58d0b-119">$count</span><span class="sxs-lookup"><span data-stu-id="58d0b-119">$count</span></span>](#count-parameter)         | <span data-ttu-id="58d0b-120">Возвращает общее количество соответствующих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-120">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="58d0b-121">$expand</span><span class="sxs-lookup"><span data-stu-id="58d0b-121">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="58d0b-122">Получает связанные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="58d0b-122">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="58d0b-123">$filter</span><span class="sxs-lookup"><span data-stu-id="58d0b-123">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="58d0b-124">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="58d0b-124">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="58d0b-125">$format</span><span class="sxs-lookup"><span data-stu-id="58d0b-125">$format</span></span>](#format-parameter)       | <span data-ttu-id="58d0b-126">Возвращает результаты в указанном формате мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="58d0b-126">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="58d0b-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="58d0b-127">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="58d0b-128">Упорядочивает результаты.</span><span class="sxs-lookup"><span data-stu-id="58d0b-128">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="58d0b-129">$search</span><span class="sxs-lookup"><span data-stu-id="58d0b-129">$search</span></span>](#search-parameter)       | <span data-ttu-id="58d0b-130">Возвращает результаты на основании условий поиска.</span><span class="sxs-lookup"><span data-stu-id="58d0b-130">Returns results based on search criteria.</span></span> |[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="58d0b-131">$select</span><span class="sxs-lookup"><span data-stu-id="58d0b-131">$select</span></span>](#select-parameter)       | <span data-ttu-id="58d0b-132">Фильтрует свойства (столбцы).</span><span class="sxs-lookup"><span data-stu-id="58d0b-132">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="58d0b-133">$skip</span><span class="sxs-lookup"><span data-stu-id="58d0b-133">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="58d0b-p104">Применяется для индексации в результирующем наборе. Также используется некоторыми API для разбиения по страницам и может использоваться вместе с параметром `$top` для разбиения результатов по страницам вручную.</span><span class="sxs-lookup"><span data-stu-id="58d0b-p104">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="58d0b-136">$top</span><span class="sxs-lookup"><span data-stu-id="58d0b-136">$top</span></span>](#top-parameter)             | <span data-ttu-id="58d0b-137">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-137">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="58d0b-138">Другие параметры запроса</span><span class="sxs-lookup"><span data-stu-id="58d0b-138">Other query parameters</span></span>

| <span data-ttu-id="58d0b-139">Имя</span><span class="sxs-lookup"><span data-stu-id="58d0b-139">Name</span></span>                     | <span data-ttu-id="58d0b-140">Описание</span><span class="sxs-lookup"><span data-stu-id="58d0b-140">Description</span></span> | <span data-ttu-id="58d0b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="58d0b-141">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="58d0b-142">$skipToken</span><span class="sxs-lookup"><span data-stu-id="58d0b-142">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="58d0b-p105">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц. (Вместо этого параметра некоторые API используют `$skip`.)</span><span class="sxs-lookup"><span data-stu-id="58d0b-p105">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a><span data-ttu-id="58d0b-145">Другие возможности URL-адресов OData</span><span class="sxs-lookup"><span data-stu-id="58d0b-145">Other OData URL capabilities</span></span>

<span data-ttu-id="58d0b-146">Следующие возможности OData 4.0 являются сегментами URL-адресов, а не параметрами запросов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-146">The following OData 4.0 capabilities are URL segments, not query parameters.</span></span>

| <span data-ttu-id="58d0b-147">Имя</span><span class="sxs-lookup"><span data-stu-id="58d0b-147">Name</span></span>                     | <span data-ttu-id="58d0b-148">Описание</span><span class="sxs-lookup"><span data-stu-id="58d0b-148">Description</span></span> | <span data-ttu-id="58d0b-149">Пример</span><span class="sxs-lookup"><span data-stu-id="58d0b-149">Example</span></span> 
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="58d0b-150">$ref</span><span class="sxs-lookup"><span data-stu-id="58d0b-150">$ref</span></span>](/graph/api/group-post-members?view=graph-rest-1.0&tabs=http) | <span data-ttu-id="58d0b-151">Обновляет принадлежность объектов к коллекции.</span><span class="sxs-lookup"><span data-stu-id="58d0b-151">Updates entities membership to a collection.</span></span> | `POST /groups/{id}/members/$ref` |
| [<span data-ttu-id="58d0b-152">$value</span><span class="sxs-lookup"><span data-stu-id="58d0b-152">$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="58d0b-153">Возвращает или обновляет двоичное значение элемента.</span><span class="sxs-lookup"><span data-stu-id="58d0b-153">Retrieves or updates the binary value of an item.</span></span> | `GET /me/photo/$value` |

## <a name="encoding-query-parameters"></a><span data-ttu-id="58d0b-154">Кодирование параметров запроса</span><span class="sxs-lookup"><span data-stu-id="58d0b-154">Encoding query parameters</span></span>

<span data-ttu-id="58d0b-155">К значениям параметров запросов нужно применить процентное кодирование.</span><span class="sxs-lookup"><span data-stu-id="58d0b-155">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="58d0b-156">Многие клиенты HTTP, браузеры и инструменты (например, [песочница Graph][graph-explorer]) помогут вам в этом.</span><span class="sxs-lookup"><span data-stu-id="58d0b-156">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="58d0b-157">Если запрос неудачный, одна из возможных причин — не удалось должным образом закодировать значения параметров запросов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-157">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="58d0b-158">URL-адрес, который не было закодирован, выглядит так:</span><span class="sxs-lookup"><span data-stu-id="58d0b-158">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="58d0b-159">Закодированный должным образом URL-адрес выглядит так:</span><span class="sxs-lookup"><span data-stu-id="58d0b-159">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

### <a name="escaping-single-quotes"></a><span data-ttu-id="58d0b-160">Пропуск одинарных кавычек</span><span class="sxs-lookup"><span data-stu-id="58d0b-160">Escaping single quotes</span></span>

<span data-ttu-id="58d0b-161">В запросах, использующих одинарные кавычки, если любой параметр также содержит одинарные кавычки, их нужно пропустить дважды; в противном случае запрос завершится сбоем из-за недопустимого синтаксиса.</span><span class="sxs-lookup"><span data-stu-id="58d0b-161">For requests that use single quotes, if any parameter values also contain single quotes, those must be double escaped; otherwise, the request will fail due to invalid syntax.</span></span> <span data-ttu-id="58d0b-162">В приведенном примере строковое значение `let''s meet for lunch?` содержит пропускаемую одинарную кавычку.</span><span class="sxs-lookup"><span data-stu-id="58d0b-162">In the example, the string value `let''s meet for lunch?` has the single quote escaped.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a><span data-ttu-id="58d0b-163">Параметр count</span><span class="sxs-lookup"><span data-stu-id="58d0b-163">count parameter</span></span>

<span data-ttu-id="58d0b-164">Параметр запроса `$count` позволяет включить общее количество элементов коллекции вместе со страницей значений, возвращенных из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58d0b-164">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="58d0b-165">Например, приведенный ниже запрос возвращает коллекцию **contact** текущего пользователя, а также ряд элементов коллекции **contact** в свойстве `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-165">For example, the following request returns both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="58d0b-166">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="58d0b-166">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


<span data-ttu-id="58d0b-167">Параметр запроса `$count` поддерживается для таких коллекций ресурсов и их отношений, которые являются производными от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="58d0b-167">The `$count` query parameter is supported for these collections of resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta):</span></span>
- [<span data-ttu-id="58d0b-168">application</span><span class="sxs-lookup"><span data-stu-id="58d0b-168">application</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-beta)
- [<span data-ttu-id="58d0b-169">orgContact</span><span class="sxs-lookup"><span data-stu-id="58d0b-169">orgContact</span></span>](https://docs.microsoft.com/graph/api/resources/orgcontact?view=graph-rest-beta)
- [<span data-ttu-id="58d0b-170">device</span><span class="sxs-lookup"><span data-stu-id="58d0b-170">device</span></span>](https://docs.microsoft.com/graph/api/resources/device?view=graph-rest-beta)
- [<span data-ttu-id="58d0b-171">group</span><span class="sxs-lookup"><span data-stu-id="58d0b-171">group</span></span>](https://docs.microsoft.com/graph/api/resources/group?view=graph-rest-beta)
- [<span data-ttu-id="58d0b-172">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="58d0b-172">servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-beta)
- <span data-ttu-id="58d0b-173">[users](https://docs.microsoft.com/graph/api/resources/user?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="58d0b-173">[users](https://docs.microsoft.com/graph/api/resources/user?view=graph-rest-beta).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="58d0b-174">Параметр expand</span><span class="sxs-lookup"><span data-stu-id="58d0b-174">expand parameter</span></span>

<span data-ttu-id="58d0b-175">Многие ресурсы Microsoft Graph возвращают как объявленные свойства ресурса, так и его связи с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="58d0b-175">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="58d0b-176">Эти связи также называются свойствами ссылки или навигации и могут ссылаться как на один ресурс, так и на коллекцию ресурсов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-176">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="58d0b-177">Например, папки почты, руководитель и подчиненные пользователя выводятся как связи.</span><span class="sxs-lookup"><span data-stu-id="58d0b-177">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="58d0b-p109">Как правило, в одном запросе можно отдельно (но не одновременно) запросить или свойства ресурса, или одно из отношений. С помощью строкового параметра запроса `$expand` в результаты можно включить расширенный ресурс или коллекцию, на которые ссылается одно отношение (свойство навигации).</span><span class="sxs-lookup"><span data-stu-id="58d0b-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="58d0b-180">В приведенном ниже примере возвращаются сведения о корневом каталоге, а также дочерние элементы верхнего уровня на диске.</span><span class="sxs-lookup"><span data-stu-id="58d0b-180">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="58d0b-181">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="58d0b-181">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="58d0b-p110">Кроме того, некоторые коллекции ресурсов позволяют указывать свойства, которые должны быть возвращены в расширенных ресурсах, благодаря параметру `$select`. В следующем примере выполняется тот же запрос, что и в предыдущем, но используется оператор [`$select`](#select-parameter), с помощью которого для расширенных дочерних элементов возвращаются только свойства **id** и **name**.</span><span class="sxs-lookup"><span data-stu-id="58d0b-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="58d0b-184">[Попробовать в песочнице Graph][expand-example]</span><span class="sxs-lookup"><span data-stu-id="58d0b-184">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="58d0b-p111">**Примечание.** Не все связи и ресурсы поддерживают параметр запроса `$expand`. Например, можно расширить связи пользователя **directReports**, **manager** и **memberOf**, но не связи **events**, **messages** или **photo**. Не все ресурсы и связи поддерживают использование параметра `$select` для расширенных элементов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="58d0b-188">Ресурсы Azure AD, производные от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), такие как [user](/graph/api/resources/user?view=graph-rest-1.0) и [group](/graph/api/resources/group?view=graph-rest-1.0), поддерживают параметр `$expand` только в `beta`, и обычно он возвращает не более 20 элементов расширенных отношений.</span><span class="sxs-lookup"><span data-stu-id="58d0b-188">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="58d0b-189">Параметр filter</span><span class="sxs-lookup"><span data-stu-id="58d0b-189">filter parameter</span></span>

<span data-ttu-id="58d0b-190">Параметр запроса `$filter` позволяет получить только подмножество объектов коллекции.</span><span class="sxs-lookup"><span data-stu-id="58d0b-190">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> <span data-ttu-id="58d0b-191">Параметр запроса `$filter` также используется для извлечения таких отношений, как members, memberOf, transitiveMembers и transitiveMemberOf.</span><span class="sxs-lookup"><span data-stu-id="58d0b-191">The `$filter` query parameter can also be used to retrieve relationships like members, memberOf, transitiveMembers, and transitiveMemberOf.</span></span> <span data-ttu-id="58d0b-192">Например, получите все группы безопасности, участником которых являетесь.</span><span class="sxs-lookup"><span data-stu-id="58d0b-192">For example, get all the security groups I'm a member of.</span></span>

<span data-ttu-id="58d0b-193">Также чтобы найти пользователей, чье отображаемое имя начинается с буквы J, используйте `startswith`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-193">The following example can be used to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="58d0b-194">[Попробовать в песочнице Graph][filter-example]</span><span class="sxs-lookup"><span data-stu-id="58d0b-194">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="58d0b-195">Поддержка операторов `$filter` зависит от того, какой API Microsoft Graph используется.</span><span class="sxs-lookup"><span data-stu-id="58d0b-195">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="58d0b-196">В большинстве случаев поддерживаются следующие операторы:</span><span class="sxs-lookup"><span data-stu-id="58d0b-196">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="58d0b-197">`eq` (равняется);</span><span class="sxs-lookup"><span data-stu-id="58d0b-197">equals (`eq`)</span></span>
- <span data-ttu-id="58d0b-198">`ne` (не равняется);</span><span class="sxs-lookup"><span data-stu-id="58d0b-198">not equals (`ne`)</span></span>
- <span data-ttu-id="58d0b-199">`gt` (больше чем);</span><span class="sxs-lookup"><span data-stu-id="58d0b-199">greater than (`gt`)</span></span>
- <span data-ttu-id="58d0b-200">`ge` (не меньше чем);</span><span class="sxs-lookup"><span data-stu-id="58d0b-200">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="58d0b-201">`lt` (меньше чем), `le` (не больше чем);</span><span class="sxs-lookup"><span data-stu-id="58d0b-201">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="58d0b-202">`and` (и);</span><span class="sxs-lookup"><span data-stu-id="58d0b-202">and (`and`)</span></span>
- <span data-ttu-id="58d0b-203">`or` (или);</span><span class="sxs-lookup"><span data-stu-id="58d0b-203">or (`or`)</span></span>
- <span data-ttu-id="58d0b-204">`not` (не).</span><span class="sxs-lookup"><span data-stu-id="58d0b-204">not (`not`)</span></span>
 
<span data-ttu-id="58d0b-205">Часто поддерживается строковый оператор `startswith`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-205">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="58d0b-206">Некоторые API поддерживают лямбда-оператор `any`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-206">The `any` lambda operator is supported for some APIs.</span></span> 

> <span data-ttu-id="58d0b-207">**Примечание.** При одновременном использовании `$filter` и `$orderby` в одном запросе [задайте свойства определенным образом](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query), чтобы получать сообщения.  </span><span class="sxs-lookup"><span data-stu-id="58d0b-207">**Note:** You must [specify properties in certain ways](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query) when using both `$filter` and `$orderby` in the same query to get messages.</span></span>

<span data-ttu-id="58d0b-208">Примеры использования см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="58d0b-208">For some usage examples, see the following table.</span></span> <span data-ttu-id="58d0b-209">Дополнительные сведения о синтаксисе `$filter` см. в [статье о протоколе OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="58d0b-209">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="58d0b-210">Приведенная ниже таблица содержит несколько примеров использования параметра запроса `$filter`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-210">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="58d0b-211">**Примечание.** Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="58d0b-211">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="58d0b-212">Описание</span><span class="sxs-lookup"><span data-stu-id="58d0b-212">Description</span></span> | <span data-ttu-id="58d0b-213">Пример</span><span class="sxs-lookup"><span data-stu-id="58d0b-213">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="58d0b-214">Поиск пользователей с именем Mary по нескольким свойствам.</span><span class="sxs-lookup"><span data-stu-id="58d0b-214">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| <span data-ttu-id="58d0b-215">Получение всех событий для вошедшего пользователя, которые начинаются после 01.07.2017 г.</span><span class="sxs-lookup"><span data-stu-id="58d0b-215">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| <span data-ttu-id="58d0b-216">Получение всех сообщений с определенного адреса, полученных вошедшим пользователем.</span><span class="sxs-lookup"><span data-stu-id="58d0b-216">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| <span data-ttu-id="58d0b-217">Получение всех сообщений, полученных вошедшим пользователем в апреле 2017 г.</span><span class="sxs-lookup"><span data-stu-id="58d0b-217">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| <span data-ttu-id="58d0b-218">Получение всех непрочитанных сообщений в папке "Входящие" вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="58d0b-218">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| <span data-ttu-id="58d0b-219">Получение списка всех групп Microsoft 365 в организации.</span><span class="sxs-lookup"><span data-stu-id="58d0b-219">List all Microsoft 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |
| <span data-ttu-id="58d0b-220">Используйте преобразование OData, чтобы получить транзитивное членство в группах с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-220">Use OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects.</span></span> | [`https://graph.microsoft.com/beta/me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`](https://developer.microsoft.com/graph/graph-explorer?request=me/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName,'a')&method=GET&version=v1.0) |

> <span data-ttu-id="58d0b-p116">**Примечание.** Ресурсы Azure AD не поддерживают следующие операторы `$filter`: `ne`, `gt`, `ge`, `lt`, `le` и `not`. В настоящее время строковый оператор `contains` не поддерживается ни одним ресурсом Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58d0b-p116">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="58d0b-223">Параметр format</span><span class="sxs-lookup"><span data-stu-id="58d0b-223">format parameter</span></span>

<span data-ttu-id="58d0b-224">Параметр запроса `$format` позволяет указать формат мультимедиа для элементов, возвращаемых из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58d0b-224">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="58d0b-225">Например, указанный ниже запрос возвращает список пользователей организации в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58d0b-225">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="58d0b-226">[Попробовать в песочнице Graph][format-example]</span><span class="sxs-lookup"><span data-stu-id="58d0b-226">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="58d0b-227">**Примечание.** Параметр запросов `$format` поддерживает ряд форматов (например, Atom, XML и JSON), но результаты могут не возвращаться во всех форматах.</span><span class="sxs-lookup"><span data-stu-id="58d0b-227">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="58d0b-228">Параметр orderby</span><span class="sxs-lookup"><span data-stu-id="58d0b-228">orderby parameter</span></span>

<span data-ttu-id="58d0b-229">Параметр запроса `$orderby` позволяет указать порядок сортировки элементов, возвращаемых из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58d0b-229">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="58d0b-230">Например, следующий запрос возвращает список пользователей в организации, упорядоченный по отображаемому имени:</span><span class="sxs-lookup"><span data-stu-id="58d0b-230">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="58d0b-231">[Попробовать в песочнице Graph][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="58d0b-231">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="58d0b-p117">Вы также можете сортировать данные по объектам сложного типа. Приведенный ниже запрос позволяет получить сообщения и отсортировать их по полю **address** свойства **from**, принадлежащего к сложному типу **emailAddress**.</span><span class="sxs-lookup"><span data-stu-id="58d0b-p117">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="58d0b-234">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="58d0b-234">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="58d0b-235">Чтобы отсортировать результаты по возрастанию или убыванию, добавьте `asc` или `desc` к имени поля, используя пробел для разделения, например: `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-235">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="58d0b-236">Некоторые API позволяют упорядочивать результаты по нескольким свойствам.</span><span class="sxs-lookup"><span data-stu-id="58d0b-236">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="58d0b-237">Например, приведенный ниже запрос позволяет упорядочить сообщения в папке "Входящие" пользователя сначала по имени отправителей по убыванию (от Я до А), а затем — по возрастанию (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="58d0b-237">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="58d0b-238">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="58d0b-238">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

> <span data-ttu-id="58d0b-239">**Примечание.** Если вы укажете $filter, сервер определит порядок сортировки результатов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-239">**Note:** When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="58d0b-240">Если вы одновременно используете `$orderby` и `$filter` для получения сообщений, так как сервер всегда определяет порядок сортировки результатов `$filter`, [необходимо задать свойства определенным образом](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query).</span><span class="sxs-lookup"><span data-stu-id="58d0b-240">If you use both `$orderby` and `$filter` to get messages, because the server always infers a sort order for the results of a `$filter`, you must [specify properties in certain ways](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query).</span></span>


<span data-ttu-id="58d0b-241">В приведенном ниже примере показан запрос, отфильтрованный по свойствам **subject** и **importance**, а затем отсортированный по свойствам **subject**, **importance** и **receivedDateTime** в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="58d0b-241">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="58d0b-242">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="58d0b-242">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="58d0b-243">**Примечание.** Ресурсы Azure AD, производные от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), такие как [user](/graph/api/resources/user?view=graph-rest-1.0) и [group](/graph/api/resources/group?view=graph-rest-1.0), не позволяют объединять параметр `$orderby` с выражениями `$filter`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-243">**Note:** With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="58d0b-244">Параметр search</span><span class="sxs-lookup"><span data-stu-id="58d0b-244">search parameter</span></span>

<span data-ttu-id="58d0b-245">Параметр запроса `$search` позволяет ограничить результаты запроса с помощью условия поиска.</span><span class="sxs-lookup"><span data-stu-id="58d0b-245">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="58d0b-246">Использование параметра $search в коллекциях message</span><span class="sxs-lookup"><span data-stu-id="58d0b-246">Using $search on message collections</span></span>

<span data-ttu-id="58d0b-247">Можно искать сообщения, основываясь на их конкретных свойствах.</span><span class="sxs-lookup"><span data-stu-id="58d0b-247">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="58d0b-248">Результаты поиска сортируются по дате и времени отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="58d0b-248">The results of the search are sorted by the date and time that the message was sent.</span></span> <span data-ttu-id="58d0b-249">Запрос `$search` возвращает до 250 результатов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-249">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="58d0b-250">Если при поиске сообщений указано только значение, а конкретные свойства не заданы, поиск выполняется по свойствам поиска по умолчанию: **from**, **subject** и **body**.</span><span class="sxs-lookup"><span data-stu-id="58d0b-250">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="58d0b-251">Следующий пример кода возвращает все сообщения из папки "Входящие" вошедшего пользователя, содержащие слово "pizza" в любом из трех свойств поиска по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="58d0b-251">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="58d0b-252">[Попробовать в песочнице Graph][search-example]</span><span class="sxs-lookup"><span data-stu-id="58d0b-252">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="58d0b-253">Кроме того, для поиска сообщений можно указать в таблице ниже их имена свойств, распознаваемые синтаксисом языка запросов по ключевым словам (KQL).</span><span class="sxs-lookup"><span data-stu-id="58d0b-253">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="58d0b-254">Эти имена свойств соответствуют свойствам, определенным в сущности **message** в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58d0b-254">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="58d0b-255">Синтаксис KQL поддерживается в Outlook и других приложениях Microsoft 365, например SharePoint. Благодаря этому возможно использование общего домена обнаружения для соответствующих хранилищ данных.</span><span class="sxs-lookup"><span data-stu-id="58d0b-255">Outlook and other Microsoft 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="58d0b-256">Свойство электронных писем, по которому можно выполнять поиск</span><span class="sxs-lookup"><span data-stu-id="58d0b-256">Searchable email property</span></span>                | <span data-ttu-id="58d0b-257">Описание</span><span class="sxs-lookup"><span data-stu-id="58d0b-257">Description</span></span> | <span data-ttu-id="58d0b-258">Пример</span><span class="sxs-lookup"><span data-stu-id="58d0b-258">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="58d0b-259">**attachment**</span><span class="sxs-lookup"><span data-stu-id="58d0b-259">**attachment**</span></span>           | <span data-ttu-id="58d0b-260">Имена файлов, вложенных в сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58d0b-260">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="58d0b-261">**bcc**</span><span class="sxs-lookup"><span data-stu-id="58d0b-261">**bcc**</span></span>           | <span data-ttu-id="58d0b-262">Поле **Скрытая копия** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="58d0b-262">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="58d0b-263">**body**</span><span class="sxs-lookup"><span data-stu-id="58d0b-263">**body**</span></span>           | <span data-ttu-id="58d0b-264">Текст сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58d0b-264">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="58d0b-265">**cc**</span><span class="sxs-lookup"><span data-stu-id="58d0b-265">**cc**</span></span>           | <span data-ttu-id="58d0b-266">Поле **Копия** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="58d0b-266">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="58d0b-267">**from**</span><span class="sxs-lookup"><span data-stu-id="58d0b-267">**from**</span></span>           | <span data-ttu-id="58d0b-268">Отправитель сообщения электронной почты, на которого указывает SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="58d0b-268">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="58d0b-269">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="58d0b-269">**hasAttachment**</span></span> | <span data-ttu-id="58d0b-270">Значение TRUE означает, что сообщение электронной почты содержит вложение, не являющееся встроенным. В противном случае задается значение FALSE.</span><span class="sxs-lookup"><span data-stu-id="58d0b-270">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| <span data-ttu-id="58d0b-271">**importance**</span><span class="sxs-lookup"><span data-stu-id="58d0b-271">**importance**</span></span>           | <span data-ttu-id="58d0b-272">Важность сообщения, которую отправитель может указать при отправке.</span><span class="sxs-lookup"><span data-stu-id="58d0b-272">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="58d0b-273">Возможные значения — `low`, `medium` и `high`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-273">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="58d0b-274">**kind**</span><span class="sxs-lookup"><span data-stu-id="58d0b-274">**kind**</span></span>           | <span data-ttu-id="58d0b-275">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="58d0b-275">The type of message.</span></span> <span data-ttu-id="58d0b-276">Допустимые значения — `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` и `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-276">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="58d0b-277">**participants**</span><span class="sxs-lookup"><span data-stu-id="58d0b-277">**participants**</span></span>           | <span data-ttu-id="58d0b-278">Такие поля сообщения электронной почты, как **От**, **Кому**, **Копия** и **Скрытая копия**, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="58d0b-278">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="58d0b-279">**received**</span><span class="sxs-lookup"><span data-stu-id="58d0b-279">**received**</span></span>           | <span data-ttu-id="58d0b-280">Дата получения сообщения адресатом.</span><span class="sxs-lookup"><span data-stu-id="58d0b-280">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="58d0b-281">**recipients**</span><span class="sxs-lookup"><span data-stu-id="58d0b-281">**recipients**</span></span>           | <span data-ttu-id="58d0b-282">Такие поля сообщения электронной почты, как **Кому**, **Копия** и **Скрытая копия**, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="58d0b-282">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="58d0b-283">**sent**</span><span class="sxs-lookup"><span data-stu-id="58d0b-283">**sent**</span></span>           | <span data-ttu-id="58d0b-284">Дата отправки сообщения отправителем.</span><span class="sxs-lookup"><span data-stu-id="58d0b-284">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="58d0b-285">**size**</span><span class="sxs-lookup"><span data-stu-id="58d0b-285">**size**</span></span>           | <span data-ttu-id="58d0b-286">Размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="58d0b-286">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="58d0b-287">**subject**</span><span class="sxs-lookup"><span data-stu-id="58d0b-287">**subject**</span></span>           | <span data-ttu-id="58d0b-288">Текст в строке темы сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58d0b-288">The text in the subject line of an email message.</span></span> <span data-ttu-id="58d0b-289">.</span><span class="sxs-lookup"><span data-stu-id="58d0b-289">.</span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="58d0b-290">**to**</span><span class="sxs-lookup"><span data-stu-id="58d0b-290">**to**</span></span>           | <span data-ttu-id="58d0b-291">Поле **Кому** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="58d0b-291">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="58d0b-292">Дополнительные сведения о доступных для поиска свойствах, синтаксисе KQL, поддерживаемых операторах и подсказках для поиска вы найдете в таких статьях:</span><span class="sxs-lookup"><span data-stu-id="58d0b-292">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="58d0b-293">[Свойства, доступные для поиска в Exchange](https://docs.microsoft.com/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)</span><span class="sxs-lookup"><span data-stu-id="58d0b-293">[Searchable properties in Exchange](https://docs.microsoft.com/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="58d0b-294">Руководство по синтаксису языка запросов по ключевым словам (KQL)</span><span class="sxs-lookup"><span data-stu-id="58d0b-294">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="58d0b-295">[Свойства сообщений и операторы поиска для обнаружения электронных данных на месте в Exchange 2016](https://technet.microsoft.com/library/dn774955(v=exchg.160).aspx).</span><span class="sxs-lookup"><span data-stu-id="58d0b-295">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="58d0b-296">Использование параметра $search в коллекциях person</span><span class="sxs-lookup"><span data-stu-id="58d0b-296">Using $search on person collections</span></span>

<span data-ttu-id="58d0b-297">API People Microsoft Graph можно использовать для получения сведений о наиболее релевантных для пользователя людях.</span><span class="sxs-lookup"><span data-stu-id="58d0b-297">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="58d0b-298">Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями.</span><span class="sxs-lookup"><span data-stu-id="58d0b-298">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="58d0b-299">API People поддерживает параметр запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-299">The People API supports the `$search` query parameter.</span></span> <span data-ttu-id="58d0b-300">Запрос `$search` возвращает до 250 результатов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-300">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="58d0b-301">Поиск людей выполняется по свойствам **displayName** и **emailAddress** ресурса [person](/graph/api/resources/person?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="58d0b-301">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person?view=graph-rest-1.0) resource.</span></span>

<span data-ttu-id="58d0b-302">По приведенному ниже запросу выполняется поиск человека с именем Irene McGowen в свойствах **displayName** и **emailAddress** всех людей из коллекции **people** вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="58d0b-302">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="58d0b-303">Так как человек с именем Irene McGowan является релевантным для вошедшего пользователя, возвращается информация о нем.</span><span class="sxs-lookup"><span data-stu-id="58d0b-303">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="58d0b-304">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="58d0b-304">The following example shows the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

<span data-ttu-id="58d0b-305">Дополнительные сведения об API поиска людей см. в [этой статье](./people-example.md#search-people).</span><span class="sxs-lookup"><span data-stu-id="58d0b-305">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

### <a name="using-search-on-directory-object-collections"></a><span data-ttu-id="58d0b-306">Использование $search в коллекциях объектов каталога</span><span class="sxs-lookup"><span data-stu-id="58d0b-306">Using $search on directory object collections</span></span>

<span data-ttu-id="58d0b-307">Параметр запроса `$search` позволяет ограничить результаты на основе критерия поиска, например поиска слов в строках, разделенных пробелами, регистром и типами символов (числами и специальными символами).</span><span class="sxs-lookup"><span data-stu-id="58d0b-307">You can use the `$search` query parameter to restrict results based on a search criterion such as looking for words in strings delimited by spaces, casing, and character types (numbers and special characters).</span></span> <span data-ttu-id="58d0b-308">Поддержка поиска по маркерам работает только в полях "displayName" и "description".</span><span class="sxs-lookup"><span data-stu-id="58d0b-308">The tokenized search support works only on the displayName and description fields.</span></span> <span data-ttu-id="58d0b-309">Любое поле можно поместить в `$search`, поля, отличные от **displayName** и **description** по умолчанию представляют собой поведение `$filter`"startswith".</span><span class="sxs-lookup"><span data-stu-id="58d0b-309">Any field can be put in `$search`, fields other than **displayName** and **description** defaults to `$filter` startswith behavior.</span></span> <span data-ttu-id="58d0b-310">Пример:</span><span class="sxs-lookup"><span data-stu-id="58d0b-310">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`
 
<span data-ttu-id="58d0b-311">В результате будут выводиться все группы с именами типа "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="58d0b-311">This looks for all groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="58d0b-312">`$search` можно использовать вместе с `$filter`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-312">`$search` can be used together with `$filter` as well.</span></span> <span data-ttu-id="58d0b-313">Пример:</span><span class="sxs-lookup"><span data-stu-id="58d0b-313">For example:</span></span> 
 
`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"` 
 
<span data-ttu-id="58d0b-314">В результате будут выводиться все группы с включенной поддержкой почты с именами типа "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="58d0b-314">This looks for all mail-enabled groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="58d0b-315">Результаты ограничены на основе логического соединения `$filter` ("И") и всего запроса в `$search`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-315">The results are restricted based on a logical conjunction (an "AND") of the `$filter` and the entire query in the `$search`.</span></span> <span data-ttu-id="58d0b-316">Искомый текст маркируется с учетом регистра, но совпадения выполняются без его учета.</span><span class="sxs-lookup"><span data-stu-id="58d0b-316">The search text is tokenized based on casing, but matches are performed in a case-insensitive manner.</span></span> <span data-ttu-id="58d0b-317">Например, "OneVideo" разбивается на два маркера ввода "one" и "video", но не учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="58d0b-317">For example, "OneVideo" would be split into two input tokens "one" and "video", but matches properties in insensitive to case.</span></span> 
 
 
<span data-ttu-id="58d0b-318">В синтаксисе поиска применяются следующие правила:</span><span class="sxs-lookup"><span data-stu-id="58d0b-318">The syntax of search follows these rules:</span></span> 
 
- <span data-ttu-id="58d0b-319">Универсальный формат: $search = "clause1" [И | ИЛИ] "[clauseX]".</span><span class="sxs-lookup"><span data-stu-id="58d0b-319">Generic format: $search="clause1" [AND | OR]  "[clauseX]".</span></span> 
- <span data-ttu-id="58d0b-320">Поддерживается любое количество предложений.</span><span class="sxs-lookup"><span data-stu-id="58d0b-320">Any number of clauses is supported.</span></span> <span data-ttu-id="58d0b-321">Также поддерживаются круглые скобки для приоритета.</span><span class="sxs-lookup"><span data-stu-id="58d0b-321">Parentheses for precedence is also supported.</span></span> 
- <span data-ttu-id="58d0b-322">Синтаксис каждого предложения — <property>:<text to search>.</span><span class="sxs-lookup"><span data-stu-id="58d0b-322">The syntax for each clause is <property>:<text to search>.</span></span> 
- <span data-ttu-id="58d0b-323">Имя свойства должно быть указано в предложении.</span><span class="sxs-lookup"><span data-stu-id="58d0b-323">The property name must be specified in clause.</span></span> <span data-ttu-id="58d0b-324">Любое свойство, которое можно использовать в `$filter`, можно также использовать в `$search`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-324">Any property that can be used in `$filter` can also be used inside `$search`.</span></span> <span data-ttu-id="58d0b-325">В зависимости от свойства поведение поиска является либо "search", либо "startswith", если поиск не поддерживается в свойстве.</span><span class="sxs-lookup"><span data-stu-id="58d0b-325">Depending on the property, the search behavior is either "search" or "startswith" if search is not supported on the property.</span></span> 
- <span data-ttu-id="58d0b-326">Вся часть предложения должна быть заключена в двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="58d0b-326">The whole clause part must be put inside double quotes.</span></span>  
- <span data-ttu-id="58d0b-327">Логический оператор "И" "ИЛИ" не должен быть в двойных кавычках.</span><span class="sxs-lookup"><span data-stu-id="58d0b-327">Logical operator 'AND' 'OR' must be put outside double quotes.</span></span> <span data-ttu-id="58d0b-328">Они должны быть прописными.</span><span class="sxs-lookup"><span data-stu-id="58d0b-328">They must be in upper case.</span></span> 
- <span data-ttu-id="58d0b-329">Учитывая, что вся часть предложения должна быть помещена в двойные кавычки, если <text to search> содержит двойные кавычки и обратную косую черту, ее необходимо пропустить до обратной косой черты.</span><span class="sxs-lookup"><span data-stu-id="58d0b-329">Given that the whole clause part needs to be put inside double quotes, if <text to search> contains double quote and backslash, it needs to be escaped by backslash.</span></span> <span data-ttu-id="58d0b-330">Другие символы не требуются пропускать.</span><span class="sxs-lookup"><span data-stu-id="58d0b-330">No other characters need to be escaped.</span></span> 

<span data-ttu-id="58d0b-331">В таблице ниже приведены некоторые примеры.</span><span class="sxs-lookup"><span data-stu-id="58d0b-331">The table below shows some examples.</span></span> 
 

| <span data-ttu-id="58d0b-332">Класс объекта</span><span class="sxs-lookup"><span data-stu-id="58d0b-332">Object class</span></span> | <span data-ttu-id="58d0b-333">Описание</span><span class="sxs-lookup"><span data-stu-id="58d0b-333">Description</span></span> | <span data-ttu-id="58d0b-334">Пример</span><span class="sxs-lookup"><span data-stu-id="58d0b-334">Example</span></span> |
| ------------ | ----------- | ------- |
| <span data-ttu-id="58d0b-335">Пользователь</span><span class="sxs-lookup"><span data-stu-id="58d0b-335">User</span></span> | <span data-ttu-id="58d0b-336">Отображаемое имя пользователя из адресной книги.</span><span class="sxs-lookup"><span data-stu-id="58d0b-336">Address book display name of the user.</span></span> |  `https://graph.microsoft.com/beta/users?$search="displayName:Guthr"` |
| <span data-ttu-id="58d0b-337">Пользователь</span><span class="sxs-lookup"><span data-stu-id="58d0b-337">User</span></span> | <span data-ttu-id="58d0b-338">Отображаемое имя пользователя или электронная почта из адресной книги.</span><span class="sxs-lookup"><span data-stu-id="58d0b-338">Address book display name or mail of the user.</span></span> | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"` |
| <span data-ttu-id="58d0b-339">Группа</span><span class="sxs-lookup"><span data-stu-id="58d0b-339">Group</span></span> | <span data-ttu-id="58d0b-340">Отображаемое имя пользователя или описание из адресной книги.</span><span class="sxs-lookup"><span data-stu-id="58d0b-340">Address book display name or description of the group.</span></span> | `https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")` |
| <span data-ttu-id="58d0b-341">Группа</span><span class="sxs-lookup"><span data-stu-id="58d0b-341">Group</span></span> | <span data-ttu-id="58d0b-342">Отображаемое имя пользователя или группа с доступом к почте из адресной книги.</span><span class="sxs-lookup"><span data-stu-id="58d0b-342">Address book display name on a mail enabled group.</span></span> | `https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"` |

<span data-ttu-id="58d0b-343">Строки ввода, указанные в `$search`, а также указанные выше свойства для поиска, разделяются на части с помощью пробелов, различных регистров и типов символов (чисел и специальных символов).</span><span class="sxs-lookup"><span data-stu-id="58d0b-343">Both the string inputs you provide in `$search`, as well as the searchable properties indicated above, are split up into parts by spaces, different casing, and character types (numbers and special characters).</span></span>

## <a name="select-parameter"></a><span data-ttu-id="58d0b-344">Параметр select</span><span class="sxs-lookup"><span data-stu-id="58d0b-344">select parameter</span></span>

<span data-ttu-id="58d0b-345">Параметр запроса `$select` позволяет возвратить набор свойств, отличный от набора по умолчанию, для отдельного ресурса или коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-345">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="58d0b-346">С помощью параметра $select можно указать подмножество или супермножество свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58d0b-346">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="58d0b-347">Например, при получении сообщений вошедшего пользователя можно указать, что необходимо вернуть только свойства **from** и **subject**:</span><span class="sxs-lookup"><span data-stu-id="58d0b-347">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="58d0b-348">[Попробовать в песочнице Graph][select-example]</span><span class="sxs-lookup"><span data-stu-id="58d0b-348">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="58d0b-349">**Важно!** Как правило, параметр `$select` рекомендуется использовать, чтобы запрос возвращал только те свойства, которые необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="58d0b-349">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="58d0b-350">Это особенно касается запросов, которые могут возвращать большой результирующий набор.</span><span class="sxs-lookup"><span data-stu-id="58d0b-350">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="58d0b-351">Ограничение набора свойств, возвращаемых в каждой строке, позволяет уменьшить сетевую нагрузку и повысить производительность вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="58d0b-351">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="58d0b-p136">В `v1.0` некоторые ресурсы Azure AD, производные от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), такие как [user](/graph/api/resources/user?view=graph-rest-1.0) и [group](/graph/api/resources/group?view=graph-rest-1.0), возвращают при чтении ограниченное подмножество свойств по умолчанию. С этими ресурсами параметр `$select` необходимо использовать для возврата свойств, не входящих в набор по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58d0b-p136">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="58d0b-354">Параметр skip</span><span class="sxs-lookup"><span data-stu-id="58d0b-354">skip parameter</span></span>

<span data-ttu-id="58d0b-p137">Параметр запроса `$skip` позволяет задать количество элементов, которое необходимо пропустить в начале коллекции. Например, следующий запрос возвращает события пользователя, отсортированные по дате создания, начиная с 21-го события в коллекции:</span><span class="sxs-lookup"><span data-stu-id="58d0b-p137">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="58d0b-357">[Попробовать в песочнице Graph][skip-example]</span><span class="sxs-lookup"><span data-stu-id="58d0b-357">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="58d0b-358">**Примечание.** Некоторые API Microsoft Graph, например для почты и календарей Outlook (**message**, **event** и **calendar**), используют `$skip` для разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="58d0b-358">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="58d0b-359">Если результаты запроса занимают несколько страниц, эти API возвращают свойство `@odata:nextLink` с URL-адресом, содержащим параметр `$skip`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-359">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="58d0b-360">Этот URL-адрес можно использовать для возврата следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-360">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="58d0b-361">[Подробнее…](./paging.md)</span><span class="sxs-lookup"><span data-stu-id="58d0b-361">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="58d0b-362">Параметр skipToken</span><span class="sxs-lookup"><span data-stu-id="58d0b-362">skipToken parameter</span></span>

<span data-ttu-id="58d0b-p139">Некоторые запросы возвращают несколько страниц данных. Это происходит из-за разбиения по страницам на стороне сервера или из-за использования параметра [`$top`](#top-parameter), который ограничивает размер возвращаемых страниц. Многие API Microsoft Graph используют параметр запроса `skipToken` для ссылки на следующие страницы результатов. Параметр `$skiptoken` содержит непрозрачный маркер, который ссылается на следующую страницу результатов и возвращается в URL-адресе, указанном в свойстве `@odata.nextLink`. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="58d0b-p139">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="58d0b-367">Параметр top</span><span class="sxs-lookup"><span data-stu-id="58d0b-367">top parameter</span></span>

<span data-ttu-id="58d0b-368">Параметр запроса `$top` позволяет задать размер страницы в результирующем наборе.</span><span class="sxs-lookup"><span data-stu-id="58d0b-368">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="58d0b-369">Если результирующий набор будет содержать больше одной страницы элементов, тело отклика будет содержать параметр `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-369">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="58d0b-370">Этот параметр содержит URL-адрес, с помощью которого можно получить следующую страницу результатов.</span><span class="sxs-lookup"><span data-stu-id="58d0b-370">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="58d0b-371">Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="58d0b-371">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="58d0b-372">Параметр $top принимает минимальное значение 1 и максимальное значение 999 (включительно).</span><span class="sxs-lookup"><span data-stu-id="58d0b-372">$top accepts a minimum value of 1 and a maximum value of 999 (inclusive).</span></span>  

<span data-ttu-id="58d0b-373">Например, следующий запрос возвращает первые пять сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="58d0b-373">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="58d0b-374">[Попробовать в песочнице Graph][top-example]</span><span class="sxs-lookup"><span data-stu-id="58d0b-374">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="58d0b-375">Обработка ошибок параметров запроса</span><span class="sxs-lookup"><span data-stu-id="58d0b-375">Error handling for query parameters</span></span>

<span data-ttu-id="58d0b-p141">Некоторые запросы возвращают сообщение об ошибке, если указанный параметр запроса не поддерживается. Например, невозможно использовать `$expand` для связи `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="58d0b-p141">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="58d0b-378">При этом необходимо отметить, что указанные в запросе параметры могут просто не сработать.</span><span class="sxs-lookup"><span data-stu-id="58d0b-378">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="58d0b-379">Это может произойти, если не поддерживаются либо сами параметры, либо их сочетание.</span><span class="sxs-lookup"><span data-stu-id="58d0b-379">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="58d0b-380">В таких случаях необходимо проверить возвращенные запросом данные и определить, дали ли указанные параметры запроса желаемый результат.</span><span class="sxs-lookup"><span data-stu-id="58d0b-380">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups?$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0



## <a name="see-also"></a><span data-ttu-id="58d0b-381">См. также</span><span class="sxs-lookup"><span data-stu-id="58d0b-381">See also</span></span>

- [<span data-ttu-id="58d0b-382">Ограничения параметров запроса</span><span class="sxs-lookup"><span data-stu-id="58d0b-382">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)
