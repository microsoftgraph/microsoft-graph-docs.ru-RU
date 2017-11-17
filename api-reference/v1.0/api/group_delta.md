# <a name="group-delta"></a><span data-ttu-id="865f6-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="865f6-101">group: delta</span></span>

<span data-ttu-id="865f6-p101">[Запросы изменений](../../../concepts/delta_query_overview.md) позволяют приложениям обнаруживать новые, обновленные и удаленные сущности, не считывая целевой ресурс полностью при каждом запросе. Чтобы узнать об изменениях в группах, выполните запрос с помощью функции *delta*. Подробные сведения вы найдете [здесь](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="865f6-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to groups, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="865f6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="865f6-105">Permissions</span></span>

<span data-ttu-id="865f6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="865f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="865f6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="865f6-108">Permission type</span></span>      | <span data-ttu-id="865f6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="865f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="865f6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="865f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="865f6-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="865f6-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="865f6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="865f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="865f6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="865f6-113">Not supported.</span></span>    |
|<span data-ttu-id="865f6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="865f6-114">Application</span></span> | <span data-ttu-id="865f6-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="865f6-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="865f6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="865f6-116">HTTP request</span></span>

<span data-ttu-id="865f6-117">Чтобы начать отслеживать изменения, выполните запрос к ресурсу groups, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="865f6-117">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a><span data-ttu-id="865f6-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="865f6-118">Query parameters</span></span>

<span data-ttu-id="865f6-p103">Отслеживание изменений в группах — это цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в первом запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в ответ. Параметры запроса нужно указать только один раз в первом запросе. Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="865f6-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="865f6-124">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="865f6-124">Query parameter</span></span>      | <span data-ttu-id="865f6-125">Тип</span><span class="sxs-lookup"><span data-stu-id="865f6-125">Type</span></span>   |<span data-ttu-id="865f6-126">Описание</span><span class="sxs-lookup"><span data-stu-id="865f6-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="865f6-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="865f6-127">$deltatoken</span></span> | <span data-ttu-id="865f6-128">string</span><span class="sxs-lookup"><span data-stu-id="865f6-128">string</span></span> | <span data-ttu-id="865f6-p104">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции групп и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="865f6-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="865f6-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="865f6-131">$skiptoken</span></span> | <span data-ttu-id="865f6-132">строка</span><span class="sxs-lookup"><span data-stu-id="865f6-132">string</span></span> | <span data-ttu-id="865f6-133">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции групп получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="865f6-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="865f6-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="865f6-134">Optional query parameters</span></span>

<span data-ttu-id="865f6-135">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="865f6-135">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="865f6-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="865f6-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="865f6-138">Запросы изменений поддерживают параметры `$select`, `$top` и `$expand` для групп.</span><span class="sxs-lookup"><span data-stu-id="865f6-138">Delta query support `$select`, `$top`, and `$expand` for groups.</span></span> 
- <span data-ttu-id="865f6-p106">Единственное поддерживаемое выражение с параметром `$orderby` — `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке.</span><span class="sxs-lookup"><span data-stu-id="865f6-p106">There is limited support for `$orderby`: The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="865f6-141">Параметр `$search` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="865f6-141">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="865f6-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="865f6-142">Request headers</span></span>
| <span data-ttu-id="865f6-143">Имя</span><span class="sxs-lookup"><span data-stu-id="865f6-143">Name</span></span>       | <span data-ttu-id="865f6-144">Описание</span><span class="sxs-lookup"><span data-stu-id="865f6-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="865f6-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="865f6-145">Authorization</span></span>  | <span data-ttu-id="865f6-146">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="865f6-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="865f6-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="865f6-147">Content-Type</span></span>  | <span data-ttu-id="865f6-148">application/json</span><span class="sxs-lookup"><span data-stu-id="865f6-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="865f6-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="865f6-149">Request body</span></span>
<span data-ttu-id="865f6-150">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="865f6-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="865f6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="865f6-151">Response</span></span>

<span data-ttu-id="865f6-p107">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект коллекции [group](../resources/group.md) в тексте ответа. Ответ также включает токен состояния — URL-адрес nextLink или deltaLink.</span><span class="sxs-lookup"><span data-stu-id="865f6-p107">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body. The response also includes a state token which is either a nextLink URL or a deltaLink URL.</span></span>

- <span data-ttu-id="865f6-p108">Если возвращается URL-адрес nextLink, это означает, что во время сеанса получены не все страницы данных. Приложение продолжает отправлять запросы, используя URL-адрес nextLink, пока в ответ не будет включен URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="865f6-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="865f6-p109">Если возвращается URL-адрес deltaLink, это означает, что больше нет данных о текущем состоянии ресурса. В последующих запросах приложение использует URL-адрес deltaLink, чтобы узнавать об изменениях ресурса.</span><span class="sxs-lookup"><span data-stu-id="865f6-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="865f6-158">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="865f6-158">See:</span></span></br>
- <span data-ttu-id="865f6-159">[Дополнительные сведения](../../../concepts/delta_query_overview.md)</span><span class="sxs-lookup"><span data-stu-id="865f6-159">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="865f6-160">[Примеры запросов](../../../concepts/delta_query_groups.md)</span><span class="sxs-lookup"><span data-stu-id="865f6-160">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for an example requests.</span></span></br>
    
## <a name="example"></a><span data-ttu-id="865f6-161">Пример</span><span class="sxs-lookup"><span data-stu-id="865f6-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="865f6-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="865f6-162">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

##### <a name="response"></a><span data-ttu-id="865f6-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="865f6-163">Response</span></span>
<span data-ttu-id="865f6-p110">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="865f6-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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