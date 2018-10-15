# <a name="chartcollection-add"></a><span data-ttu-id="daafe-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="daafe-101">ChartCollection: add</span></span>

<span data-ttu-id="daafe-102">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="daafe-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="daafe-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="daafe-103">Permissions</span></span>
<span data-ttu-id="daafe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="daafe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="daafe-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="daafe-106">Permission type</span></span>      | <span data-ttu-id="daafe-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="daafe-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="daafe-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="daafe-108">Delegated (work or school account)</span></span> | <span data-ttu-id="daafe-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="daafe-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="daafe-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="daafe-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daafe-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daafe-111">Not supported.</span></span>    |
|<span data-ttu-id="daafe-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="daafe-112">Application</span></span> | <span data-ttu-id="daafe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daafe-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="daafe-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="daafe-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="daafe-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="daafe-115">Request headers</span></span>
| <span data-ttu-id="daafe-116">Имя</span><span class="sxs-lookup"><span data-stu-id="daafe-116">Name</span></span>       | <span data-ttu-id="daafe-117">Описание</span><span class="sxs-lookup"><span data-stu-id="daafe-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="daafe-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="daafe-118">Authorization</span></span>  | <span data-ttu-id="daafe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="daafe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="daafe-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="daafe-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="daafe-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="daafe-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="daafe-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="daafe-124">Request body</span></span>
<span data-ttu-id="daafe-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="daafe-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="daafe-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="daafe-126">Parameter</span></span>    | <span data-ttu-id="daafe-127">Тип</span><span class="sxs-lookup"><span data-stu-id="daafe-127">Type</span></span>   |<span data-ttu-id="daafe-128">Описание</span><span class="sxs-lookup"><span data-stu-id="daafe-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daafe-129">type</span><span class="sxs-lookup"><span data-stu-id="daafe-129">type</span></span>|<span data-ttu-id="daafe-130">string</span><span class="sxs-lookup"><span data-stu-id="daafe-130">string</span></span>|<span data-ttu-id="daafe-131">Представляет тип диаграммы.</span><span class="sxs-lookup"><span data-stu-id="daafe-131">Represents the name of a chart object.</span></span>  <span data-ttu-id="daafe-132">Возможные значения: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="daafe-132">The possible values are `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, or `PieOfPie`.</span></span>|
|<span data-ttu-id="daafe-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="daafe-133">sourceData</span></span>|<span data-ttu-id="daafe-134">Json</span><span class="sxs-lookup"><span data-stu-id="daafe-134">Json</span></span>|<span data-ttu-id="daafe-135">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="daafe-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="daafe-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="daafe-136">seriesBy</span></span>|<span data-ttu-id="daafe-137">string</span><span class="sxs-lookup"><span data-stu-id="daafe-137">string</span></span>|<span data-ttu-id="daafe-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="daafe-138">Optional.</span></span> <span data-ttu-id="daafe-139">Указывает способ, с помощью которого столбцы или строки используются в качестве рядов данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="daafe-139">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: , , .</span></span>  <span data-ttu-id="daafe-140">Возможные значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="daafe-140">The possible values are `Auto`, `Columns`, `Rows`, , , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="daafe-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="daafe-141">Response</span></span>

<span data-ttu-id="daafe-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект [WorkbookChart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="daafe-142">If successful, this method returns `200 OK` response code and [groupSetting](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daafe-143">Пример</span><span class="sxs-lookup"><span data-stu-id="daafe-143">Example</span></span>
<span data-ttu-id="daafe-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="daafe-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="daafe-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="daafe-145">Request</span></span>
<span data-ttu-id="daafe-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="daafe-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="daafe-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="daafe-147">Response</span></span>
<span data-ttu-id="daafe-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="daafe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
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
