# <a name="worksheet-cell"></a><span data-ttu-id="9077b-101">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="9077b-101">Worksheet: Cell</span></span>

<span data-ttu-id="9077b-p101">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="9077b-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9077b-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9077b-104">Prerequisites</span></span>
<span data-ttu-id="9077b-105">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="9077b-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="9077b-106">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="9077b-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="9077b-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9077b-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="9077b-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9077b-108">Request headers</span></span>
| <span data-ttu-id="9077b-109">Имя</span><span class="sxs-lookup"><span data-stu-id="9077b-109">Name</span></span>       | <span data-ttu-id="9077b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9077b-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9077b-111">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9077b-111">Authorization</span></span>  | <span data-ttu-id="9077b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9077b-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9077b-114">Отклик</span><span class="sxs-lookup"><span data-stu-id="9077b-114">Response</span></span>

<span data-ttu-id="9077b-115">В случае успеха этот метод возвращает код отклика `200, OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9077b-115">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9077b-116">Пример</span><span class="sxs-lookup"><span data-stu-id="9077b-116">Example</span></span>
<span data-ttu-id="9077b-117">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9077b-117">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9077b-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="9077b-118">Request</span></span>
<span data-ttu-id="9077b-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9077b-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="9077b-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="9077b-120">Response</span></span>
<span data-ttu-id="9077b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9077b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
