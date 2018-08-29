# <a name="chartseriescollection-itemat"></a><span data-ttu-id="e4cd4-101">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="e4cd4-101">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="e4cd4-102">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-102">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="e4cd4-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4cd4-103">Permissions</span></span>
<span data-ttu-id="e4cd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4cd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4cd4-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4cd4-106">Permission type</span></span>      | <span data-ttu-id="e4cd4-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4cd4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4cd4-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4cd4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e4cd4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4cd4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4cd4-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4cd4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4cd4-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-111">Not supported.</span></span>    |
|<span data-ttu-id="e4cd4-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4cd4-112">Application</span></span> | <span data-ttu-id="e4cd4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4cd4-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4cd4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="e4cd4-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4cd4-115">Request headers</span></span>
| <span data-ttu-id="e4cd4-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e4cd4-116">Name</span></span>       | <span data-ttu-id="e4cd4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e4cd4-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e4cd4-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4cd4-118">Authorization</span></span>  | <span data-ttu-id="e4cd4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4cd4-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e4cd4-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="e4cd4-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4cd4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4cd4-124">Request body</span></span>
<span data-ttu-id="e4cd4-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e4cd4-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="e4cd4-126">Parameter</span></span>    | <span data-ttu-id="e4cd4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e4cd4-127">Type</span></span>   |<span data-ttu-id="e4cd4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e4cd4-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4cd4-129">index</span><span class="sxs-lookup"><span data-stu-id="e4cd4-129">index</span></span>|<span data-ttu-id="e4cd4-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e4cd4-130">Int32</span></span>|<span data-ttu-id="e4cd4-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e4cd4-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4cd4-133">Response</span></span>

<span data-ttu-id="e4cd4-134">В случае успеха, этот метод возвращает`200 OK` код ответа и объект[WorkbookChartSeries](../resources/chartseries.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-134">If successful, this method returns `200 OK` response code and [groupSetting](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4cd4-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e4cd4-135">Example</span></span>
<span data-ttu-id="e4cd4-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e4cd4-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4cd4-137">Request</span></span>
<span data-ttu-id="e4cd4-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartseriescollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 2
}
```

##### <a name="response"></a><span data-ttu-id="e4cd4-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4cd4-139">Response</span></span>
<span data-ttu-id="e4cd4-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4cd4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->