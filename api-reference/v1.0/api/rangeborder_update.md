# <a name="update-rangeborder"></a><span data-ttu-id="c75d6-101">Обновление объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="c75d6-101">Update rangeborder</span></span>

<span data-ttu-id="c75d6-102">Обновление свойств объекта rangeborder.</span><span class="sxs-lookup"><span data-stu-id="c75d6-102">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c75d6-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c75d6-103">Permissions</span></span>
<span data-ttu-id="c75d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c75d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c75d6-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c75d6-106">Permission type</span></span>      | <span data-ttu-id="c75d6-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c75d6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c75d6-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c75d6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c75d6-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c75d6-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c75d6-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c75d6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c75d6-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c75d6-111">Not supported.</span></span>    |
|<span data-ttu-id="c75d6-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c75d6-112">Application</span></span> | <span data-ttu-id="c75d6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c75d6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c75d6-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c75d6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c75d6-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c75d6-115">Optional request headers</span></span>
| <span data-ttu-id="c75d6-116">Имя</span><span class="sxs-lookup"><span data-stu-id="c75d6-116">Name</span></span>       | <span data-ttu-id="c75d6-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c75d6-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c75d6-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c75d6-118">Authorization</span></span>  | <span data-ttu-id="c75d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c75d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c75d6-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c75d6-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="c75d6-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c75d6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c75d6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c75d6-124">Request body</span></span>
<span data-ttu-id="c75d6-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c75d6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c75d6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c75d6-128">Property</span></span>     | <span data-ttu-id="c75d6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c75d6-129">Type</span></span>   |<span data-ttu-id="c75d6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c75d6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c75d6-131">color</span><span class="sxs-lookup"><span data-stu-id="c75d6-131">color</span></span>|<span data-ttu-id="c75d6-132">строка</span><span class="sxs-lookup"><span data-stu-id="c75d6-132">string</span></span>|<span data-ttu-id="c75d6-133">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="c75d6-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="c75d6-134">style</span><span class="sxs-lookup"><span data-stu-id="c75d6-134">style</span></span>|<span data-ttu-id="c75d6-135">string (строка)</span><span class="sxs-lookup"><span data-stu-id="c75d6-135">string</span></span>|<span data-ttu-id="c75d6-136">Одна из констант типа линии, определяющая тип линии границы.</span><span class="sxs-lookup"><span data-stu-id="c75d6-136">One of the constants of line style specifying the line style for the border. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="c75d6-137">Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="c75d6-137">The possible values are `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`, , , , or .</span></span>|
|<span data-ttu-id="c75d6-138">weight</span><span class="sxs-lookup"><span data-stu-id="c75d6-138">weight</span></span>|<span data-ttu-id="c75d6-139">string (строка)</span><span class="sxs-lookup"><span data-stu-id="c75d6-139">string</span></span>|<span data-ttu-id="c75d6-140">Задает толщину границы в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="c75d6-140">Specifies the weight of the border around a range. Possible values are: , , , .</span></span> <span data-ttu-id="c75d6-141">Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="c75d6-141">The possible values are `Hairline`, `Thin`, `Medium`, `Thick`, , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="c75d6-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="c75d6-142">Response</span></span>

<span data-ttu-id="c75d6-143">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [WorkbookRangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c75d6-143">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c75d6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="c75d6-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c75d6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c75d6-145">Request</span></span>
<span data-ttu-id="c75d6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c75d6-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="c75d6-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="c75d6-147">Response</span></span>
<span data-ttu-id="c75d6-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c75d6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->