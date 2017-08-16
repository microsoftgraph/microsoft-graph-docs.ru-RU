# <a name="worksheet-usedrange"></a><span data-ttu-id="e5f24-101">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="e5f24-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="e5f24-p101">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="e5f24-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5f24-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="e5f24-104">Prerequisites</span></span>
<span data-ttu-id="e5f24-105">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="e5f24-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="e5f24-106">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="e5f24-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="e5f24-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5f24-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="optional-request-parameter"></a><span data-ttu-id="e5f24-108">Необязательный параметр запросов</span><span class="sxs-lookup"><span data-stu-id="e5f24-108">Optional request parameter</span></span>
<span data-ttu-id="e5f24-109">В URL-адресе запроса предоставьте необязательный параметр запросов.</span><span class="sxs-lookup"><span data-stu-id="e5f24-109">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="e5f24-110">Параметр</span><span class="sxs-lookup"><span data-stu-id="e5f24-110">Parameter</span></span>    | <span data-ttu-id="e5f24-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e5f24-111">Type</span></span>   |<span data-ttu-id="e5f24-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e5f24-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5f24-113">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="e5f24-113">valuesOnly</span></span>|<span data-ttu-id="e5f24-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5f24-114">Boolean</span></span>|<span data-ttu-id="e5f24-p102">Необязательный параметр. Учитывает только ячейки со значениями (игнорирует форматирование).</span><span class="sxs-lookup"><span data-stu-id="e5f24-p102">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|


## <a name="request-headers"></a><span data-ttu-id="e5f24-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5f24-117">Request headers</span></span>
| <span data-ttu-id="e5f24-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e5f24-118">Name</span></span>       | <span data-ttu-id="e5f24-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e5f24-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5f24-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5f24-120">Authorization</span></span>  | <span data-ttu-id="e5f24-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5f24-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e5f24-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5f24-123">Response</span></span>

<span data-ttu-id="e5f24-124">В случае успеха этот метод возвращает код отклика `200, OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e5f24-124">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5f24-125">Пример</span><span class="sxs-lookup"><span data-stu-id="e5f24-125">Example</span></span>
<span data-ttu-id="e5f24-126">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e5f24-126">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e5f24-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5f24-127">Request</span></span>
<span data-ttu-id="e5f24-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5f24-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
Content-type: application/json

```

##### <a name="response"></a><span data-ttu-id="e5f24-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5f24-129">Response</span></span>
<span data-ttu-id="e5f24-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5f24-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
