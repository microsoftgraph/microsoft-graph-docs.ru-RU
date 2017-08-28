# <a name="get-mailfolder"></a><span data-ttu-id="c2bc9-101">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="c2bc9-101">Get mailFolder</span></span>

<span data-ttu-id="c2bc9-102">Получение свойств и связей объекта mailfolder.</span><span class="sxs-lookup"><span data-stu-id="c2bc9-102">Retrieve the properties and relationships of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2bc9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2bc9-103">Permissions</span></span>
<span data-ttu-id="c2bc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c2bc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c2bc9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2bc9-106">Permission type</span></span>      | <span data-ttu-id="c2bc9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2bc9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2bc9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2bc9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c2bc9-109">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2bc9-109">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c2bc9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2bc9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2bc9-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2bc9-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c2bc9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2bc9-112">Application</span></span> | <span data-ttu-id="c2bc9-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2bc9-113">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2bc9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2bc9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2bc9-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2bc9-115">Optional query parameters</span></span>
<span data-ttu-id="c2bc9-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2bc9-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c2bc9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2bc9-117">Request headers</span></span>
| <span data-ttu-id="c2bc9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c2bc9-118">Name</span></span>       | <span data-ttu-id="c2bc9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c2bc9-119">Type</span></span> | <span data-ttu-id="c2bc9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c2bc9-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c2bc9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2bc9-121">Authorization</span></span>  | <span data-ttu-id="c2bc9-122">string</span><span class="sxs-lookup"><span data-stu-id="c2bc9-122">string</span></span>  | <span data-ttu-id="c2bc9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2bc9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2bc9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2bc9-125">Request body</span></span>
<span data-ttu-id="c2bc9-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2bc9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2bc9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2bc9-127">Response</span></span>

<span data-ttu-id="c2bc9-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2bc9-128">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2bc9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c2bc9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2bc9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2bc9-130">Request</span></span>
<span data-ttu-id="c2bc9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2bc9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="c2bc9-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2bc9-132">Response</span></span>
<span data-ttu-id="c2bc9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c2bc9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
