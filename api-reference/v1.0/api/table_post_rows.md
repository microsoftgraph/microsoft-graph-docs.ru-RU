# <a name="create-tablerow"></a><span data-ttu-id="c03f0-101">Создание объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="c03f0-101">Create TableRow</span></span>

<span data-ttu-id="c03f0-102">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="c03f0-102">Adds a row to the end of the table.</span></span> <span data-ttu-id="c03f0-103">Обратите внимание, что API может принимать несколько строк данных, использующих его.</span><span class="sxs-lookup"><span data-stu-id="c03f0-103">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="c03f0-104">Добавление одной строки за один раз может привести к замедлению.</span><span class="sxs-lookup"><span data-stu-id="c03f0-104">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="c03f0-105">Рекомендуемым подходом было бы собрать строки вместе в один вызов, а не выполнять вставку единичных строк.</span><span class="sxs-lookup"><span data-stu-id="c03f0-105">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="c03f0-106">Для достижения наилучших результатов соберите строки, которые требуется вставить, на стороне приложения и выполните одну операцию по добавлению строк.</span><span class="sxs-lookup"><span data-stu-id="c03f0-106">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="c03f0-107">Поэкспериментируйте с количеством строк, чтобы определить идеальное их число для использования в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="c03f0-107">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="c03f0-108">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="c03f0-108">Error Handling</span></span>

<span data-ttu-id="c03f0-109">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="c03f0-109">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="c03f0-110">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="c03f0-110">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="c03f0-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c03f0-111">Permissions</span></span>
<span data-ttu-id="c03f0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c03f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c03f0-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c03f0-114">Permission type</span></span>      | <span data-ttu-id="c03f0-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c03f0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c03f0-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c03f0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c03f0-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c03f0-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c03f0-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c03f0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c03f0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c03f0-119">Not supported.</span></span>    |
|<span data-ttu-id="c03f0-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c03f0-120">Application</span></span> | <span data-ttu-id="c03f0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c03f0-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c03f0-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c03f0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="c03f0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c03f0-123">Request headers</span></span>
| <span data-ttu-id="c03f0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c03f0-124">Name</span></span>       | <span data-ttu-id="c03f0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c03f0-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c03f0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c03f0-126">Authorization</span></span>  | <span data-ttu-id="c03f0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c03f0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c03f0-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c03f0-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="c03f0-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c03f0-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c03f0-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c03f0-132">Request body</span></span>
<span data-ttu-id="c03f0-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c03f0-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c03f0-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="c03f0-134">Parameter</span></span>    | <span data-ttu-id="c03f0-135">Тип</span><span class="sxs-lookup"><span data-stu-id="c03f0-135">Type</span></span>   |<span data-ttu-id="c03f0-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c03f0-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c03f0-137">index</span><span class="sxs-lookup"><span data-stu-id="c03f0-137">index</span></span>|<span data-ttu-id="c03f0-138">number</span><span class="sxs-lookup"><span data-stu-id="c03f0-138">number</span></span>|<span data-ttu-id="c03f0-p106">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="c03f0-p106">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="c03f0-144">values</span><span class="sxs-lookup"><span data-stu-id="c03f0-144">values</span></span>|<span data-ttu-id="c03f0-145">Json</span><span class="sxs-lookup"><span data-stu-id="c03f0-145">Json</span></span>|<span data-ttu-id="c03f0-146">Двумерный массив неформатированных значений строк таблицы (boolean (логический), string (строка) или number (число)).</span><span class="sxs-lookup"><span data-stu-id="c03f0-146">A 2-dimensional array of unformatted values of the table rows (boolean or string or number).</span></span>|

## <a name="response"></a><span data-ttu-id="c03f0-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="c03f0-147">Response</span></span>

<span data-ttu-id="c03f0-148">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c03f0-148">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c03f0-149">Пример</span><span class="sxs-lookup"><span data-stu-id="c03f0-149">Example</span></span>
<span data-ttu-id="c03f0-150">В этом примере в конец таблицы производится вставка двух строк данных.</span><span class="sxs-lookup"><span data-stu-id="c03f0-150">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="c03f0-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c03f0-151">Request</span></span>
<span data-ttu-id="c03f0-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c03f0-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
##### <a name="response"></a><span data-ttu-id="c03f0-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="c03f0-153">Response</span></span>
<span data-ttu-id="c03f0-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c03f0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table_post_rows.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not.",
    "Warning: /api-reference/v1.0/api/table_post_rows.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)"
  ],
  "tocPath": ""
}-->
