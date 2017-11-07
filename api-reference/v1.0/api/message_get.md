# <a name="get-message"></a><span data-ttu-id="51737-101">Получение message</span><span class="sxs-lookup"><span data-stu-id="51737-101">Get message</span></span>

<span data-ttu-id="51737-102">Получение свойств и связей объекта [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="51737-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="51737-103">Так как ресурс **message** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="51737-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="51737-104">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="51737-104">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="51737-105">Получение сообщений из папки другого пользователя</span><span class="sxs-lookup"><span data-stu-id="51737-105">Get messages in another user's message folder</span></span>

<span data-ttu-id="51737-106">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, то вы можете получить сообщения из папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="51737-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="51737-107">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="51737-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="51737-108">Например, ваше приложение получило делегированные разрешения от пользователя с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="51737-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="51737-109">Предположим, что другой пользователь (Garth) поделился своей папкой сообщений с Никитой.</span><span class="sxs-lookup"><span data-stu-id="51737-109">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="51737-110">Вы можете получить сообщение из этой общей папки, указав идентификатор пользователя (или имя участника-пользователя) Garth, пример соответствующего запроса показан ниже.</span><span class="sxs-lookup"><span data-stu-id="51737-110">You can get a contact in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages/{id}
```

<span data-ttu-id="51737-111">Эта возможность распространяется на все поддерживаемые операции GET над сообщениями для отдельного пользователя, как показано в приведенном ниже разделе [HTTP-запрос](#http-request).</span><span class="sxs-lookup"><span data-stu-id="51737-111">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="51737-112">Она также применяется, если пользователь Garth делегировал разрешения на доступ ко всему своему почтовому ящику пользователю с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="51737-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="51737-113">Если пользователь Garth не поделился своей папкой сообщений с Никитой и не делегировал этому пользователю разрешения на доступ к своему почтовому ящику, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="51737-113">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="51737-114">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно получить только сообщение из папки пользователя, выполнившего вход, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="51737-114">In such cases, specifying a user ID or user principal name only works for getting a contact in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
```

<span data-ttu-id="51737-115">Эта возможность доступна только в операциях GET для следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="51737-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="51737-116">общие папки контактов, календари и папки сообщений;</span><span class="sxs-lookup"><span data-stu-id="51737-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="51737-117">контакты, события и сообщения в общих папках;</span><span class="sxs-lookup"><span data-stu-id="51737-117">Contacts and events in shared folders</span></span>
- <span data-ttu-id="51737-118">указанные выше ресурсы в тех почтовых ящиках, разрешения на доступ к которым делегированы.</span><span class="sxs-lookup"><span data-stu-id="51737-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="51737-119">Эта возможность недоступна для других операций над контактами, событиями, сообщениями и их папками.</span><span class="sxs-lookup"><span data-stu-id="51737-119">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="51737-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51737-120">Permissions</span></span>
<span data-ttu-id="51737-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="51737-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51737-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51737-123">Permission type</span></span>      | <span data-ttu-id="51737-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51737-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51737-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51737-125">Delegated (work or school account)</span></span> | <span data-ttu-id="51737-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="51737-126">Mail.Read</span></span>    |
|<span data-ttu-id="51737-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51737-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51737-128">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="51737-128">Mail.Read</span></span>    |
|<span data-ttu-id="51737-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51737-129">Application</span></span> | <span data-ttu-id="51737-130">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="51737-130">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="51737-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51737-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="51737-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51737-132">Optional query parameters</span></span>
<span data-ttu-id="51737-133">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51737-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51737-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51737-134">Request headers</span></span>
| <span data-ttu-id="51737-135">Имя</span><span class="sxs-lookup"><span data-stu-id="51737-135">Name</span></span>       | <span data-ttu-id="51737-136">Тип</span><span class="sxs-lookup"><span data-stu-id="51737-136">Type</span></span> | <span data-ttu-id="51737-137">Описание</span><span class="sxs-lookup"><span data-stu-id="51737-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="51737-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="51737-138">Authorization</span></span>  | <span data-ttu-id="51737-139">string</span><span class="sxs-lookup"><span data-stu-id="51737-139">string</span></span>  | <span data-ttu-id="51737-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51737-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51737-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51737-142">Request body</span></span>
<span data-ttu-id="51737-143">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51737-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51737-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="51737-144">Response</span></span>

<span data-ttu-id="51737-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51737-145">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51737-146">Пример</span><span class="sxs-lookup"><span data-stu-id="51737-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51737-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="51737-147">Request</span></span>
<span data-ttu-id="51737-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51737-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="51737-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="51737-149">Response</span></span>
<span data-ttu-id="51737-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51737-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="51737-153">См. также</span><span class="sxs-lookup"><span data-stu-id="51737-153">See also</span></span>

- [<span data-ttu-id="51737-154">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="51737-154">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="51737-155">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="51737-155">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
