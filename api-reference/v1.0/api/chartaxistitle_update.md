# <a name="update-chartaxistitle"></a><span data-ttu-id="9388d-101">Обновление объекта chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="9388d-101">Update chartaxistitle</span></span>

<span data-ttu-id="9388d-102">Обновление свойств объекта chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="9388d-102">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9388d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9388d-103">Permissions</span></span>
<span data-ttu-id="9388d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9388d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9388d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9388d-106">Permission type</span></span>      | <span data-ttu-id="9388d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9388d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9388d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9388d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9388d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9388d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9388d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9388d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9388d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9388d-111">Not supported.</span></span>    |
|<span data-ttu-id="9388d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9388d-112">Application</span></span> | <span data-ttu-id="9388d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9388d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9388d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9388d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="9388d-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9388d-115">Optional request headers</span></span>
| <span data-ttu-id="9388d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="9388d-116">Name</span></span>       | <span data-ttu-id="9388d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9388d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9388d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9388d-118">Authorization</span></span>  | <span data-ttu-id="9388d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9388d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9388d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9388d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="9388d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9388d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9388d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9388d-124">Request body</span></span>
<span data-ttu-id="9388d-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9388d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9388d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9388d-128">Property</span></span>     | <span data-ttu-id="9388d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9388d-129">Type</span></span>   |<span data-ttu-id="9388d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9388d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9388d-131">text</span><span class="sxs-lookup"><span data-stu-id="9388d-131">text</span></span>|<span data-ttu-id="9388d-132">строка</span><span class="sxs-lookup"><span data-stu-id="9388d-132">string</span></span>|<span data-ttu-id="9388d-133">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="9388d-133">Represents the axis title.</span></span>|
|<span data-ttu-id="9388d-134">видимый</span><span class="sxs-lookup"><span data-stu-id="9388d-134">visible</span></span>|<span data-ttu-id="9388d-135">логический</span><span class="sxs-lookup"><span data-stu-id="9388d-135">boolean</span></span>|<span data-ttu-id="9388d-136">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="9388d-136">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="9388d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="9388d-137">Response</span></span>

<span data-ttu-id="9388d-138">В случае успеха, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookChartAxisTitle](../resources/chartaxistitle.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9388d-138">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9388d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9388d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9388d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9388d-140">Request</span></span>
<span data-ttu-id="9388d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9388d-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="9388d-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="9388d-142">Response</span></span>
<span data-ttu-id="9388d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9388d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->