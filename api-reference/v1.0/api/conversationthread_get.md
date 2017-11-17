# <a name="get-conversationthread"></a><span data-ttu-id="c545f-101">Получение объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="c545f-101">Get conversationThread</span></span>

<span data-ttu-id="c545f-p101">Получение определенной цепочки, принадлежащей группе. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="c545f-p101">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="c545f-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c545f-104">Permissions</span></span>
<span data-ttu-id="c545f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c545f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c545f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c545f-107">Permission type</span></span>      | <span data-ttu-id="c545f-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c545f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c545f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c545f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c545f-110">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c545f-110">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="c545f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c545f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c545f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c545f-112">Not supported.</span></span>    |
|<span data-ttu-id="c545f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c545f-113">Application</span></span> | <span data-ttu-id="c545f-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c545f-114">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c545f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c545f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="c545f-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c545f-116">Optional query parameters</span></span>
<span data-ttu-id="c545f-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c545f-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c545f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c545f-118">Request headers</span></span>
| <span data-ttu-id="c545f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c545f-119">Header</span></span>       | <span data-ttu-id="c545f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c545f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c545f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c545f-121">Authorization</span></span>  | <span data-ttu-id="c545f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c545f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c545f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c545f-124">Request body</span></span>
<span data-ttu-id="c545f-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c545f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c545f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c545f-126">Response</span></span>

<span data-ttu-id="c545f-127">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c545f-127">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c545f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c545f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c545f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c545f-129">Request</span></span>
<span data-ttu-id="c545f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c545f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="c545f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c545f-131">Response</span></span>
<span data-ttu-id="c545f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c545f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
