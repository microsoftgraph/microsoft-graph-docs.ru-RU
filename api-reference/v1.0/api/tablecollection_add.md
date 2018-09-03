# <a name="tablecollection-add"></a><span data-ttu-id="8b62b-101">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="8b62b-101">TableCollection: add</span></span>

<span data-ttu-id="8b62b-p101">Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="8b62b-p101">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="8b62b-105">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="8b62b-105">Error Handling</span></span>

<span data-ttu-id="8b62b-106">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="8b62b-106">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="8b62b-107">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="8b62b-107">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b62b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b62b-108">Permissions</span></span>
<span data-ttu-id="8b62b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b62b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b62b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b62b-111">Permission type</span></span>      | <span data-ttu-id="8b62b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b62b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b62b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b62b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8b62b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b62b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b62b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b62b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b62b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b62b-116">Not supported.</span></span>    |
|<span data-ttu-id="8b62b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b62b-117">Application</span></span> | <span data-ttu-id="8b62b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b62b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b62b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b62b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="8b62b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b62b-120">Request headers</span></span>
| <span data-ttu-id="8b62b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8b62b-121">Name</span></span>       | <span data-ttu-id="8b62b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8b62b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b62b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b62b-123">Authorization</span></span>  | <span data-ttu-id="8b62b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b62b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b62b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8b62b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="8b62b-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8b62b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b62b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b62b-129">Request body</span></span>
<span data-ttu-id="8b62b-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8b62b-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b62b-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="8b62b-131">Parameter</span></span>    | <span data-ttu-id="8b62b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8b62b-132">Type</span></span>   |<span data-ttu-id="8b62b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8b62b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b62b-134">address</span><span class="sxs-lookup"><span data-stu-id="8b62b-134">address</span></span>|<span data-ttu-id="8b62b-135">строка</span><span class="sxs-lookup"><span data-stu-id="8b62b-135">string</span></span>|<span data-ttu-id="8b62b-p106">Адрес или имя объекта range, представляющего источник данных. Если адрес не содержит имя листа, используется текущий активный лист.</span><span class="sxs-lookup"><span data-stu-id="8b62b-p106">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="8b62b-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="8b62b-138">hasHeaders</span></span>|<span data-ttu-id="8b62b-139">логический</span><span class="sxs-lookup"><span data-stu-id="8b62b-139">boolean</span></span>|<span data-ttu-id="8b62b-p107">Логическое значение, указывающее, имеют ли импортируемые данные метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="8b62b-p107">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="8b62b-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b62b-143">Response</span></span>

<span data-ttu-id="8b62b-144">В случае успеха, этот метод возвращает `200 OK` код ответа и объект [WorkbookTable](../resources/table.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8b62b-144">If successful, this method returns `200 OK` response code and [groupSetting](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b62b-145">Пример</span><span class="sxs-lookup"><span data-stu-id="8b62b-145">Example</span></span>
<span data-ttu-id="8b62b-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8b62b-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8b62b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b62b-147">Request</span></span>
<span data-ttu-id="8b62b-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b62b-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="8b62b-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b62b-149">Response</span></span>
<span data-ttu-id="8b62b-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b62b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
