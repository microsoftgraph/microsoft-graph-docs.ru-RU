# <a name="tablerowcollection-add"></a><span data-ttu-id="87c4e-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="87c4e-101">TableRowCollection: add</span></span>

<span data-ttu-id="87c4e-102">Добавляет новую строку в таблицу.</span><span class="sxs-lookup"><span data-stu-id="87c4e-102">Adds a new row to the table.</span></span>

## <a name="error-handling"></a><span data-ttu-id="87c4e-103">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="87c4e-103">Error Handling</span></span>

<span data-ttu-id="87c4e-104">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="87c4e-104">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="87c4e-105">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="87c4e-105">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="87c4e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87c4e-106">Permissions</span></span>
<span data-ttu-id="87c4e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87c4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87c4e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87c4e-109">Permission type</span></span>      | <span data-ttu-id="87c4e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87c4e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c4e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87c4e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87c4e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87c4e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87c4e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87c4e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87c4e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87c4e-114">Not supported.</span></span>    |
|<span data-ttu-id="87c4e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87c4e-115">Application</span></span> | <span data-ttu-id="87c4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87c4e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87c4e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87c4e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="87c4e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87c4e-118">Request headers</span></span>
| <span data-ttu-id="87c4e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="87c4e-119">Name</span></span>       | <span data-ttu-id="87c4e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="87c4e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="87c4e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87c4e-121">Authorization</span></span>  | <span data-ttu-id="87c4e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87c4e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87c4e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="87c4e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="87c4e-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="87c4e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87c4e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87c4e-127">Request body</span></span>
<span data-ttu-id="87c4e-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="87c4e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="87c4e-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="87c4e-129">Parameter</span></span>    | <span data-ttu-id="87c4e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="87c4e-130">Type</span></span>   |<span data-ttu-id="87c4e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="87c4e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87c4e-132">index</span><span class="sxs-lookup"><span data-stu-id="87c4e-132">index</span></span>|<span data-ttu-id="87c4e-133">number</span><span class="sxs-lookup"><span data-stu-id="87c4e-133">number</span></span>|<span data-ttu-id="87c4e-p105">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="87c4e-p105">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="87c4e-139">values</span><span class="sxs-lookup"><span data-stu-id="87c4e-139">values</span></span>|<span data-ttu-id="87c4e-140">(boolean, string или number)</span><span class="sxs-lookup"><span data-stu-id="87c4e-140">(boolean or string or number)</span></span>|<span data-ttu-id="87c4e-p106">Необязательный параметр. Двухмерный массив неформатированных значений строки таблицы.</span><span class="sxs-lookup"><span data-stu-id="87c4e-p106">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="87c4e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="87c4e-143">Response</span></span>

<span data-ttu-id="87c4e-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87c4e-144">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87c4e-145">Пример</span><span class="sxs-lookup"><span data-stu-id="87c4e-145">Example</span></span>
<span data-ttu-id="87c4e-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="87c4e-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87c4e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="87c4e-147">Request</span></span>
<span data-ttu-id="87c4e-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87c4e-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="87c4e-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="87c4e-149">Response</span></span>
<span data-ttu-id="87c4e-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87c4e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
  "tocPath": ""
}-->
