# <a name="tablesort-apply"></a><span data-ttu-id="2fb5a-101">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="2fb5a-101">TableSort: apply</span></span>

<span data-ttu-id="2fb5a-102">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2fb5a-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="2fb5a-103">Prerequisites</span></span>
<span data-ttu-id="2fb5a-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="2fb5a-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="2fb5a-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="2fb5a-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fb5a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="2fb5a-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2fb5a-107">Request headers</span></span>
| <span data-ttu-id="2fb5a-108">Имя</span><span class="sxs-lookup"><span data-stu-id="2fb5a-108">Name</span></span>       | <span data-ttu-id="2fb5a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2fb5a-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2fb5a-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fb5a-110">Authorization</span></span>  | <span data-ttu-id="2fb5a-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2fb5a-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fb5a-113">Request body</span></span>
<span data-ttu-id="2fb5a-114">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2fb5a-115">Параметр</span><span class="sxs-lookup"><span data-stu-id="2fb5a-115">Parameter</span></span>    | <span data-ttu-id="2fb5a-116">Тип</span><span class="sxs-lookup"><span data-stu-id="2fb5a-116">Type</span></span>   |<span data-ttu-id="2fb5a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="2fb5a-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fb5a-118">fields</span><span class="sxs-lookup"><span data-stu-id="2fb5a-118">fields</span></span>|<span data-ttu-id="2fb5a-119">SortField</span><span class="sxs-lookup"><span data-stu-id="2fb5a-119">SortField</span></span>|<span data-ttu-id="2fb5a-120">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="2fb5a-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="2fb5a-121">matchCase</span></span>|<span data-ttu-id="2fb5a-122">boolean</span><span class="sxs-lookup"><span data-stu-id="2fb5a-122">boolean</span></span>|<span data-ttu-id="2fb5a-p102">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="2fb5a-125">method</span><span class="sxs-lookup"><span data-stu-id="2fb5a-125">method</span></span>|<span data-ttu-id="2fb5a-126">string</span><span class="sxs-lookup"><span data-stu-id="2fb5a-126">string</span></span>|<span data-ttu-id="2fb5a-p103">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-p103">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="2fb5a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fb5a-130">Response</span></span>

<span data-ttu-id="2fb5a-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fb5a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2fb5a-133">Example</span></span>
<span data-ttu-id="2fb5a-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2fb5a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fb5a-135">Request</span></span>
<span data-ttu-id="2fb5a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="2fb5a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fb5a-137">Response</span></span>
<span data-ttu-id="2fb5a-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2fb5a-138">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->