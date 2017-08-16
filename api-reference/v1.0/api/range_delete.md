# <a name="range-delete"></a><span data-ttu-id="af7bb-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="af7bb-101">Range: delete</span></span>

<span data-ttu-id="af7bb-102">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="af7bb-102">Deletes the cells associated with the range.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af7bb-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="af7bb-103">Prerequisites</span></span>
<span data-ttu-id="af7bb-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="af7bb-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="af7bb-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="af7bb-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="af7bb-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af7bb-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="af7bb-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af7bb-107">Request headers</span></span>
| <span data-ttu-id="af7bb-108">Имя</span><span class="sxs-lookup"><span data-stu-id="af7bb-108">Name</span></span>       | <span data-ttu-id="af7bb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="af7bb-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="af7bb-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af7bb-110">Authorization</span></span>  | <span data-ttu-id="af7bb-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af7bb-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="af7bb-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af7bb-113">Request body</span></span>
<span data-ttu-id="af7bb-114">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="af7bb-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="af7bb-115">Параметр</span><span class="sxs-lookup"><span data-stu-id="af7bb-115">Parameter</span></span>    | <span data-ttu-id="af7bb-116">Тип</span><span class="sxs-lookup"><span data-stu-id="af7bb-116">Type</span></span>   |<span data-ttu-id="af7bb-117">Описание</span><span class="sxs-lookup"><span data-stu-id="af7bb-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af7bb-118">shift</span><span class="sxs-lookup"><span data-stu-id="af7bb-118">shift</span></span>|<span data-ttu-id="af7bb-119">string</span><span class="sxs-lookup"><span data-stu-id="af7bb-119">string</span></span>|<span data-ttu-id="af7bb-p102">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="af7bb-p102">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="af7bb-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="af7bb-122">Response</span></span>

<span data-ttu-id="af7bb-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="af7bb-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af7bb-125">Пример</span><span class="sxs-lookup"><span data-stu-id="af7bb-125">Example</span></span>
<span data-ttu-id="af7bb-126">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="af7bb-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="af7bb-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="af7bb-127">Request</span></span>
<span data-ttu-id="af7bb-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af7bb-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="af7bb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="af7bb-129">Response</span></span>
<span data-ttu-id="af7bb-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="af7bb-130">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->