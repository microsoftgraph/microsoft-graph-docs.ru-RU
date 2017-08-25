# <a name="list-attachments"></a><span data-ttu-id="a423c-101">Список вложений</span><span class="sxs-lookup"><span data-stu-id="a423c-101">List attachments</span></span>

<span data-ttu-id="a423c-102">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="a423c-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="a423c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a423c-103">Permissions</span></span>
<span data-ttu-id="a423c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a423c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a423c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a423c-106">Permission type</span></span>      | <span data-ttu-id="a423c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a423c-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="a423c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a423c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a423c-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a423c-109">Group.Read.All, Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="a423c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a423c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a423c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a423c-111">Not supported.</span></span>    | 
|<span data-ttu-id="a423c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a423c-112">Application</span></span> | <span data-ttu-id="a423c-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a423c-113">Group.Read.All, Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a423c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a423c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a423c-115">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="a423c-115">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a423c-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a423c-116">Optional query parameters</span></span>
<span data-ttu-id="a423c-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a423c-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a423c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a423c-118">Request headers</span></span>
| <span data-ttu-id="a423c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a423c-119">Header</span></span>       | <span data-ttu-id="a423c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a423c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a423c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a423c-121">Authorization</span></span>  | <span data-ttu-id="a423c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a423c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a423c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a423c-124">Request body</span></span>
<span data-ttu-id="a423c-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a423c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a423c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a423c-126">Response</span></span>

<span data-ttu-id="a423c-127">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a423c-127">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a423c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="a423c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a423c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a423c-129">Request</span></span>
<span data-ttu-id="a423c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a423c-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="a423c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a423c-131">Response</span></span>
<span data-ttu-id="a423c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a423c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
