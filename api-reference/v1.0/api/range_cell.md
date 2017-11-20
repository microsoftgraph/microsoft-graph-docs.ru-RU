# <a name="range-cell"></a><span data-ttu-id="d50d9-101">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="d50d9-101">Range: Cell</span></span>

<span data-ttu-id="d50d9-p101">Получает объект диапазона, содержащий одну ячейку, на основе номера строки и столбца. Ячейка может быть вне родительского диапазона, если она расположена в таблице листа. Возвращаемая ячейка располагается относительно верхней левой ячейки диапазона.</span><span class="sxs-lookup"><span data-stu-id="d50d9-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="d50d9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d50d9-105">Permissions</span></span>
<span data-ttu-id="d50d9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d50d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d50d9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d50d9-108">Permission type</span></span>      | <span data-ttu-id="d50d9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d50d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d50d9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d50d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d50d9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d50d9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d50d9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d50d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d50d9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d50d9-113">Not supported.</span></span>    |
|<span data-ttu-id="d50d9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d50d9-114">Application</span></span> | <span data-ttu-id="d50d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d50d9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d50d9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d50d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="d50d9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d50d9-117">Request headers</span></span>
| <span data-ttu-id="d50d9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d50d9-118">Name</span></span>       | <span data-ttu-id="d50d9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d50d9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d50d9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d50d9-120">Authorization</span></span>  | <span data-ttu-id="d50d9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d50d9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d50d9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d50d9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d50d9-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d50d9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d50d9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d50d9-126">Request body</span></span>
<span data-ttu-id="d50d9-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d50d9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d50d9-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="d50d9-128">Parameter</span></span>    | <span data-ttu-id="d50d9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d50d9-129">Type</span></span>   |<span data-ttu-id="d50d9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d50d9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d50d9-131">row</span><span class="sxs-lookup"><span data-stu-id="d50d9-131">row</span></span>|<span data-ttu-id="d50d9-132">number</span><span class="sxs-lookup"><span data-stu-id="d50d9-132">number</span></span>|<span data-ttu-id="d50d9-p105">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="d50d9-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="d50d9-135">column</span><span class="sxs-lookup"><span data-stu-id="d50d9-135">column</span></span>|<span data-ttu-id="d50d9-136">number</span><span class="sxs-lookup"><span data-stu-id="d50d9-136">number</span></span>|<span data-ttu-id="d50d9-p106">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="d50d9-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="d50d9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d50d9-139">Response</span></span>

<span data-ttu-id="d50d9-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d50d9-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d50d9-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d50d9-141">Example</span></span>
<span data-ttu-id="d50d9-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d50d9-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d50d9-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d50d9-143">Request</span></span>
<span data-ttu-id="d50d9-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d50d9-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="d50d9-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d50d9-145">Response</span></span>
<span data-ttu-id="d50d9-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d50d9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->