# <a name="worksheet-cell"></a><span data-ttu-id="21664-101">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="21664-101">Worksheet: Cell</span></span>

<span data-ttu-id="21664-p101">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="21664-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="21664-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21664-104">Permissions</span></span>
<span data-ttu-id="21664-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="21664-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="21664-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21664-107">Permission type</span></span>      | <span data-ttu-id="21664-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21664-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21664-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21664-109">Delegated (work or school account)</span></span> | <span data-ttu-id="21664-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21664-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="21664-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21664-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21664-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21664-112">Not supported.</span></span>    |
|<span data-ttu-id="21664-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21664-113">Application</span></span> | <span data-ttu-id="21664-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21664-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21664-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21664-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="21664-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21664-116">Request headers</span></span>
| <span data-ttu-id="21664-117">Имя</span><span class="sxs-lookup"><span data-stu-id="21664-117">Name</span></span>       | <span data-ttu-id="21664-118">Описание</span><span class="sxs-lookup"><span data-stu-id="21664-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="21664-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21664-119">Authorization</span></span>  | <span data-ttu-id="21664-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21664-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21664-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="21664-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="21664-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="21664-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="21664-125">Параметры</span><span class="sxs-lookup"><span data-stu-id="21664-125">Parameters</span></span>
<span data-ttu-id="21664-126">В пути запроса укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="21664-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="21664-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="21664-127">Parameter</span></span>    | <span data-ttu-id="21664-128">Тип</span><span class="sxs-lookup"><span data-stu-id="21664-128">Type</span></span>   |<span data-ttu-id="21664-129">Описание</span><span class="sxs-lookup"><span data-stu-id="21664-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21664-130">row</span><span class="sxs-lookup"><span data-stu-id="21664-130">row</span></span>|<span data-ttu-id="21664-131">Int32</span><span class="sxs-lookup"><span data-stu-id="21664-131">Int32</span></span>|<span data-ttu-id="21664-p105">Номер строки ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="21664-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="21664-134">column</span><span class="sxs-lookup"><span data-stu-id="21664-134">column</span></span>|<span data-ttu-id="21664-135">Int32</span><span class="sxs-lookup"><span data-stu-id="21664-135">Int32</span></span>|<span data-ttu-id="21664-p106">Номер столбца ячейки, которую требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="21664-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="21664-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="21664-138">Response</span></span>

<span data-ttu-id="21664-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="21664-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21664-140">Пример</span><span class="sxs-lookup"><span data-stu-id="21664-140">Example</span></span>
<span data-ttu-id="21664-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="21664-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="21664-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="21664-142">Request</span></span>
<span data-ttu-id="21664-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21664-143">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="21664-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="21664-144">Response</span></span>
<span data-ttu-id="21664-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21664-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
