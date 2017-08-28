# <a name="get-message"></a><span data-ttu-id="3ea44-101">Получение message</span><span class="sxs-lookup"><span data-stu-id="3ea44-101">Get message</span></span>

<span data-ttu-id="3ea44-102">Получение свойств и связей объекта [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="3ea44-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="3ea44-103">Так как ресурс **message** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="3ea44-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="3ea44-104">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="3ea44-104">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ea44-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea44-105">Permissions</span></span>
<span data-ttu-id="3ea44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ea44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3ea44-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea44-108">Permission type</span></span>      | <span data-ttu-id="3ea44-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ea44-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ea44-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ea44-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ea44-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ea44-111">Mail.Read</span></span>    |
|<span data-ttu-id="3ea44-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ea44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ea44-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ea44-113">Mail.Read</span></span>    |
|<span data-ttu-id="3ea44-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ea44-114">Application</span></span> | <span data-ttu-id="3ea44-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ea44-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ea44-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ea44-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3ea44-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3ea44-117">Optional query parameters</span></span>
<span data-ttu-id="3ea44-118">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3ea44-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3ea44-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ea44-119">Request headers</span></span>
| <span data-ttu-id="3ea44-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3ea44-120">Name</span></span>       | <span data-ttu-id="3ea44-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3ea44-121">Type</span></span> | <span data-ttu-id="3ea44-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3ea44-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ea44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ea44-123">Authorization</span></span>  | <span data-ttu-id="3ea44-124">string</span><span class="sxs-lookup"><span data-stu-id="3ea44-124">string</span></span>  | <span data-ttu-id="3ea44-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ea44-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ea44-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ea44-127">Request body</span></span>
<span data-ttu-id="3ea44-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ea44-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ea44-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea44-129">Response</span></span>

<span data-ttu-id="3ea44-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ea44-130">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3ea44-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3ea44-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ea44-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea44-132">Request</span></span>
<span data-ttu-id="3ea44-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ea44-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="3ea44-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ea44-134">Response</span></span>
<span data-ttu-id="3ea44-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3ea44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3ea44-138">См. также</span><span class="sxs-lookup"><span data-stu-id="3ea44-138">See also</span></span>

- [<span data-ttu-id="3ea44-139">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="3ea44-139">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="3ea44-140">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3ea44-140">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
