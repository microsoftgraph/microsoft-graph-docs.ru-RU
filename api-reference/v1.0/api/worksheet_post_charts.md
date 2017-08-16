# <a name="create-chart"></a><span data-ttu-id="0f35c-101">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="0f35c-101">Create Chart</span></span>

<span data-ttu-id="0f35c-102">С помощью этого API можно создать объект Chart.</span><span class="sxs-lookup"><span data-stu-id="0f35c-102">Use this API to create a new Chart.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f35c-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="0f35c-103">Prerequisites</span></span>
<span data-ttu-id="0f35c-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="0f35c-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="0f35c-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="0f35c-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="0f35c-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f35c-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="0f35c-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f35c-107">Request headers</span></span>
| <span data-ttu-id="0f35c-108">Имя</span><span class="sxs-lookup"><span data-stu-id="0f35c-108">Name</span></span>       | <span data-ttu-id="0f35c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f35c-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0f35c-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f35c-110">Authorization</span></span>  | <span data-ttu-id="0f35c-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f35c-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0f35c-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f35c-113">Request body</span></span>
<span data-ttu-id="0f35c-114">Предоставьте в тексте запроса описание объекта [Chart](../resources/chart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f35c-114">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0f35c-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f35c-115">Response</span></span>

<span data-ttu-id="0f35c-116">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f35c-116">If successful, this method returns `201, Created` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f35c-117">Пример</span><span class="sxs-lookup"><span data-stu-id="0f35c-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f35c-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f35c-118">Request</span></span>
<span data-ttu-id="0f35c-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f35c-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="0f35c-120">Предоставьте в тексте запроса описание объекта [Chart](../resources/chart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f35c-120">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0f35c-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f35c-121">Response</span></span>
<span data-ttu-id="0f35c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0f35c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->