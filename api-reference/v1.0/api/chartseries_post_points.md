# <a name="create-chartpoints"></a><span data-ttu-id="5a338-101">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="5a338-101">Create ChartPoints</span></span>

<span data-ttu-id="5a338-102">С помощью этого API можно создать объект ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="5a338-102">Use this API to create a new ChartPoints.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a338-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="5a338-103">Prerequisites</span></span>
<span data-ttu-id="5a338-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="5a338-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="5a338-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="5a338-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="5a338-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a338-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="5a338-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a338-107">Request headers</span></span>
| <span data-ttu-id="5a338-108">Имя</span><span class="sxs-lookup"><span data-stu-id="5a338-108">Name</span></span>       | <span data-ttu-id="5a338-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5a338-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5a338-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a338-110">Authorization</span></span>  | <span data-ttu-id="5a338-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a338-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5a338-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a338-113">Request body</span></span>
<span data-ttu-id="5a338-114">Предоставьте в тексте запроса описание объекта [ChartPoints](../resources/chartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a338-114">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5a338-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a338-115">Response</span></span>

<span data-ttu-id="5a338-116">В случае успеха этот метод возвращает код отклика `201, Created` и объект [ChartPoints](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a338-116">If successful, this method returns `201, Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a338-117">Пример</span><span class="sxs-lookup"><span data-stu-id="5a338-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a338-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a338-118">Request</span></span>
<span data-ttu-id="5a338-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a338-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="5a338-120">Предоставьте в тексте запроса описание объекта [ChartPoints](../resources/chartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a338-120">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5a338-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a338-121">Response</span></span>
<span data-ttu-id="5a338-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5a338-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->