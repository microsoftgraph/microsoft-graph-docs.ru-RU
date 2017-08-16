# <a name="create-tablecolumn"></a><span data-ttu-id="2e866-101">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="2e866-101">Create TableColumn</span></span>

<span data-ttu-id="2e866-102">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="2e866-102">Use this API to create a new TableColumn.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e866-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="2e866-103">Prerequisites</span></span>
<span data-ttu-id="2e866-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="2e866-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="2e866-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="2e866-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="2e866-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e866-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="2e866-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e866-107">Request headers</span></span>
| <span data-ttu-id="2e866-108">Имя</span><span class="sxs-lookup"><span data-stu-id="2e866-108">Name</span></span>       | <span data-ttu-id="2e866-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2e866-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2e866-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e866-110">Authorization</span></span>  | <span data-ttu-id="2e866-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e866-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2e866-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e866-113">Request body</span></span>
<span data-ttu-id="2e866-114">Предоставьте в тексте запроса описание объекта [TableColumn](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e866-114">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2e866-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e866-115">Response</span></span>

<span data-ttu-id="2e866-116">В случае успеха этот метод возвращает код отклика `201, Created` и объект [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e866-116">If successful, this method returns `201, Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e866-117">Пример</span><span class="sxs-lookup"><span data-stu-id="2e866-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e866-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e866-118">Request</span></span>
<span data-ttu-id="2e866-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e866-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="2e866-120">Предоставьте в тексте запроса описание объекта [TableColumn](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e866-120">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2e866-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e866-121">Response</span></span>
<span data-ttu-id="2e866-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2e866-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->