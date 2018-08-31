# <a name="update-chartgridlines"></a><span data-ttu-id="ee691-101">Обновление объекта chartgridlines</span><span class="sxs-lookup"><span data-stu-id="ee691-101">Update chartgridlines</span></span>

<span data-ttu-id="ee691-102">Обновление свойств объекта chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="ee691-102">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee691-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee691-103">Permissions</span></span>
<span data-ttu-id="ee691-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee691-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee691-106">Permission type</span></span>      | <span data-ttu-id="ee691-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee691-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee691-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee691-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ee691-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee691-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee691-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee691-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee691-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee691-111">Not supported.</span></span>    |
|<span data-ttu-id="ee691-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee691-112">Application</span></span> | <span data-ttu-id="ee691-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee691-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee691-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee691-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
```
## <a name="request-headers"></a><span data-ttu-id="ee691-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee691-115">Request headers</span></span>
| <span data-ttu-id="ee691-116">Имя</span><span class="sxs-lookup"><span data-stu-id="ee691-116">Name</span></span>       | <span data-ttu-id="ee691-117">Описание</span><span class="sxs-lookup"><span data-stu-id="ee691-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ee691-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee691-118">Authorization</span></span>  | <span data-ttu-id="ee691-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee691-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee691-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ee691-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="ee691-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ee691-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee691-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee691-124">Request body</span></span>
<span data-ttu-id="ee691-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ee691-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ee691-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee691-128">Property</span></span>     | <span data-ttu-id="ee691-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ee691-129">Type</span></span>   |<span data-ttu-id="ee691-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ee691-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee691-131">visible</span><span class="sxs-lookup"><span data-stu-id="ee691-131">visible</span></span>|<span data-ttu-id="ee691-132">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="ee691-132">boolean</span></span>|<span data-ttu-id="ee691-133">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="ee691-133">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="ee691-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee691-134">Response</span></span>

<span data-ttu-id="ee691-135">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [WorkbookChartGridlines](../resources/chartgridlines.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee691-135">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee691-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ee691-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee691-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee691-137">Request</span></span>
<span data-ttu-id="ee691-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee691-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="ee691-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee691-139">Response</span></span>
<span data-ttu-id="ee691-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee691-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->