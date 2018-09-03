# <a name="rangesort-apply"></a><span data-ttu-id="4a071-101">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="4a071-101">RangeSort: apply</span></span>

<span data-ttu-id="4a071-102">Выполнение операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="4a071-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a071-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a071-103">Permissions</span></span>
<span data-ttu-id="4a071-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a071-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a071-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a071-106">Permission type</span></span>      | <span data-ttu-id="4a071-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a071-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a071-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a071-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4a071-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a071-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a071-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a071-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a071-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a071-111">Not supported.</span></span>    |
|<span data-ttu-id="4a071-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a071-112">Application</span></span> | <span data-ttu-id="4a071-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a071-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a071-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a071-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="4a071-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a071-115">Request headers</span></span>
| <span data-ttu-id="4a071-116">Имя</span><span class="sxs-lookup"><span data-stu-id="4a071-116">Name</span></span>       | <span data-ttu-id="4a071-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4a071-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a071-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a071-118">Authorization</span></span>  | <span data-ttu-id="4a071-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a071-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a071-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4a071-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="4a071-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4a071-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a071-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a071-124">Request body</span></span>
<span data-ttu-id="4a071-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4a071-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a071-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="4a071-126">Parameter</span></span>    | <span data-ttu-id="4a071-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4a071-127">Type</span></span>   |<span data-ttu-id="4a071-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4a071-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a071-129">fields</span><span class="sxs-lookup"><span data-stu-id="4a071-129">fields</span></span>|<span data-ttu-id="4a071-130">Коллекция WorkbookSortField</span><span class="sxs-lookup"><span data-stu-id="4a071-130">WorkbookSortField collection</span></span>|<span data-ttu-id="4a071-131">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="4a071-131">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="4a071-132">matchCase</span><span class="sxs-lookup"><span data-stu-id="4a071-132">matchCase</span></span>|<span data-ttu-id="4a071-133">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4a071-133">boolean</span></span>|<span data-ttu-id="4a071-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="4a071-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="4a071-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="4a071-136">hasHeaders</span></span>|<span data-ttu-id="4a071-137">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="4a071-137">boolean</span></span>|<span data-ttu-id="4a071-p105">Необязательный параметр. Указывает, есть ли у диапазона заголовок.</span><span class="sxs-lookup"><span data-stu-id="4a071-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="4a071-140">orientation</span><span class="sxs-lookup"><span data-stu-id="4a071-140">orientation</span></span>|<span data-ttu-id="4a071-141">string (строка)</span><span class="sxs-lookup"><span data-stu-id="4a071-141">string</span></span>|<span data-ttu-id="4a071-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a071-142">Optional.</span></span> <span data-ttu-id="4a071-143">Указывает направление сортировки: по строкам или по столбцам.</span><span class="sxs-lookup"><span data-stu-id="4a071-143">Optional. Whether the operation is sorting rows or columns.  Possible values are: , .</span></span>  <span data-ttu-id="4a071-144">Возможные значения: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="4a071-144">The possible values are:</span></span>|
|<span data-ttu-id="4a071-145">method</span><span class="sxs-lookup"><span data-stu-id="4a071-145">method</span></span>|<span data-ttu-id="4a071-146">string (строка)</span><span class="sxs-lookup"><span data-stu-id="4a071-146">string</span></span>|<span data-ttu-id="4a071-147">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a071-147">Optional.</span></span> <span data-ttu-id="4a071-148">Метод сортировки, используемый для китайских символов.</span><span class="sxs-lookup"><span data-stu-id="4a071-148">Optional. The ordering method used for Chinese characters.  Possible values are: , .</span></span>  <span data-ttu-id="4a071-149">Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="4a071-149">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="4a071-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a071-150">Response</span></span>

<span data-ttu-id="4a071-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4a071-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a071-153">Пример</span><span class="sxs-lookup"><span data-stu-id="4a071-153">Example</span></span>
<span data-ttu-id="4a071-154">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4a071-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4a071-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a071-155">Request</span></span>
<span data-ttu-id="4a071-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a071-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
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

##### <a name="response"></a><span data-ttu-id="4a071-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a071-157">Response</span></span>
<span data-ttu-id="4a071-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a071-158">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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