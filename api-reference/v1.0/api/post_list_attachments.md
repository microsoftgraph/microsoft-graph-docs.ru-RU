# <a name="list-attachments"></a><span data-ttu-id="548a9-101">Список вложений</span><span class="sxs-lookup"><span data-stu-id="548a9-101">List attachments</span></span>

<span data-ttu-id="548a9-102">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="548a9-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="548a9-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="548a9-103">Prerequisites</span></span>
<span data-ttu-id="548a9-104">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="548a9-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="548a9-105">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="548a9-105">Group.Read.All</span></span>
* <span data-ttu-id="548a9-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="548a9-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="548a9-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="548a9-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="548a9-108">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="548a9-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="548a9-109">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="548a9-109">Optional query parameters</span></span>
<span data-ttu-id="548a9-110">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="548a9-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="548a9-111">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="548a9-111">Request headers</span></span>
| <span data-ttu-id="548a9-112">Заголовок</span><span class="sxs-lookup"><span data-stu-id="548a9-112">Header</span></span>       | <span data-ttu-id="548a9-113">Значение</span><span class="sxs-lookup"><span data-stu-id="548a9-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="548a9-114">Авторизация</span><span class="sxs-lookup"><span data-stu-id="548a9-114">Authorization</span></span>  | <span data-ttu-id="548a9-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="548a9-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="548a9-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="548a9-117">Request body</span></span>
<span data-ttu-id="548a9-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="548a9-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="548a9-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="548a9-119">Response</span></span>

<span data-ttu-id="548a9-120">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="548a9-120">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="548a9-121">Пример</span><span class="sxs-lookup"><span data-stu-id="548a9-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="548a9-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="548a9-122">Request</span></span>
<span data-ttu-id="548a9-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="548a9-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="548a9-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="548a9-124">Response</span></span>
<span data-ttu-id="548a9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="548a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
