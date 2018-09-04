# <a name="chart-image"></a><span data-ttu-id="20aa3-101">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="20aa3-101">Chart: Image</span></span>

<span data-ttu-id="20aa3-102">Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="20aa3-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="20aa3-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20aa3-103">Permissions</span></span>
<span data-ttu-id="20aa3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="20aa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="20aa3-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20aa3-106">Permission type</span></span>      | <span data-ttu-id="20aa3-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20aa3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20aa3-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20aa3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="20aa3-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20aa3-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20aa3-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20aa3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20aa3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20aa3-111">Not supported.</span></span>    |
|<span data-ttu-id="20aa3-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20aa3-112">Application</span></span> | <span data-ttu-id="20aa3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20aa3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20aa3-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20aa3-114">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="20aa3-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20aa3-115">Request headers</span></span>
| <span data-ttu-id="20aa3-116">Имя</span><span class="sxs-lookup"><span data-stu-id="20aa3-116">Name</span></span>       | <span data-ttu-id="20aa3-117">Описание</span><span class="sxs-lookup"><span data-stu-id="20aa3-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20aa3-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20aa3-118">Authorization</span></span>  | <span data-ttu-id="20aa3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20aa3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20aa3-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="20aa3-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="20aa3-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="20aa3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="20aa3-124">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="20aa3-124">Path parameters</span></span>
<span data-ttu-id="20aa3-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="20aa3-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20aa3-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="20aa3-126">Parameter</span></span>    | <span data-ttu-id="20aa3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="20aa3-127">Type</span></span>   |<span data-ttu-id="20aa3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="20aa3-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20aa3-129">height</span><span class="sxs-lookup"><span data-stu-id="20aa3-129">height</span></span>|<span data-ttu-id="20aa3-130">Int32</span><span class="sxs-lookup"><span data-stu-id="20aa3-130">Int32</span></span>|<span data-ttu-id="20aa3-131">Желаемая высота создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="20aa3-131">Optional. The desired height of the resulting image.</span></span> <span data-ttu-id="20aa3-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="20aa3-132">Optional.</span></span>|
|<span data-ttu-id="20aa3-133">width</span><span class="sxs-lookup"><span data-stu-id="20aa3-133">width</span></span>|<span data-ttu-id="20aa3-134">Int32</span><span class="sxs-lookup"><span data-stu-id="20aa3-134">Int32</span></span>|<span data-ttu-id="20aa3-135">Желаемая ширина создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="20aa3-135">Optional. The desired width of the resulting image.</span></span> <span data-ttu-id="20aa3-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="20aa3-136">Optional.</span></span>|
|<span data-ttu-id="20aa3-137">fittingMode</span><span class="sxs-lookup"><span data-stu-id="20aa3-137">fittingMode</span></span>|<span data-ttu-id="20aa3-138">строка</span><span class="sxs-lookup"><span data-stu-id="20aa3-138">string</span></span>|<span data-ttu-id="20aa3-139">Метод, используемый для масштабирования диаграммы для указанного измерения (если заданы и высота, и ширина).»</span><span class="sxs-lookup"><span data-stu-id="20aa3-139">Optional. The method used to scale the chart to the specified dimensions (if both height and width are set)."  Possible values are: , , .</span></span>  <span data-ttu-id="20aa3-140">Возможные значения: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="20aa3-140">The possible values are `Fit`, `FitAndCenter`, `Fill`, , , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="20aa3-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="20aa3-141">Response</span></span>

<span data-ttu-id="20aa3-142">В случае успеха этот метод возвращает код отклика `200 OK` и строку изображения с кодировкой base-64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20aa3-142">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20aa3-143">Пример</span><span class="sxs-lookup"><span data-stu-id="20aa3-143">Example</span></span>
<span data-ttu-id="20aa3-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="20aa3-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="20aa3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="20aa3-145">Request</span></span>
<span data-ttu-id="20aa3-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20aa3-146">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="20aa3-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="20aa3-147">Response</span></span>
<span data-ttu-id="20aa3-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="20aa3-148">Here is an example of the response.</span></span> <span data-ttu-id="20aa3-149">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="20aa3-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="20aa3-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20aa3-150">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="20aa3-151">Применение</span><span class="sxs-lookup"><span data-stu-id="20aa3-151">Usage</span></span>

<span data-ttu-id="20aa3-152">Вы можете обеспечить отображение строки Base64 в теге изображения HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="20aa3-152">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="20aa3-153">В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="20aa3-153">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="20aa3-154">Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="20aa3-154">Here is an example of a chart image returned with the default parameters.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="20aa3-156">Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки.</span><span class="sxs-lookup"><span data-stu-id="20aa3-156">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="20aa3-157">Ниже показано то же изображение диаграммы, но с такими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="20aa3-157">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
