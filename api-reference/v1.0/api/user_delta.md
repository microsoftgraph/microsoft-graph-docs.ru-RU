# <a name="user-delta"></a><span data-ttu-id="e5e2d-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="e5e2d-101">user: delta</span></span>

<span data-ttu-id="e5e2d-p101">[Запросы изменений](../../../concepts/delta_query_overview.md) позволяют приложениям обнаруживать новые, обновленные и удаленные сущности, не считывая целевой ресурс полностью при каждом запросе. Чтобы узнать об изменениях в ресурсе users, выполните запрос с помощью функции *delta*. Подробные сведения вы найдете [здесь](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="e5e2d-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to users, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5e2d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5e2d-105">Permissions</span></span>

<span data-ttu-id="e5e2d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e5e2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e5e2d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5e2d-108">Permission type</span></span>      | <span data-ttu-id="e5e2d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5e2d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5e2d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5e2d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5e2d-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5e2d-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5e2d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5e2d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5e2d-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5e2d-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="e5e2d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5e2d-114">Application</span></span> | <span data-ttu-id="e5e2d-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5e2d-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5e2d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5e2d-116">HTTP request</span></span>

<span data-ttu-id="e5e2d-117">Чтобы начать отслеживать изменения, выполните запрос к ресурсу users, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-117">To begin tracking changes, you make a request including the delta function on the users resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

### <a name="query-parameters"></a><span data-ttu-id="e5e2d-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="e5e2d-118">Query parameters</span></span>

<span data-ttu-id="e5e2d-p103">Отслеживание изменений в ресурсе users — это цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в первом запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в ответ. Параметры запроса нужно указать только один раз в первом запросе. Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-p103">Tracking changes in users incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="e5e2d-124">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="e5e2d-124">Query parameter</span></span>      | <span data-ttu-id="e5e2d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e5e2d-125">Type</span></span>   |<span data-ttu-id="e5e2d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e5e2d-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5e2d-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="e5e2d-127">$deltatoken</span></span> | <span data-ttu-id="e5e2d-128">string</span><span class="sxs-lookup"><span data-stu-id="e5e2d-128">string</span></span> | <span data-ttu-id="e5e2d-p104">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="e5e2d-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e5e2d-131">$skiptoken</span></span> | <span data-ttu-id="e5e2d-132">строка</span><span class="sxs-lookup"><span data-stu-id="e5e2d-132">string</span></span> | <span data-ttu-id="e5e2d-133">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e5e2d-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5e2d-134">Optional query parameters</span></span>

<span data-ttu-id="e5e2d-135">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-135">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="e5e2d-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="e5e2d-138">Запросы изменений поддерживают параметры `$select`, `$top` и `$expand` для сообщений.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-138">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="e5e2d-139">Имеется ограниченная поддержка параметров `$filter` и `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="e5e2d-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="e5e2d-140">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений, касающихся одного или двух определенных пользователей: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-140">The only supported `$filter` expression is for tracking changes on one or two specific users:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`</span></span> 
  * <span data-ttu-id="e5e2d-141">Единственное поддерживаемое выражение `$orderby` выглядит как `$orderby=receivedDateTime+desc`.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-141">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`.</span></span> <span data-ttu-id="e5e2d-142">Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-142">The only supported  expression is . If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="e5e2d-143">Параметр `$search` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-143">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5e2d-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5e2d-144">Request headers</span></span>
| <span data-ttu-id="e5e2d-145">Имя</span><span class="sxs-lookup"><span data-stu-id="e5e2d-145">Name</span></span>       | <span data-ttu-id="e5e2d-146">Описание</span><span class="sxs-lookup"><span data-stu-id="e5e2d-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5e2d-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5e2d-147">Authorization</span></span>  | <span data-ttu-id="e5e2d-148">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="e5e2d-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="e5e2d-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5e2d-149">Content-Type</span></span>  | <span data-ttu-id="e5e2d-150">application/json</span><span class="sxs-lookup"><span data-stu-id="e5e2d-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5e2d-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5e2d-151">Request body</span></span>
<span data-ttu-id="e5e2d-152">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5e2d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5e2d-153">Response</span></span>

<span data-ttu-id="e5e2d-p107">В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции [user](../resources/user.md) в тексте ответа. Ответ также включает URL-адрес nextLink или deltaLink.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-p107">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body. The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="e5e2d-p108">Если возвращается URL-адрес nextLink, это означает, что во время сеанса получены не все страницы данных. Приложение продолжает отправлять запросы, используя URL-адрес nextLink, пока в ответ не будет включен URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="e5e2d-p109">Если возвращается URL-адрес deltaLink, это означает, что больше нет данных о текущем состоянии ресурса. В последующих запросах приложение использует URL-адрес deltaLink, чтобы узнавать об изменениях ресурса.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="e5e2d-160">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="e5e2d-160">See:</span></span></br>
- <span data-ttu-id="e5e2d-161">[Дополнительные сведения](../../../concepts/delta_query_overview.md)</span><span class="sxs-lookup"><span data-stu-id="e5e2d-161">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="e5e2d-162">[Примеры запросов](../../../concepts/delta_query_users.md)</span><span class="sxs-lookup"><span data-stu-id="e5e2d-162">[Get incremental changes for users](../../../concepts/delta_query_users.md) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="e5e2d-163">Пример</span><span class="sxs-lookup"><span data-stu-id="e5e2d-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5e2d-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5e2d-164">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/delta
```

##### <a name="response"></a><span data-ttu-id="e5e2d-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5e2d-165">Response</span></span>
<span data-ttu-id="e5e2d-p110">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5e2d-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->