# <a name="list-conversations"></a><span data-ttu-id="4120f-101">Список бесед</span><span class="sxs-lookup"><span data-stu-id="4120f-101">List conversations</span></span>
<span data-ttu-id="4120f-102">Получение списка объектов [conversation](../resources/conversation.md) в этой группе.</span><span class="sxs-lookup"><span data-stu-id="4120f-102">Retrieve the list of conversations in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="4120f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4120f-103">Permissions</span></span>
<span data-ttu-id="4120f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4120f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4120f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4120f-106">Permission type</span></span>      | <span data-ttu-id="4120f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4120f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4120f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4120f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4120f-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4120f-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4120f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4120f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4120f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4120f-111">Not supported.</span></span>    |
|<span data-ttu-id="4120f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4120f-112">Application</span></span> | <span data-ttu-id="4120f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4120f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4120f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4120f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4120f-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4120f-115">Optional query parameters</span></span>
<span data-ttu-id="4120f-116">Этот метод поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4120f-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4120f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4120f-117">Request headers</span></span>
| <span data-ttu-id="4120f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4120f-118">Header</span></span>       | <span data-ttu-id="4120f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4120f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4120f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4120f-120">Authorization</span></span>  | <span data-ttu-id="4120f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4120f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4120f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4120f-123">Request body</span></span>
<span data-ttu-id="4120f-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4120f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4120f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4120f-125">Response</span></span>
<span data-ttu-id="4120f-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4120f-126">If successful, this method returns a `200 OK` response code and collection of [Conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4120f-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4120f-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4120f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4120f-128">Request</span></span>
<span data-ttu-id="4120f-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4120f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
#### <a name="response"></a><span data-ttu-id="4120f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4120f-130">Response</span></span>
<span data-ttu-id="4120f-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4120f-131">The following is an example of the response.</span></span>
><span data-ttu-id="4120f-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4120f-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4120f-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4120f-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->