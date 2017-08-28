# <a name="contactfolder-delta"></a><span data-ttu-id="c3719-101">contactFolder: delta</span><span class="sxs-lookup"><span data-stu-id="c3719-101">contactFolder: delta</span></span>

<span data-ttu-id="c3719-102">Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="c3719-102">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="c3719-p101">Вызов функции **delta** для папок контактов в почтовом ящике похож на запрос GET. С тем исключением, что можно запрашивать добавочные изменения в папках контактов, правильно применяя [маркеры состояния](../../../concepts/delta_query_overview.md) при этих вызовах. Это позволяет обслуживать и синхронизировать локальное хранилище папок контактов пользователя, не загружая каждый раз все папки контактов этого почтового ящика с сервера.</span><span class="sxs-lookup"><span data-stu-id="c3719-p101">A **delta** function call for contact folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](../../../concepts/delta_query_overview.md) in one or more of these calls, you can query for incremental changes in the contact folders. This allows you to maintain and synchronize a local store of a user's contact folders without having to fetch all the contact folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3719-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3719-105">Permissions</span></span>
<span data-ttu-id="c3719-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3719-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c3719-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3719-108">Permission type</span></span>      | <span data-ttu-id="c3719-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3719-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3719-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3719-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3719-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3719-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c3719-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3719-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3719-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3719-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c3719-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3719-114">Application</span></span> | <span data-ttu-id="c3719-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3719-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3719-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3719-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/delta
GET /users/<id>/contactFolders/delta
```

### <a name="query-parameters"></a><span data-ttu-id="c3719-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c3719-117">Query parameters</span></span>

<span data-ttu-id="c3719-p103">Отслеживание изменений в папках контактов представляет собой цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене (`skiptoken` или `$deltatoken`), входящем в состав URL-адреса `nextLink` или `deltaLink`, который включен в отклик. Параметры запроса нужно указать только один раз в первом запросе. Копируйте URL-адрес `nextLink` или `deltaLink` из предыдущего отклика и применяйте его в последующих запросах, так как он уже содержит необходимые закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="c3719-p103">Tracking changes in contact folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion (`skiptoken` or `$deltatoken`) of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="c3719-123">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="c3719-123">Query parameter</span></span>      | <span data-ttu-id="c3719-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c3719-124">Type</span></span>   |<span data-ttu-id="c3719-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c3719-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c3719-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="c3719-126">$deltatoken</span></span> | <span data-ttu-id="c3719-127">string</span><span class="sxs-lookup"><span data-stu-id="c3719-127">string</span></span> | <span data-ttu-id="c3719-p104">Этот [маркер состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** для той же коллекции папок контактов и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="c3719-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same contact folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="c3719-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c3719-130">$skiptoken</span></span> | <span data-ttu-id="c3719-131">string</span><span class="sxs-lookup"><span data-stu-id="c3719-131">string</span></span> | <span data-ttu-id="c3719-132">Этот [маркер состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает, что из коллекции папок контактов получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="c3719-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact folder collection.</span></span> |

#### <a name="odata-query-parameters"></a><span data-ttu-id="c3719-133">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="c3719-133">OData query parameters</span></span>

<span data-ttu-id="c3719-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="c3719-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="c3719-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3719-136">Request headers</span></span>
| <span data-ttu-id="c3719-137">Имя</span><span class="sxs-lookup"><span data-stu-id="c3719-137">Name</span></span>       | <span data-ttu-id="c3719-138">Тип</span><span class="sxs-lookup"><span data-stu-id="c3719-138">Type</span></span> | <span data-ttu-id="c3719-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c3719-139">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="c3719-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3719-140">Authorization</span></span>  | <span data-ttu-id="c3719-141">string</span><span class="sxs-lookup"><span data-stu-id="c3719-141">string</span></span>  | <span data-ttu-id="c3719-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3719-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3719-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3719-144">Content-Type</span></span>  | <span data-ttu-id="c3719-145">string</span><span class="sxs-lookup"><span data-stu-id="c3719-145">string</span></span>  | <span data-ttu-id="c3719-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3719-p107">application/json. Required.</span></span> |
| <span data-ttu-id="c3719-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="c3719-148">Prefer</span></span> | <span data-ttu-id="c3719-149">string</span><span class="sxs-lookup"><span data-stu-id="c3719-149">string</span></span>  | <span data-ttu-id="c3719-p108">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c3719-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c3719-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3719-152">Response</span></span>

<span data-ttu-id="c3719-153">В случае успешного выполнения этот метод возвращает код отклика `200, OK` и объект коллекции [contactFolder](../resources/contactfolder.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c3719-153">If successful, this method returns a `200, OK` response code and [contactFolder](../resources/contactfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3719-154">Пример</span><span class="sxs-lookup"><span data-stu-id="c3719-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3719-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3719-155">Request</span></span>
<span data-ttu-id="c3719-156">В следующем примере показано, как выполнить один вызов функции **delta** и ограничить максимальное количество папок контактов в теле отклика двумя.</span><span class="sxs-lookup"><span data-stu-id="c3719-156">The following example shows how to make a single **delta** function call, and limit the maximum number of contact folders in the response body to 2.</span></span>

<span data-ttu-id="c3719-157">Чтобы отследить изменения в папках контактов почтового ящика, выполните один или несколько вызовов функции **delta** с правильными маркерами состояния, чтобы получить набор добавочных изменений с момента последнего разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="c3719-157">To track changes in the contact folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="c3719-p109">Пример, в котором показано, как использовать маркеры состояния для отслеживания изменений сообщений в почтовой папке: [Получение добавочных изменений сообщений в папке](../../../concepts/delta_query_messages.md). Отслеживания папок контактов и отслеживания сообщений в папках отличаются, прежде всего, URL-адресами разностных запросов и возвращаемыми в откликах коллекциями (**contactFolder** и **message** соответственно).</span><span class="sxs-lookup"><span data-stu-id="c3719-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](../../../concepts/delta_query_messages.md). The main differences between tracking contact folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contactFolder** rather than **message** collections.</span></span>

<!-- {
  "blockType": "request",
  "name": "contactfolder_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="c3719-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3719-160">Response</span></span>

<span data-ttu-id="c3719-161">В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_</span><span class="sxs-lookup"><span data-stu-id="c3719-161">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="c3719-p110">или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_, второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.</span><span class="sxs-lookup"><span data-stu-id="c3719-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="c3719-164">Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="c3719-164">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="c3719-p111">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3719-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/contactfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
     "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="c3719-167">См. также</span><span class="sxs-lookup"><span data-stu-id="c3719-167">See also</span></span>

- [<span data-ttu-id="c3719-168">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="c3719-168">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="c3719-169">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="c3719-169">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->