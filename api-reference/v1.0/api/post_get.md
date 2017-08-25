# <a name="get-post"></a><span data-ttu-id="f6aa3-101">Вывод записи</span><span class="sxs-lookup"><span data-stu-id="f6aa3-101">Get post</span></span>

<span data-ttu-id="f6aa3-p101">Получение свойств и связей записи в указанной цепочке. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="f6aa3-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="f6aa3-104">Так как ресурс **post** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **post**.</span><span class="sxs-lookup"><span data-stu-id="f6aa3-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6aa3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6aa3-105">Permissions</span></span>
<span data-ttu-id="f6aa3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6aa3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f6aa3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6aa3-108">Permission type</span></span>      | <span data-ttu-id="f6aa3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6aa3-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f6aa3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6aa3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6aa3-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6aa3-111">Group.Read.All, Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="f6aa3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6aa3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6aa3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6aa3-113">Not supported.</span></span>    | 
|<span data-ttu-id="f6aa3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6aa3-114">Application</span></span> | <span data-ttu-id="f6aa3-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6aa3-115">Group.Read.All, Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f6aa3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6aa3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6aa3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6aa3-117">Optional query parameters</span></span>
<span data-ttu-id="f6aa3-118">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6aa3-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f6aa3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6aa3-119">Request headers</span></span>
| <span data-ttu-id="f6aa3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6aa3-120">Header</span></span>       | <span data-ttu-id="f6aa3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f6aa3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6aa3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6aa3-122">Authorization</span></span>  | <span data-ttu-id="f6aa3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6aa3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6aa3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6aa3-125">Request body</span></span>
<span data-ttu-id="f6aa3-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6aa3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6aa3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6aa3-127">Response</span></span>

<span data-ttu-id="f6aa3-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6aa3-128">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6aa3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f6aa3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6aa3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6aa3-130">Request</span></span>
<span data-ttu-id="f6aa3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6aa3-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="f6aa3-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6aa3-132">Response</span></span>
<span data-ttu-id="f6aa3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f6aa3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

{
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "receivedDateTime": "datetime-value",
  "hasAttachments": true,
  "from": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  },
  "sender": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="f6aa3-136">См. также</span><span class="sxs-lookup"><span data-stu-id="f6aa3-136">See also</span></span>

- [<span data-ttu-id="f6aa3-137">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="f6aa3-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="f6aa3-138">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f6aa3-138">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
