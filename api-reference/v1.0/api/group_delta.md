# <a name="group-delta"></a><span data-ttu-id="998c4-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="998c4-101">group: delta</span></span>
<span data-ttu-id="998c4-p101">[Запросы изменений](../../../concepts/delta_query_overview.md) позволяют приложениям обнаруживать новые, обновленные и удаленные сущности, не считывая целевой ресурс полностью при каждом запросе. Чтобы узнать об изменениях в группах, выполните запрос с помощью функции *delta*. Подробные сведения вы найдете [здесь](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="998c4-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to groups, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="998c4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="998c4-105">Permissions</span></span>
<span data-ttu-id="998c4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="998c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="998c4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="998c4-108">Permission type</span></span>      | <span data-ttu-id="998c4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="998c4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="998c4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="998c4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="998c4-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="998c4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="998c4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="998c4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="998c4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="998c4-113">Not supported.</span></span>    |
|<span data-ttu-id="998c4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="998c4-114">Application</span></span> | <span data-ttu-id="998c4-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="998c4-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="998c4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="998c4-116">HTTP request</span></span>
<span data-ttu-id="998c4-117">Чтобы начать отслеживать изменения, выполните запрос к ресурсу groups, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="998c4-117">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a><span data-ttu-id="998c4-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="998c4-118">Query parameters</span></span>
<span data-ttu-id="998c4-p103">Отслеживание изменений в группах запускает один или более циклов вызовов **разностной** функции. Если вы используете какой-либо параметр запроса (кроме `$deltatoken` и `$skiptoken`), вам необходимо указать его в исходном **разностном** запросе. Microsoft Graph автоматически кодирует любые указанные параметры в той части предоставленного в ответе URL-адреса `nextLink` или `deltaLink`, которая содержит токен.</span><span class="sxs-lookup"><span data-stu-id="998c4-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="998c4-122">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="998c4-122">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="998c4-123">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="998c4-123">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="998c4-124">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="998c4-124">Query parameter</span></span>      | <span data-ttu-id="998c4-125">Тип</span><span class="sxs-lookup"><span data-stu-id="998c4-125">Type</span></span>   |<span data-ttu-id="998c4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="998c4-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="998c4-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="998c4-127">$deltatoken</span></span> | <span data-ttu-id="998c4-128">string</span><span class="sxs-lookup"><span data-stu-id="998c4-128">string</span></span> | <span data-ttu-id="998c4-p104">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции групп и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="998c4-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="998c4-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="998c4-131">$skiptoken</span></span> | <span data-ttu-id="998c4-132">строка</span><span class="sxs-lookup"><span data-stu-id="998c4-132">string</span></span> | <span data-ttu-id="998c4-133">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции групп получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="998c4-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="998c4-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="998c4-134">Optional query parameters</span></span>
<span data-ttu-id="998c4-135">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="998c4-135">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="998c4-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="998c4-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="998c4-138">Запросы изменений поддерживают параметры `$select`, `$top` и `$expand` для групп.</span><span class="sxs-lookup"><span data-stu-id="998c4-138">Delta query support `$select`, `$top`, and `$expand` for groups.</span></span> 
- <span data-ttu-id="998c4-139">Имеется ограниченная поддержка параметров `$filter` и `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="998c4-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="998c4-140">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="998c4-140">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="998c4-141">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="998c4-141">You can filter multiple objects.</span></span> <span data-ttu-id="998c4-142">Например, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`.</span><span class="sxs-lookup"><span data-stu-id="998c4-142">For example: `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`.</span></span> <span data-ttu-id="998c4-143">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="998c4-143">There is a limit of 50 filtered objects.</span></span>
- <span data-ttu-id="998c4-144">Параметр `$search` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="998c4-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="998c4-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="998c4-145">Request headers</span></span>
| <span data-ttu-id="998c4-146">Имя</span><span class="sxs-lookup"><span data-stu-id="998c4-146">Name</span></span>       | <span data-ttu-id="998c4-147">Описание</span><span class="sxs-lookup"><span data-stu-id="998c4-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="998c4-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="998c4-148">Authorization</span></span>  | <span data-ttu-id="998c4-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="998c4-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="998c4-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="998c4-150">Content-Type</span></span>  | <span data-ttu-id="998c4-151">application/json</span><span class="sxs-lookup"><span data-stu-id="998c4-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="998c4-152">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="998c4-152">Request body</span></span>
<span data-ttu-id="998c4-153">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="998c4-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="998c4-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="998c4-154">Response</span></span>
<span data-ttu-id="998c4-p107">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект коллекции [group](../resources/group.md) в тексте ответа. Ответ также включает токен состояния — URL-адрес nextLink или deltaLink.</span><span class="sxs-lookup"><span data-stu-id="998c4-p107">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body. The response also includes a state token which is either a nextLink URL or a deltaLink URL.</span></span>

- <span data-ttu-id="998c4-p108">Если возвращается URL-адрес nextLink, это означает, что во время сеанса получены не все страницы данных. Приложение продолжает отправлять запросы, используя URL-адрес nextLink, пока в ответ не будет включен URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="998c4-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="998c4-p109">Если возвращается URL-адрес deltaLink, это означает, что больше нет данных о текущем состоянии ресурса. В последующих запросах приложение использует URL-адрес deltaLink, чтобы узнавать об изменениях ресурса.</span><span class="sxs-lookup"><span data-stu-id="998c4-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="998c4-161">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="998c4-161">See:</span></span></br>
- <span data-ttu-id="998c4-162">[Дополнительные сведения](../../../concepts/delta_query_overview.md)</span><span class="sxs-lookup"><span data-stu-id="998c4-162">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="998c4-163">[Примеры запросов](../../../concepts/delta_query_groups.md)</span><span class="sxs-lookup"><span data-stu-id="998c4-163">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for an example requests.</span></span></br>
    
## <a name="example"></a><span data-ttu-id="998c4-164">Пример</span><span class="sxs-lookup"><span data-stu-id="998c4-164">Example</span></span>
#### <a name="request"></a><span data-ttu-id="998c4-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="998c4-165">Request</span></span>
<span data-ttu-id="998c4-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="998c4-166">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response"></a><span data-ttu-id="998c4-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="998c4-167">Response</span></span>
<span data-ttu-id="998c4-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="998c4-168">The following is an example of the response.</span></span>
><span data-ttu-id="998c4-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="998c4-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->