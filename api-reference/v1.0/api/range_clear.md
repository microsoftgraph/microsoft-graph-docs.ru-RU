# <a name="range-clear"></a><span data-ttu-id="e848d-101">Range: clear</span><span class="sxs-lookup"><span data-stu-id="e848d-101">Range: clear</span></span>

<span data-ttu-id="e848d-102">Очищает значения, формат, заливку, границу диапазона и т. д.</span><span class="sxs-lookup"><span data-stu-id="e848d-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e848d-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="e848d-103">Prerequisites</span></span>
<span data-ttu-id="e848d-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="e848d-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="e848d-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="e848d-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="e848d-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e848d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/clear
GET /workbook/worksheets/{id|name}/range(<address>)/clear
GET /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="e848d-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e848d-107">Request headers</span></span>
| <span data-ttu-id="e848d-108">Имя</span><span class="sxs-lookup"><span data-stu-id="e848d-108">Name</span></span>       | <span data-ttu-id="e848d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e848d-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e848d-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e848d-110">Authorization</span></span>  | <span data-ttu-id="e848d-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e848d-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e848d-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e848d-113">Request body</span></span>
<span data-ttu-id="e848d-114">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e848d-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e848d-115">Параметр</span><span class="sxs-lookup"><span data-stu-id="e848d-115">Parameter</span></span>    | <span data-ttu-id="e848d-116">Тип</span><span class="sxs-lookup"><span data-stu-id="e848d-116">Type</span></span>   |<span data-ttu-id="e848d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e848d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e848d-118">applyTo</span><span class="sxs-lookup"><span data-stu-id="e848d-118">applyTo</span></span>|<span data-ttu-id="e848d-119">string</span><span class="sxs-lookup"><span data-stu-id="e848d-119">string</span></span>|<span data-ttu-id="e848d-p102">Необязательный параметр. Определяет тип действия очистки.  Возможные значения: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="e848d-p102">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="e848d-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="e848d-123">Response</span></span>

<span data-ttu-id="e848d-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e848d-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e848d-126">Пример</span><span class="sxs-lookup"><span data-stu-id="e848d-126">Example</span></span>
<span data-ttu-id="e848d-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e848d-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e848d-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="e848d-128">Request</span></span>
<span data-ttu-id="e848d-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e848d-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="e848d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e848d-130">Response</span></span>
<span data-ttu-id="e848d-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e848d-131">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->