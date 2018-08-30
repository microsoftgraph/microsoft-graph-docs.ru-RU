# <a name="update-charttitle"></a><span data-ttu-id="3d93a-101">Обновление объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="3d93a-101">Update charttitle</span></span>

<span data-ttu-id="3d93a-102">Обновление свойств объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="3d93a-102">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d93a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d93a-103">Permissions</span></span>
<span data-ttu-id="3d93a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d93a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3d93a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d93a-106">Permission type</span></span>      | <span data-ttu-id="3d93a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d93a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d93a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d93a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3d93a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d93a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3d93a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d93a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d93a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d93a-111">Not supported.</span></span>    |
|<span data-ttu-id="3d93a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d93a-112">Application</span></span> | <span data-ttu-id="3d93a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d93a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d93a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d93a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="3d93a-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d93a-115">Optional request headers</span></span>
| <span data-ttu-id="3d93a-116">Имя</span><span class="sxs-lookup"><span data-stu-id="3d93a-116">Name</span></span>       | <span data-ttu-id="3d93a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3d93a-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3d93a-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d93a-118">Authorization</span></span>  | <span data-ttu-id="3d93a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d93a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d93a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3d93a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3d93a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3d93a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d93a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d93a-124">Request body</span></span>
<span data-ttu-id="3d93a-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3d93a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3d93a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d93a-128">Property</span></span>     | <span data-ttu-id="3d93a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3d93a-129">Type</span></span>   |<span data-ttu-id="3d93a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3d93a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d93a-131">overlay</span><span class="sxs-lookup"><span data-stu-id="3d93a-131">overlay</span></span>|<span data-ttu-id="3d93a-132">логический</span><span class="sxs-lookup"><span data-stu-id="3d93a-132">boolean</span></span>|<span data-ttu-id="3d93a-133">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="3d93a-133">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="3d93a-134">text</span><span class="sxs-lookup"><span data-stu-id="3d93a-134">text</span></span>|<span data-ttu-id="3d93a-135">строка</span><span class="sxs-lookup"><span data-stu-id="3d93a-135">string</span></span>|<span data-ttu-id="3d93a-136">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3d93a-136">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="3d93a-137">visible</span><span class="sxs-lookup"><span data-stu-id="3d93a-137">visible</span></span>|<span data-ttu-id="3d93a-138">логический</span><span class="sxs-lookup"><span data-stu-id="3d93a-138">boolean</span></span>|<span data-ttu-id="3d93a-139">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3d93a-139">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="3d93a-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d93a-140">Response</span></span>

<span data-ttu-id="3d93a-141">В случае успеха этот метод возвращает `200 OK`код ответа и обновленный объект[WorkbookChartTitle](../resources/charttitle.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3d93a-141">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d93a-142">Пример</span><span class="sxs-lookup"><span data-stu-id="3d93a-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d93a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d93a-143">Request</span></span>
<span data-ttu-id="3d93a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d93a-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="3d93a-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d93a-145">Response</span></span>
<span data-ttu-id="3d93a-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d93a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->