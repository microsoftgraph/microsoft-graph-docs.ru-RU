# <a name="list-messages"></a><span data-ttu-id="0f670-101">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="0f670-101">List messages</span></span>

<span data-ttu-id="0f670-102">Получение всех сообщений в почтовом ящике вошедшего пользователя или в указанной папке этого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="0f670-102">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="0f670-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f670-103">Permissions</span></span>
<span data-ttu-id="0f670-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0f670-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f670-106">Permission type</span></span>      | <span data-ttu-id="0f670-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f670-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f670-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f670-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0f670-109">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f670-109">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0f670-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f670-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f670-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f670-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0f670-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f670-112">Application</span></span> | <span data-ttu-id="0f670-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f670-113">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f670-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f670-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0f670-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0f670-115">Optional query parameters</span></span>
<span data-ttu-id="0f670-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0f670-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0f670-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f670-117">Request headers</span></span>
| <span data-ttu-id="0f670-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0f670-118">Name</span></span>       | <span data-ttu-id="0f670-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0f670-119">Type</span></span> | <span data-ttu-id="0f670-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0f670-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0f670-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f670-121">Authorization</span></span>  | <span data-ttu-id="0f670-122">string</span><span class="sxs-lookup"><span data-stu-id="0f670-122">string</span></span>  | <span data-ttu-id="0f670-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f670-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f670-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f670-125">Request body</span></span>
<span data-ttu-id="0f670-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f670-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f670-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f670-127">Response</span></span>

<span data-ttu-id="0f670-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f670-128">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f670-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0f670-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f670-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f670-130">Request</span></span>
<span data-ttu-id="0f670-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f670-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="0f670-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f670-132">Response</span></span>
<span data-ttu-id="0f670-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0f670-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
