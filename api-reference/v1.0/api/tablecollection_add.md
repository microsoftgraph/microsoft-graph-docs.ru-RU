# <a name="tablecollection-add"></a><span data-ttu-id="7c153-101">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="7c153-101">TableCollection: add</span></span>

<span data-ttu-id="7c153-p101">Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="7c153-p101">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c153-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c153-105">Permissions</span></span>
<span data-ttu-id="7c153-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c153-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c153-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c153-108">Permission type</span></span>      | <span data-ttu-id="7c153-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c153-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c153-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c153-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c153-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c153-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c153-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c153-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c153-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c153-113">Not supported.</span></span>    |
|<span data-ttu-id="7c153-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c153-114">Application</span></span> | <span data-ttu-id="7c153-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c153-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c153-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c153-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="7c153-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c153-117">Request headers</span></span>
| <span data-ttu-id="7c153-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7c153-118">Name</span></span>       | <span data-ttu-id="7c153-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7c153-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c153-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c153-120">Authorization</span></span>  | <span data-ttu-id="7c153-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c153-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c153-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c153-123">Request body</span></span>
<span data-ttu-id="7c153-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7c153-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7c153-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="7c153-125">Parameter</span></span>    | <span data-ttu-id="7c153-126">Тип</span><span class="sxs-lookup"><span data-stu-id="7c153-126">Type</span></span>   |<span data-ttu-id="7c153-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7c153-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c153-128">address</span><span class="sxs-lookup"><span data-stu-id="7c153-128">address</span></span>|<span data-ttu-id="7c153-129">string</span><span class="sxs-lookup"><span data-stu-id="7c153-129">string</span></span>|<span data-ttu-id="7c153-p104">Адрес или имя объекта range, представляющего источник данных. Если адрес не содержит имя листа, используется текущий активный лист.</span><span class="sxs-lookup"><span data-stu-id="7c153-p104">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="7c153-132">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="7c153-132">hasHeaders</span></span>|<span data-ttu-id="7c153-133">boolean</span><span class="sxs-lookup"><span data-stu-id="7c153-133">boolean</span></span>|<span data-ttu-id="7c153-p105">Логическое значение, указывающее, имеют ли импортируемые данные метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="7c153-p105">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="7c153-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c153-137">Response</span></span>

<span data-ttu-id="7c153-138">В случае успеха этот метод возвращает код отклика `200, OK` и объект [Table](../resources/table.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c153-138">If successful, this method returns `200, OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c153-139">Пример</span><span class="sxs-lookup"><span data-stu-id="7c153-139">Example</span></span>
<span data-ttu-id="7c153-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7c153-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c153-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c153-141">Request</span></span>
<span data-ttu-id="7c153-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c153-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7c153-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c153-143">Response</span></span>
<span data-ttu-id="7c153-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7c153-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
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
