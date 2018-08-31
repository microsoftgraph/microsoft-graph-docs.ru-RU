# <a name="update-chartlegend"></a><span data-ttu-id="12a7f-101">Обновление объекта chartlegend</span><span class="sxs-lookup"><span data-stu-id="12a7f-101">Update chartlegend</span></span>

<span data-ttu-id="12a7f-102">Обновление свойств объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="12a7f-102">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="12a7f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12a7f-103">Permissions</span></span>
<span data-ttu-id="12a7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="12a7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12a7f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12a7f-106">Permission type</span></span>      | <span data-ttu-id="12a7f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12a7f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12a7f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12a7f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="12a7f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12a7f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12a7f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12a7f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12a7f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a7f-111">Not supported.</span></span>    |
|<span data-ttu-id="12a7f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12a7f-112">Application</span></span> | <span data-ttu-id="12a7f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a7f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12a7f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12a7f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="12a7f-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12a7f-115">Optional request headers</span></span>
| <span data-ttu-id="12a7f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="12a7f-116">Name</span></span>       | <span data-ttu-id="12a7f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="12a7f-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="12a7f-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12a7f-118">Authorization</span></span>  | <span data-ttu-id="12a7f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12a7f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12a7f-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="12a7f-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="12a7f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="12a7f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12a7f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12a7f-124">Request body</span></span>
<span data-ttu-id="12a7f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="12a7f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="12a7f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="12a7f-128">Property</span></span>     | <span data-ttu-id="12a7f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="12a7f-129">Type</span></span>   |<span data-ttu-id="12a7f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="12a7f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12a7f-131">overlay</span><span class="sxs-lookup"><span data-stu-id="12a7f-131">overlay</span></span>|<span data-ttu-id="12a7f-132">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="12a7f-132">boolean</span></span>|<span data-ttu-id="12a7f-133">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="12a7f-133">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="12a7f-134">position</span><span class="sxs-lookup"><span data-stu-id="12a7f-134">position</span></span>|<span data-ttu-id="12a7f-135">string (строка)</span><span class="sxs-lookup"><span data-stu-id="12a7f-135">string</span></span>|<span data-ttu-id="12a7f-136">Представляет положение условного обозначения диаграммы.</span><span class="sxs-lookup"><span data-stu-id="12a7f-136">Represents the position of the legend on the chart. Possible values are: , , , , , .</span></span> <span data-ttu-id="12a7f-137">Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`,`Custom`.</span><span class="sxs-lookup"><span data-stu-id="12a7f-137">The possible values are `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`, , , , , , or .</span></span>|
|<span data-ttu-id="12a7f-138">visible</span><span class="sxs-lookup"><span data-stu-id="12a7f-138">visible</span></span>|<span data-ttu-id="12a7f-139">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="12a7f-139">boolean</span></span>|<span data-ttu-id="12a7f-140">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="12a7f-140">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="12a7f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="12a7f-141">Response</span></span>

<span data-ttu-id="12a7f-142">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [WorkbookChartLegend](../resources/chartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12a7f-142">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12a7f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="12a7f-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12a7f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a7f-144">Request</span></span>
<span data-ttu-id="12a7f-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a7f-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="12a7f-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="12a7f-146">Response</span></span>
<span data-ttu-id="12a7f-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12a7f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->