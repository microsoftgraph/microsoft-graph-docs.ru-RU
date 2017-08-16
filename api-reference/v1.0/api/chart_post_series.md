# <a name="create-chartseries"></a><span data-ttu-id="89912-101">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="89912-101">Create ChartSeries</span></span>

<span data-ttu-id="89912-102">С помощью этого API можно создать объект ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="89912-102">Use this API to create a new ChartSeries.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89912-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="89912-103">Prerequisites</span></span>
<span data-ttu-id="89912-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="89912-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="89912-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="89912-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="89912-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89912-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="89912-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89912-107">Request headers</span></span>
| <span data-ttu-id="89912-108">Имя</span><span class="sxs-lookup"><span data-stu-id="89912-108">Name</span></span>       | <span data-ttu-id="89912-109">Описание</span><span class="sxs-lookup"><span data-stu-id="89912-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89912-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89912-110">Authorization</span></span>  | <span data-ttu-id="89912-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89912-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="89912-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89912-113">Request body</span></span>
<span data-ttu-id="89912-114">Предоставьте в тексте запроса описание объекта [ChartSeries](../resources/chartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89912-114">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="89912-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="89912-115">Response</span></span>

<span data-ttu-id="89912-116">В случае успеха этот метод возвращает код отклика `201, Created` и объект [ChartSeries](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89912-116">If successful, this method returns `201, Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89912-117">Пример</span><span class="sxs-lookup"><span data-stu-id="89912-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89912-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="89912-118">Request</span></span>
<span data-ttu-id="89912-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89912-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="89912-120">Предоставьте в тексте запроса описание объекта [ChartSeries](../resources/chartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89912-120">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="89912-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="89912-121">Response</span></span>
<span data-ttu-id="89912-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="89912-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->