# <a name="list-threads"></a><span data-ttu-id="6d18d-101">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="6d18d-101">List threads</span></span>

<span data-ttu-id="6d18d-102">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="6d18d-102">Get all the threads of a group.</span></span>

<span data-ttu-id="6d18d-103">Примечание. Вы также можете [получить все цепочки беседы](conversation_list_threads.md).</span><span class="sxs-lookup"><span data-stu-id="6d18d-103">Note: You can also [get all the threads of a conversation](conversation_list_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d18d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d18d-104">Permissions</span></span>
<span data-ttu-id="6d18d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d18d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6d18d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d18d-107">Permission type</span></span>      | <span data-ttu-id="6d18d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d18d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d18d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d18d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6d18d-110">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d18d-110">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d18d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d18d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d18d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d18d-112">Not supported.</span></span>    |
|<span data-ttu-id="6d18d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d18d-113">Application</span></span> | <span data-ttu-id="6d18d-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d18d-114">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d18d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d18d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d18d-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6d18d-116">Optional query parameters</span></span>
<span data-ttu-id="6d18d-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6d18d-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6d18d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d18d-118">Request headers</span></span>
| <span data-ttu-id="6d18d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d18d-119">Header</span></span>       | <span data-ttu-id="6d18d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6d18d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d18d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d18d-121">Authorization</span></span>  | <span data-ttu-id="6d18d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d18d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d18d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d18d-124">Request body</span></span>
<span data-ttu-id="6d18d-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d18d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d18d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d18d-126">Response</span></span>

<span data-ttu-id="6d18d-127">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ConversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d18d-127">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d18d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="6d18d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d18d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d18d-129">Request</span></span>
<span data-ttu-id="6d18d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d18d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="6d18d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d18d-131">Response</span></span>
<span data-ttu-id="6d18d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6d18d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
