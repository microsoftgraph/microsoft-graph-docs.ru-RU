# <a name="update-chartdatalabels"></a><span data-ttu-id="3d6ba-101">Обновление объекта chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="3d6ba-101">Update chartdatalabels</span></span>

<span data-ttu-id="3d6ba-102">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-102">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d6ba-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d6ba-103">Permissions</span></span>
<span data-ttu-id="3d6ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d6ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3d6ba-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d6ba-106">Permission type</span></span>      | <span data-ttu-id="3d6ba-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d6ba-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d6ba-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d6ba-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3d6ba-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d6ba-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3d6ba-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d6ba-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d6ba-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-111">Not supported.</span></span>    |
|<span data-ttu-id="3d6ba-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d6ba-112">Application</span></span> | <span data-ttu-id="3d6ba-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d6ba-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d6ba-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="3d6ba-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d6ba-115">Optional request headers</span></span>
| <span data-ttu-id="3d6ba-116">Имя</span><span class="sxs-lookup"><span data-stu-id="3d6ba-116">Name</span></span>       | <span data-ttu-id="3d6ba-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3d6ba-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3d6ba-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d6ba-118">Authorization</span></span>  | <span data-ttu-id="3d6ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d6ba-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d6ba-121">Request body</span></span>
<span data-ttu-id="3d6ba-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3d6ba-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d6ba-125">Property</span></span>     | <span data-ttu-id="3d6ba-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3d6ba-126">Type</span></span>   |<span data-ttu-id="3d6ba-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3d6ba-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d6ba-128">position</span><span class="sxs-lookup"><span data-stu-id="3d6ba-128">position</span></span>|<span data-ttu-id="3d6ba-129">string</span><span class="sxs-lookup"><span data-stu-id="3d6ba-129">string</span></span>|<span data-ttu-id="3d6ba-p104">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-p104">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="3d6ba-132">разделитель</span><span class="sxs-lookup"><span data-stu-id="3d6ba-132">separator</span></span>|<span data-ttu-id="3d6ba-133">string</span><span class="sxs-lookup"><span data-stu-id="3d6ba-133">string</span></span>|<span data-ttu-id="3d6ba-134">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-134">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="3d6ba-135">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="3d6ba-135">showBubbleSize</span></span>|<span data-ttu-id="3d6ba-136">boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ba-136">boolean</span></span>|<span data-ttu-id="3d6ba-137">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-137">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="3d6ba-138">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="3d6ba-138">showCategoryName</span></span>|<span data-ttu-id="3d6ba-139">boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ba-139">boolean</span></span>|<span data-ttu-id="3d6ba-140">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-140">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="3d6ba-141">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="3d6ba-141">showLegendKey</span></span>|<span data-ttu-id="3d6ba-142">boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ba-142">boolean</span></span>|<span data-ttu-id="3d6ba-143">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-143">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="3d6ba-144">showPercentage</span><span class="sxs-lookup"><span data-stu-id="3d6ba-144">showPercentage</span></span>|<span data-ttu-id="3d6ba-145">boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ba-145">boolean</span></span>|<span data-ttu-id="3d6ba-146">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-146">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="3d6ba-147">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="3d6ba-147">showSeriesName</span></span>|<span data-ttu-id="3d6ba-148">boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ba-148">boolean</span></span>|<span data-ttu-id="3d6ba-149">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-149">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="3d6ba-150">showValue</span><span class="sxs-lookup"><span data-stu-id="3d6ba-150">showValue</span></span>|<span data-ttu-id="3d6ba-151">boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ba-151">boolean</span></span>|<span data-ttu-id="3d6ba-152">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-152">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="3d6ba-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d6ba-153">Response</span></span>

<span data-ttu-id="3d6ba-154">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartDataLabels](../resources/chartdatalabels.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-154">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d6ba-155">Пример</span><span class="sxs-lookup"><span data-stu-id="3d6ba-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d6ba-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d6ba-156">Request</span></span>
<span data-ttu-id="3d6ba-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-157">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3d6ba-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d6ba-158">Response</span></span>
<span data-ttu-id="3d6ba-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3d6ba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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