# <a name="create-tablerow"></a><span data-ttu-id="b2ceb-101">Создание объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="b2ceb-101">Create TableRow</span></span>

<span data-ttu-id="b2ceb-102">С помощью этого API можно создать объект TableRow.</span><span class="sxs-lookup"><span data-stu-id="b2ceb-102">Use this API to create a new TableRow.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2ceb-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="b2ceb-103">Prerequisites</span></span>
<span data-ttu-id="b2ceb-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="b2ceb-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="b2ceb-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="b2ceb-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="b2ceb-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2ceb-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows

```
## <a name="request-headers"></a><span data-ttu-id="b2ceb-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2ceb-107">Request headers</span></span>
| <span data-ttu-id="b2ceb-108">Имя</span><span class="sxs-lookup"><span data-stu-id="b2ceb-108">Name</span></span>       | <span data-ttu-id="b2ceb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2ceb-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2ceb-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2ceb-110">Authorization</span></span>  | <span data-ttu-id="b2ceb-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2ceb-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b2ceb-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2ceb-113">Request body</span></span>
<span data-ttu-id="b2ceb-114">Предоставьте в тексте запроса описание объекта [TableRow](../resources/tablerow.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2ceb-114">In the request body, supply a JSON representation of [TableRow](../resources/tablerow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b2ceb-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2ceb-115">Response</span></span>

<span data-ttu-id="b2ceb-116">В случае успеха этот метод возвращает код отклика `201, Created` и объект [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2ceb-116">If successful, this method returns `201, Created` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2ceb-117">Пример</span><span class="sxs-lookup"><span data-stu-id="b2ceb-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2ceb-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2ceb-118">Request</span></span>
<span data-ttu-id="b2ceb-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2ceb-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablerow_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="b2ceb-120">Предоставьте в тексте запроса описание объекта [TableRow](../resources/tablerow.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2ceb-120">In the request body, supply a JSON representation of [TableRow](../resources/tablerow.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b2ceb-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2ceb-121">Response</span></span>
<span data-ttu-id="b2ceb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b2ceb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->