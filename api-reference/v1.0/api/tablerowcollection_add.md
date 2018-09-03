# <a name="tablerowcollection-add"></a><span data-ttu-id="65a04-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="65a04-101">TableRowCollection: add</span></span>

<span data-ttu-id="65a04-102">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="65a04-102">Adds a row to the end of the table.</span></span> <span data-ttu-id="65a04-103">Обратите внимание, что API может принимать несколько строк данных, использующих его.</span><span class="sxs-lookup"><span data-stu-id="65a04-103">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="65a04-104">Добавление одной строки за один раз может привести к замедлению.</span><span class="sxs-lookup"><span data-stu-id="65a04-104">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="65a04-105">Рекомендуемым подходом было бы собрать строки вместе в один вызов, а не выполнять вставку единичных строк.</span><span class="sxs-lookup"><span data-stu-id="65a04-105">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="65a04-106">Для достижения наилучших результатов соберите строки, которые требуется вставить, на стороне приложения и выполните одну операцию по добавлению строк.</span><span class="sxs-lookup"><span data-stu-id="65a04-106">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="65a04-107">Поэкспериментируйте с количеством строк, чтобы определить идеальное их число для использования в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="65a04-107">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="65a04-108">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="65a04-108">Error Handling</span></span>

<span data-ttu-id="65a04-109">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="65a04-109">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="65a04-110">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="65a04-110">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="65a04-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65a04-111">Permissions</span></span>
<span data-ttu-id="65a04-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65a04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65a04-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65a04-114">Permission type</span></span>      | <span data-ttu-id="65a04-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65a04-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65a04-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65a04-116">Delegated (work or school account)</span></span> | <span data-ttu-id="65a04-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65a04-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="65a04-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65a04-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65a04-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65a04-119">Not supported.</span></span>    |
|<span data-ttu-id="65a04-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65a04-120">Application</span></span> | <span data-ttu-id="65a04-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65a04-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65a04-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65a04-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="65a04-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65a04-123">Request headers</span></span>
| <span data-ttu-id="65a04-124">Имя</span><span class="sxs-lookup"><span data-stu-id="65a04-124">Name</span></span>       | <span data-ttu-id="65a04-125">Описание</span><span class="sxs-lookup"><span data-stu-id="65a04-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="65a04-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65a04-126">Authorization</span></span>  | <span data-ttu-id="65a04-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65a04-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65a04-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="65a04-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="65a04-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="65a04-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65a04-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65a04-132">Request body</span></span>
<span data-ttu-id="65a04-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="65a04-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="65a04-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="65a04-134">Parameter</span></span>    | <span data-ttu-id="65a04-135">Тип</span><span class="sxs-lookup"><span data-stu-id="65a04-135">Type</span></span>   |<span data-ttu-id="65a04-136">Описание</span><span class="sxs-lookup"><span data-stu-id="65a04-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65a04-137">index</span><span class="sxs-lookup"><span data-stu-id="65a04-137">index</span></span>|<span data-ttu-id="65a04-138">Int32</span><span class="sxs-lookup"><span data-stu-id="65a04-138">Int32</span></span>|<span data-ttu-id="65a04-p106">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="65a04-p106">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="65a04-144">values</span><span class="sxs-lookup"><span data-stu-id="65a04-144">values</span></span>|<span data-ttu-id="65a04-145">Json</span><span class="sxs-lookup"><span data-stu-id="65a04-145">Json</span></span>|<span data-ttu-id="65a04-p107">Необязательный параметр. Двумерный массив неформатированных значений строки таблицы.</span><span class="sxs-lookup"><span data-stu-id="65a04-p107">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="65a04-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="65a04-148">Response</span></span>

<span data-ttu-id="65a04-149">В случае успеха этот метод возвращает код отклика `200 OK` и объект [WorkbookTableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65a04-149">If successful, this method returns `200 OK` response code and [groupSetting](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65a04-150">Пример</span><span class="sxs-lookup"><span data-stu-id="65a04-150">Example</span></span>
<span data-ttu-id="65a04-151">В этом примере в конец таблицы производится вставка двух строк данных.</span><span class="sxs-lookup"><span data-stu-id="65a04-151">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="65a04-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="65a04-152">Request</span></span>
<span data-ttu-id="65a04-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65a04-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": 5,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="65a04-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="65a04-154">Response</span></span>
<span data-ttu-id="65a04-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65a04-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Warning: /api-reference/v1.0/api/tablerowcollection_add.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/tablerowcollection_add.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
