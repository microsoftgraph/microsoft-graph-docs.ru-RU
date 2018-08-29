# <a name="update-chart"></a><span data-ttu-id="d0bb8-101">Обновление диаграммы</span><span class="sxs-lookup"><span data-stu-id="d0bb8-101">Update chart</span></span>

<span data-ttu-id="d0bb8-102">Обновление свойств объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-102">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d0bb8-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0bb8-103">Permissions</span></span>
<span data-ttu-id="d0bb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0bb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0bb8-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0bb8-106">Permission type</span></span>      | <span data-ttu-id="d0bb8-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0bb8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0bb8-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0bb8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d0bb8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0bb8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d0bb8-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0bb8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0bb8-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-111">Not supported.</span></span>    |
|<span data-ttu-id="d0bb8-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0bb8-112">Application</span></span> | <span data-ttu-id="d0bb8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0bb8-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0bb8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d0bb8-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0bb8-115">Optional request headers</span></span>
| <span data-ttu-id="d0bb8-116">Имя</span><span class="sxs-lookup"><span data-stu-id="d0bb8-116">Name</span></span>       | <span data-ttu-id="d0bb8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d0bb8-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d0bb8-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0bb8-118">Authorization</span></span>  | <span data-ttu-id="d0bb8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0bb8-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d0bb8-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="d0bb8-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0bb8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0bb8-124">Request body</span></span>
<span data-ttu-id="d0bb8-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d0bb8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0bb8-128">Property</span></span>     | <span data-ttu-id="d0bb8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d0bb8-129">Type</span></span>   |<span data-ttu-id="d0bb8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d0bb8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0bb8-131">height</span><span class="sxs-lookup"><span data-stu-id="d0bb8-131">height</span></span>|<span data-ttu-id="d0bb8-132">double</span><span class="sxs-lookup"><span data-stu-id="d0bb8-132">double</span></span>|<span data-ttu-id="d0bb8-133">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="d0bb8-133">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="d0bb8-134">left</span><span class="sxs-lookup"><span data-stu-id="d0bb8-134">left</span></span>|<span data-ttu-id="d0bb8-135">double</span><span class="sxs-lookup"><span data-stu-id="d0bb8-135">double</span></span>|<span data-ttu-id="d0bb8-136">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-136">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="d0bb8-137">name</span><span class="sxs-lookup"><span data-stu-id="d0bb8-137">name</span></span>|<span data-ttu-id="d0bb8-138">строка</span><span class="sxs-lookup"><span data-stu-id="d0bb8-138">string</span></span>|<span data-ttu-id="d0bb8-139">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-139">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="d0bb8-140">top</span><span class="sxs-lookup"><span data-stu-id="d0bb8-140">top</span></span>|<span data-ttu-id="d0bb8-141">double</span><span class="sxs-lookup"><span data-stu-id="d0bb8-141">double</span></span>|<span data-ttu-id="d0bb8-142">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="d0bb8-142">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="d0bb8-143">width</span><span class="sxs-lookup"><span data-stu-id="d0bb8-143">width</span></span>|<span data-ttu-id="d0bb8-144">double</span><span class="sxs-lookup"><span data-stu-id="d0bb8-144">double</span></span>|<span data-ttu-id="d0bb8-145">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="d0bb8-145">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="d0bb8-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0bb8-146">Response</span></span>

<span data-ttu-id="d0bb8-147">В случае успеха, этот метод возвращает `200 OK`код ответа и обновленный объект [WorkbookChart](../resources/chart.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-147">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0bb8-148">Пример</span><span class="sxs-lookup"><span data-stu-id="d0bb8-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0bb8-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0bb8-149">Request</span></span>
<span data-ttu-id="d0bb8-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="d0bb8-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0bb8-151">Response</span></span>
<span data-ttu-id="d0bb8-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0bb8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->