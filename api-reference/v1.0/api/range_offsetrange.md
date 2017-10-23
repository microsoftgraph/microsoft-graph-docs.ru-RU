# <a name="range-offsetrange"></a><span data-ttu-id="75fb9-101">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="75fb9-101">Range: OffsetRange</span></span>

<span data-ttu-id="75fb9-p101">Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.</span><span class="sxs-lookup"><span data-stu-id="75fb9-p101">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="75fb9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75fb9-105">Permissions</span></span>
<span data-ttu-id="75fb9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="75fb9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75fb9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75fb9-108">Permission type</span></span>      | <span data-ttu-id="75fb9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75fb9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75fb9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75fb9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="75fb9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75fb9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75fb9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75fb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75fb9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75fb9-113">Not supported.</span></span>    |
|<span data-ttu-id="75fb9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75fb9-114">Application</span></span> | <span data-ttu-id="75fb9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75fb9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75fb9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75fb9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(<address>)/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="75fb9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75fb9-117">Request headers</span></span>
| <span data-ttu-id="75fb9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="75fb9-118">Name</span></span>       | <span data-ttu-id="75fb9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="75fb9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75fb9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75fb9-120">Authorization</span></span>  | <span data-ttu-id="75fb9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75fb9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75fb9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75fb9-123">Request body</span></span>
<span data-ttu-id="75fb9-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="75fb9-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="75fb9-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="75fb9-125">Parameter</span></span>    | <span data-ttu-id="75fb9-126">Тип</span><span class="sxs-lookup"><span data-stu-id="75fb9-126">Type</span></span>   |<span data-ttu-id="75fb9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="75fb9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75fb9-128">rowOffset</span><span class="sxs-lookup"><span data-stu-id="75fb9-128">rowOffset</span></span>|<span data-ttu-id="75fb9-129">number</span><span class="sxs-lookup"><span data-stu-id="75fb9-129">number</span></span>|<span data-ttu-id="75fb9-p104">Количество строк (положительное, отрицательное или нулевое), на которое необходимо сместить диапазон. Положительные значения соответствуют смещению вниз, а отрицательные — вверх.</span><span class="sxs-lookup"><span data-stu-id="75fb9-p104">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="75fb9-132">columnOffset</span><span class="sxs-lookup"><span data-stu-id="75fb9-132">columnOffset</span></span>|<span data-ttu-id="75fb9-133">number</span><span class="sxs-lookup"><span data-stu-id="75fb9-133">number</span></span>|<span data-ttu-id="75fb9-p105">Количество столбцов (положительное, отрицательное или 0), на который нужно сместить диапазон. Положительные значения соответствуют смещению вправо, а отрицательные — влево.</span><span class="sxs-lookup"><span data-stu-id="75fb9-p105">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="75fb9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="75fb9-136">Response</span></span>

<span data-ttu-id="75fb9-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="75fb9-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75fb9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="75fb9-138">Example</span></span>
<span data-ttu-id="75fb9-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="75fb9-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75fb9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="75fb9-140">Request</span></span>
<span data-ttu-id="75fb9-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75fb9-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="75fb9-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="75fb9-142">Response</span></span>
<span data-ttu-id="75fb9-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="75fb9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->