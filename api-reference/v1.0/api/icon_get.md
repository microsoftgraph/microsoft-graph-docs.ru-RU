# <a name="get-icon"></a><span data-ttu-id="4ecc4-101">Получение объекта Icon</span><span class="sxs-lookup"><span data-stu-id="4ecc4-101">Get Icon</span></span>

<span data-ttu-id="4ecc4-102">Получение свойств и связей объекта значка.</span><span class="sxs-lookup"><span data-stu-id="4ecc4-102">Retrieve the properties and relationships of icon object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ecc4-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="4ecc4-103">Prerequisites</span></span>
<span data-ttu-id="4ecc4-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="4ecc4-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="4ecc4-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="4ecc4-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="4ecc4-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ecc4-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ecc4-107">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ecc4-107">Optional query parameters</span></span>
<span data-ttu-id="4ecc4-108">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ecc4-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ecc4-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ecc4-109">Request headers</span></span>
| <span data-ttu-id="4ecc4-110">Имя</span><span class="sxs-lookup"><span data-stu-id="4ecc4-110">Name</span></span>      |<span data-ttu-id="4ecc4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ecc4-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ecc4-112">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ecc4-112">Authorization</span></span>  | <span data-ttu-id="4ecc4-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ecc4-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ecc4-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ecc4-115">Request body</span></span>
<span data-ttu-id="4ecc4-116">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ecc4-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ecc4-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ecc4-117">Response</span></span>

<span data-ttu-id="4ecc4-118">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Icon](../resources/icon.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ecc4-118">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ecc4-119">Пример</span><span class="sxs-lookup"><span data-stu-id="4ecc4-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ecc4-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ecc4-120">Request</span></span>
<span data-ttu-id="4ecc4-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ecc4-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="4ecc4-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ecc4-122">Response</span></span>
<span data-ttu-id="4ecc4-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4ecc4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->