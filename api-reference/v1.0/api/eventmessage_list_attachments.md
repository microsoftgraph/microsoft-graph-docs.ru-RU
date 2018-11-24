# <a name="list-attachments"></a><span data-ttu-id="5dba4-101">Список вложений</span><span class="sxs-lookup"><span data-stu-id="5dba4-101">List attachments</span></span>

<span data-ttu-id="5dba4-102">Получение списка объектов вложений.</span><span class="sxs-lookup"><span data-stu-id="5dba4-102">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5dba4-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5dba4-103">Permissions</span></span>
<span data-ttu-id="5dba4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5dba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5dba4-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5dba4-106">Permission type</span></span>      | <span data-ttu-id="5dba4-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5dba4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dba4-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5dba4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5dba4-109">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5dba4-109">Mail.Read</span></span>    |
|<span data-ttu-id="5dba4-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5dba4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dba4-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5dba4-111">Mail.Read</span></span>    |
|<span data-ttu-id="5dba4-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5dba4-112">Application</span></span> | <span data-ttu-id="5dba4-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5dba4-113">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dba4-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5dba4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5dba4-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5dba4-115">Optional query parameters</span></span>
<span data-ttu-id="5dba4-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5dba4-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5dba4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5dba4-117">Request headers</span></span>
| <span data-ttu-id="5dba4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5dba4-118">Name</span></span>       | <span data-ttu-id="5dba4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5dba4-119">Type</span></span> | <span data-ttu-id="5dba4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5dba4-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5dba4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dba4-121">Authorization</span></span>  | <span data-ttu-id="5dba4-122">string</span><span class="sxs-lookup"><span data-stu-id="5dba4-122">string</span></span>  | <span data-ttu-id="5dba4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5dba4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dba4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5dba4-125">Request body</span></span>
<span data-ttu-id="5dba4-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5dba4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dba4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5dba4-127">Response</span></span>

<span data-ttu-id="5dba4-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5dba4-128">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5dba4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5dba4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5dba4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5dba4-130">Request</span></span>
<span data-ttu-id="5dba4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5dba4-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="5dba4-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5dba4-132">Response</span></span>
<span data-ttu-id="5dba4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5dba4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
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
