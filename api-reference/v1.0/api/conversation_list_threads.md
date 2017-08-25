# <a name="list-threads"></a><span data-ttu-id="1c917-101">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="1c917-101">List threads</span></span>

<span data-ttu-id="1c917-102">Получение всех цепочек в беседе группы.</span><span class="sxs-lookup"><span data-stu-id="1c917-102">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="1c917-103">Примечание. Вы можете [получить все цепочки группы](group_list_threads.md).</span><span class="sxs-lookup"><span data-stu-id="1c917-103">Note: You can also [get all the threads of a group](group_list_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c917-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c917-104">Permissions</span></span>
<span data-ttu-id="1c917-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c917-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c917-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c917-107">Permission type</span></span>      | <span data-ttu-id="1c917-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c917-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="1c917-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c917-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1c917-110">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c917-110">Group.ReadWrite.All, Group.Read.All</span></span>    | 
|<span data-ttu-id="1c917-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c917-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c917-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c917-112">Not supported.</span></span>    | 
|<span data-ttu-id="1c917-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c917-113">Application</span></span> | <span data-ttu-id="1c917-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c917-114">Group.ReadWrite.All, Group.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1c917-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c917-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c917-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1c917-116">Optional query parameters</span></span>
<span data-ttu-id="1c917-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1c917-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1c917-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c917-118">Request headers</span></span>
| <span data-ttu-id="1c917-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c917-119">Header</span></span>       | <span data-ttu-id="1c917-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1c917-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c917-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c917-121">Authorization</span></span>  | <span data-ttu-id="1c917-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c917-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c917-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c917-124">Request body</span></span>
<span data-ttu-id="1c917-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c917-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c917-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c917-126">Response</span></span>

<span data-ttu-id="1c917-127">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c917-127">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c917-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1c917-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c917-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c917-129">Request</span></span>
<span data-ttu-id="1c917-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c917-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="1c917-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c917-131">Response</span></span>
<span data-ttu-id="1c917-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1c917-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
