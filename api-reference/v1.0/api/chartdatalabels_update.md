# <a name="update-chartdatalabels"></a><span data-ttu-id="c3fb9-101">Обновление объекта chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="c3fb9-101">Update chartdatalabels</span></span>

<span data-ttu-id="c3fb9-102">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-102">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3fb9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3fb9-103">Permissions</span></span>
<span data-ttu-id="c3fb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c3fb9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3fb9-106">Permission type</span></span>      | <span data-ttu-id="c3fb9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3fb9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3fb9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3fb9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c3fb9-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3fb9-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c3fb9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3fb9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3fb9-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-111">Not supported.</span></span>    |
|<span data-ttu-id="c3fb9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3fb9-112">Application</span></span> | <span data-ttu-id="c3fb9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3fb9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3fb9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="c3fb9-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3fb9-115">Optional request headers</span></span>
| <span data-ttu-id="c3fb9-116">Имя</span><span class="sxs-lookup"><span data-stu-id="c3fb9-116">Name</span></span>       | <span data-ttu-id="c3fb9-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c3fb9-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c3fb9-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3fb9-118">Authorization</span></span>  | <span data-ttu-id="c3fb9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3fb9-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c3fb9-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="c3fb9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3fb9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3fb9-124">Request body</span></span>
<span data-ttu-id="c3fb9-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c3fb9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3fb9-128">Property</span></span>     | <span data-ttu-id="c3fb9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c3fb9-129">Type</span></span>   |<span data-ttu-id="c3fb9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c3fb9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3fb9-131">position</span><span class="sxs-lookup"><span data-stu-id="c3fb9-131">position</span></span>|<span data-ttu-id="c3fb9-132">string</span><span class="sxs-lookup"><span data-stu-id="c3fb9-132">string</span></span>|<span data-ttu-id="c3fb9-p105">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="c3fb9-135">разделитель</span><span class="sxs-lookup"><span data-stu-id="c3fb9-135">separator</span></span>|<span data-ttu-id="c3fb9-136">string</span><span class="sxs-lookup"><span data-stu-id="c3fb9-136">string</span></span>|<span data-ttu-id="c3fb9-137">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-137">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="c3fb9-138">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="c3fb9-138">showBubbleSize</span></span>|<span data-ttu-id="c3fb9-139">boolean</span><span class="sxs-lookup"><span data-stu-id="c3fb9-139">boolean</span></span>|<span data-ttu-id="c3fb9-140">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-140">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="c3fb9-141">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="c3fb9-141">showCategoryName</span></span>|<span data-ttu-id="c3fb9-142">boolean</span><span class="sxs-lookup"><span data-stu-id="c3fb9-142">boolean</span></span>|<span data-ttu-id="c3fb9-143">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-143">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="c3fb9-144">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="c3fb9-144">showLegendKey</span></span>|<span data-ttu-id="c3fb9-145">boolean</span><span class="sxs-lookup"><span data-stu-id="c3fb9-145">boolean</span></span>|<span data-ttu-id="c3fb9-146">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-146">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="c3fb9-147">showPercentage</span><span class="sxs-lookup"><span data-stu-id="c3fb9-147">showPercentage</span></span>|<span data-ttu-id="c3fb9-148">boolean</span><span class="sxs-lookup"><span data-stu-id="c3fb9-148">boolean</span></span>|<span data-ttu-id="c3fb9-149">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-149">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="c3fb9-150">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="c3fb9-150">showSeriesName</span></span>|<span data-ttu-id="c3fb9-151">boolean</span><span class="sxs-lookup"><span data-stu-id="c3fb9-151">boolean</span></span>|<span data-ttu-id="c3fb9-152">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-152">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="c3fb9-153">showValue</span><span class="sxs-lookup"><span data-stu-id="c3fb9-153">showValue</span></span>|<span data-ttu-id="c3fb9-154">boolean</span><span class="sxs-lookup"><span data-stu-id="c3fb9-154">boolean</span></span>|<span data-ttu-id="c3fb9-155">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-155">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="c3fb9-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3fb9-156">Response</span></span>

<span data-ttu-id="c3fb9-157">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartDataLabels](../resources/chartdatalabels.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-157">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3fb9-158">Пример</span><span class="sxs-lookup"><span data-stu-id="c3fb9-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3fb9-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3fb9-159">Request</span></span>
<span data-ttu-id="c3fb9-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
##### <a name="response"></a><span data-ttu-id="c3fb9-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3fb9-161">Response</span></span>
<span data-ttu-id="c3fb9-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c3fb9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->