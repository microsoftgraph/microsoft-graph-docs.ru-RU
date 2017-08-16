# <a name="create-rangeborder"></a><span data-ttu-id="45bb3-101">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="45bb3-101">Create RangeBorder</span></span>

<span data-ttu-id="45bb3-102">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="45bb3-102">Use this API to create a new RangeBorder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45bb3-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="45bb3-103">Prerequisites</span></span>
<span data-ttu-id="45bb3-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="45bb3-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="45bb3-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="45bb3-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="45bb3-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45bb3-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(<address>)/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="45bb3-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45bb3-107">Request headers</span></span>
| <span data-ttu-id="45bb3-108">Имя</span><span class="sxs-lookup"><span data-stu-id="45bb3-108">Name</span></span>       | <span data-ttu-id="45bb3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="45bb3-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="45bb3-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45bb3-110">Authorization</span></span>  | <span data-ttu-id="45bb3-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45bb3-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="45bb3-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45bb3-113">Request body</span></span>
<span data-ttu-id="45bb3-114">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45bb3-114">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="45bb3-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="45bb3-115">Response</span></span>

<span data-ttu-id="45bb3-116">В случае успеха этот метод возвращает код отклика `201, Created` и объект [RangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45bb3-116">If successful, this method returns `201, Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45bb3-117">Пример</span><span class="sxs-lookup"><span data-stu-id="45bb3-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45bb3-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="45bb3-118">Request</span></span>
<span data-ttu-id="45bb3-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45bb3-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
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
<span data-ttu-id="45bb3-120">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45bb3-120">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="45bb3-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="45bb3-121">Response</span></span>
<span data-ttu-id="45bb3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45bb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->