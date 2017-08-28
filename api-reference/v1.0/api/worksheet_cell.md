# <a name="worksheet-cell"></a><span data-ttu-id="8c80b-101">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="8c80b-101">Worksheet: Cell</span></span>

<span data-ttu-id="8c80b-p101">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="8c80b-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c80b-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c80b-104">Permissions</span></span>
<span data-ttu-id="8c80b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c80b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c80b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c80b-107">Permission type</span></span>      | <span data-ttu-id="8c80b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c80b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c80b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c80b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8c80b-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c80b-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c80b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c80b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c80b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c80b-112">Not supported.</span></span>    |
|<span data-ttu-id="8c80b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c80b-113">Application</span></span> | <span data-ttu-id="8c80b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c80b-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c80b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c80b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="8c80b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c80b-116">Request headers</span></span>
| <span data-ttu-id="8c80b-117">Имя</span><span class="sxs-lookup"><span data-stu-id="8c80b-117">Name</span></span>       | <span data-ttu-id="8c80b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="8c80b-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c80b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c80b-119">Authorization</span></span>  | <span data-ttu-id="8c80b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c80b-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8c80b-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c80b-122">Response</span></span>

<span data-ttu-id="8c80b-123">В случае успеха этот метод возвращает код отклика `200, OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8c80b-123">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c80b-124">Пример</span><span class="sxs-lookup"><span data-stu-id="8c80b-124">Example</span></span>
<span data-ttu-id="8c80b-125">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8c80b-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c80b-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c80b-126">Request</span></span>
<span data-ttu-id="8c80b-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c80b-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="8c80b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c80b-128">Response</span></span>
<span data-ttu-id="8c80b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8c80b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
