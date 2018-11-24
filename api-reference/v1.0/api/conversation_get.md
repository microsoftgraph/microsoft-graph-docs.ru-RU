# <a name="get-conversation"></a><span data-ttu-id="53d24-101">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="53d24-101">Get conversation</span></span>

<span data-ttu-id="53d24-102">Получение свойств и связей объекта беседы.</span><span class="sxs-lookup"><span data-stu-id="53d24-102">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="53d24-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53d24-103">Permissions</span></span>
<span data-ttu-id="53d24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="53d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="53d24-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53d24-106">Permission type</span></span>      | <span data-ttu-id="53d24-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53d24-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53d24-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53d24-108">Delegated (work or school account)</span></span> | <span data-ttu-id="53d24-109">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="53d24-109">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="53d24-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53d24-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53d24-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53d24-111">Not supported.</span></span>    |
|<span data-ttu-id="53d24-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53d24-112">Application</span></span> | <span data-ttu-id="53d24-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="53d24-113">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53d24-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53d24-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="53d24-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53d24-115">Optional query parameters</span></span>
<span data-ttu-id="53d24-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="53d24-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="53d24-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53d24-117">Request headers</span></span>
| <span data-ttu-id="53d24-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53d24-118">Header</span></span>       | <span data-ttu-id="53d24-119">Значение</span><span class="sxs-lookup"><span data-stu-id="53d24-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53d24-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53d24-120">Authorization</span></span>  | <span data-ttu-id="53d24-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53d24-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53d24-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53d24-123">Request body</span></span>
<span data-ttu-id="53d24-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53d24-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53d24-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="53d24-125">Response</span></span>

<span data-ttu-id="53d24-126">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53d24-126">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53d24-127">Пример</span><span class="sxs-lookup"><span data-stu-id="53d24-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53d24-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="53d24-128">Request</span></span>
<span data-ttu-id="53d24-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53d24-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="53d24-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="53d24-130">Response</span></span>
<span data-ttu-id="53d24-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="53d24-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
