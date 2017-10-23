# <a name="chartcollection-add"></a><span data-ttu-id="c5c71-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="c5c71-101">ChartCollection: add</span></span>

<span data-ttu-id="c5c71-102">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="c5c71-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5c71-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5c71-103">Permissions</span></span>
<span data-ttu-id="c5c71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5c71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5c71-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5c71-106">Permission type</span></span>      | <span data-ttu-id="c5c71-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5c71-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5c71-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5c71-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c5c71-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5c71-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5c71-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5c71-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5c71-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c71-111">Not supported.</span></span>    |
|<span data-ttu-id="c5c71-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5c71-112">Application</span></span> | <span data-ttu-id="c5c71-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c71-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5c71-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5c71-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="c5c71-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5c71-115">Request headers</span></span>
| <span data-ttu-id="c5c71-116">Имя</span><span class="sxs-lookup"><span data-stu-id="c5c71-116">Name</span></span>       | <span data-ttu-id="c5c71-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c5c71-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5c71-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5c71-118">Authorization</span></span>  | <span data-ttu-id="c5c71-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5c71-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5c71-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5c71-121">Request body</span></span>
<span data-ttu-id="c5c71-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c5c71-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5c71-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="c5c71-123">Parameter</span></span>    | <span data-ttu-id="c5c71-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c5c71-124">Type</span></span>   |<span data-ttu-id="c5c71-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c5c71-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5c71-126">type</span><span class="sxs-lookup"><span data-stu-id="c5c71-126">type</span></span>|<span data-ttu-id="c5c71-127">string</span><span class="sxs-lookup"><span data-stu-id="c5c71-127">string</span></span>|<span data-ttu-id="c5c71-p103">Представляет тип диаграммы.  Возможные значения: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="c5c71-p103">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="c5c71-130">sourceData</span><span class="sxs-lookup"><span data-stu-id="c5c71-130">sourceData</span></span>|<span data-ttu-id="c5c71-131">string</span><span class="sxs-lookup"><span data-stu-id="c5c71-131">string</span></span>|<span data-ttu-id="c5c71-132">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="c5c71-132">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="c5c71-133">seriesBy</span><span class="sxs-lookup"><span data-stu-id="c5c71-133">seriesBy</span></span>|<span data-ttu-id="c5c71-134">string</span><span class="sxs-lookup"><span data-stu-id="c5c71-134">string</span></span>|<span data-ttu-id="c5c71-p104">Необязательный параметр. Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме.  Возможные значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="c5c71-p104">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="c5c71-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5c71-138">Response</span></span>

<span data-ttu-id="c5c71-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5c71-139">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5c71-140">Пример</span><span class="sxs-lookup"><span data-stu-id="c5c71-140">Example</span></span>
<span data-ttu-id="c5c71-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c5c71-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5c71-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5c71-142">Request</span></span>
<span data-ttu-id="c5c71-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5c71-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="c5c71-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5c71-144">Response</span></span>
<span data-ttu-id="c5c71-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5c71-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
