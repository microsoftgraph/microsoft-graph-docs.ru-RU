# <a name="rangesort-apply"></a><span data-ttu-id="fa244-101">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="fa244-101">RangeSort: apply</span></span>

<span data-ttu-id="fa244-102">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="fa244-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa244-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="fa244-103">Prerequisites</span></span>
<span data-ttu-id="fa244-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="fa244-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="fa244-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="fa244-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="fa244-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa244-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(<address>)/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="fa244-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa244-107">Request headers</span></span>
| <span data-ttu-id="fa244-108">Имя</span><span class="sxs-lookup"><span data-stu-id="fa244-108">Name</span></span>       | <span data-ttu-id="fa244-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fa244-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa244-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa244-110">Authorization</span></span>  | <span data-ttu-id="fa244-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa244-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="fa244-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa244-113">Request body</span></span>
<span data-ttu-id="fa244-114">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fa244-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa244-115">Параметр</span><span class="sxs-lookup"><span data-stu-id="fa244-115">Parameter</span></span>    | <span data-ttu-id="fa244-116">Тип</span><span class="sxs-lookup"><span data-stu-id="fa244-116">Type</span></span>   |<span data-ttu-id="fa244-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fa244-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa244-118">fields</span><span class="sxs-lookup"><span data-stu-id="fa244-118">fields</span></span>|<span data-ttu-id="fa244-119">SortField</span><span class="sxs-lookup"><span data-stu-id="fa244-119">SortField</span></span>|<span data-ttu-id="fa244-120">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="fa244-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="fa244-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="fa244-121">matchCase</span></span>|<span data-ttu-id="fa244-122">boolean</span><span class="sxs-lookup"><span data-stu-id="fa244-122">boolean</span></span>|<span data-ttu-id="fa244-p102">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="fa244-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="fa244-125">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="fa244-125">hasHeaders</span></span>|<span data-ttu-id="fa244-126">boolean</span><span class="sxs-lookup"><span data-stu-id="fa244-126">boolean</span></span>|<span data-ttu-id="fa244-p103">Необязательный параметр. Указывает, есть ли у диапазона заголовок.</span><span class="sxs-lookup"><span data-stu-id="fa244-p103">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="fa244-129">orientation</span><span class="sxs-lookup"><span data-stu-id="fa244-129">orientation</span></span>|<span data-ttu-id="fa244-130">string</span><span class="sxs-lookup"><span data-stu-id="fa244-130">string</span></span>|<span data-ttu-id="fa244-p104">Необязательный параметр. Указывает направление сортировки: по строкам или по столбцам.  Возможные значения: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="fa244-p104">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="fa244-134">method</span><span class="sxs-lookup"><span data-stu-id="fa244-134">method</span></span>|<span data-ttu-id="fa244-135">string</span><span class="sxs-lookup"><span data-stu-id="fa244-135">string</span></span>|<span data-ttu-id="fa244-p105">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="fa244-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="fa244-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa244-139">Response</span></span>

<span data-ttu-id="fa244-p106">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fa244-p106">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa244-142">Пример</span><span class="sxs-lookup"><span data-stu-id="fa244-142">Example</span></span>
<span data-ttu-id="fa244-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fa244-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa244-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa244-144">Request</span></span>
<span data-ttu-id="fa244-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa244-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="fa244-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa244-146">Response</span></span>
<span data-ttu-id="fa244-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fa244-147">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->