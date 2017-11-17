# <a name="rangesort-apply"></a><span data-ttu-id="55fe0-101">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="55fe0-101">RangeSort: apply</span></span>

<span data-ttu-id="55fe0-102">Выполнение операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="55fe0-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="55fe0-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55fe0-103">Permissions</span></span>
<span data-ttu-id="55fe0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="55fe0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="55fe0-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55fe0-106">Permission type</span></span>      | <span data-ttu-id="55fe0-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55fe0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55fe0-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55fe0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="55fe0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55fe0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="55fe0-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55fe0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55fe0-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55fe0-111">Not supported.</span></span>    |
|<span data-ttu-id="55fe0-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55fe0-112">Application</span></span> | <span data-ttu-id="55fe0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55fe0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55fe0-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55fe0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="55fe0-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55fe0-115">Request headers</span></span>
| <span data-ttu-id="55fe0-116">Имя</span><span class="sxs-lookup"><span data-stu-id="55fe0-116">Name</span></span>       | <span data-ttu-id="55fe0-117">Описание</span><span class="sxs-lookup"><span data-stu-id="55fe0-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="55fe0-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55fe0-118">Authorization</span></span>  | <span data-ttu-id="55fe0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55fe0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55fe0-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55fe0-121">Request body</span></span>
<span data-ttu-id="55fe0-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="55fe0-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55fe0-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="55fe0-123">Parameter</span></span>    | <span data-ttu-id="55fe0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="55fe0-124">Type</span></span>   |<span data-ttu-id="55fe0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="55fe0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55fe0-126">fields</span><span class="sxs-lookup"><span data-stu-id="55fe0-126">fields</span></span>|<span data-ttu-id="55fe0-127">SortField</span><span class="sxs-lookup"><span data-stu-id="55fe0-127">SortField</span></span>|<span data-ttu-id="55fe0-128">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="55fe0-128">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="55fe0-129">matchCase</span><span class="sxs-lookup"><span data-stu-id="55fe0-129">matchCase</span></span>|<span data-ttu-id="55fe0-130">boolean</span><span class="sxs-lookup"><span data-stu-id="55fe0-130">boolean</span></span>|<span data-ttu-id="55fe0-p103">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="55fe0-p103">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="55fe0-133">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="55fe0-133">hasHeaders</span></span>|<span data-ttu-id="55fe0-134">boolean</span><span class="sxs-lookup"><span data-stu-id="55fe0-134">boolean</span></span>|<span data-ttu-id="55fe0-p104">Необязательный параметр. Указывает, есть ли у диапазона заголовок.</span><span class="sxs-lookup"><span data-stu-id="55fe0-p104">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="55fe0-137">orientation</span><span class="sxs-lookup"><span data-stu-id="55fe0-137">orientation</span></span>|<span data-ttu-id="55fe0-138">string</span><span class="sxs-lookup"><span data-stu-id="55fe0-138">string</span></span>|<span data-ttu-id="55fe0-p105">Необязательный параметр. Указывает направление сортировки: по строкам или по столбцам.  Возможные значения: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="55fe0-p105">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="55fe0-142">метод</span><span class="sxs-lookup"><span data-stu-id="55fe0-142">method</span></span>|<span data-ttu-id="55fe0-143">string</span><span class="sxs-lookup"><span data-stu-id="55fe0-143">string</span></span>|<span data-ttu-id="55fe0-p106">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="55fe0-p106">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="55fe0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="55fe0-147">Response</span></span>

<span data-ttu-id="55fe0-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="55fe0-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55fe0-150">Пример</span><span class="sxs-lookup"><span data-stu-id="55fe0-150">Example</span></span>
<span data-ttu-id="55fe0-151">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="55fe0-151">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="55fe0-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="55fe0-152">Request</span></span>
<span data-ttu-id="55fe0-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55fe0-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="55fe0-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="55fe0-154">Response</span></span>
<span data-ttu-id="55fe0-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55fe0-155">Here is an example of the response.</span></span> 
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