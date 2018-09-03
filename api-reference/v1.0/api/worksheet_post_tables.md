# <a name="create-table"></a><span data-ttu-id="13e6d-101">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="13e6d-101">Create table</span></span>

<span data-ttu-id="13e6d-102">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="13e6d-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="13e6d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13e6d-103">Permissions</span></span>
<span data-ttu-id="13e6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="13e6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="13e6d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13e6d-106">Permission type</span></span>      | <span data-ttu-id="13e6d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13e6d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13e6d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13e6d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="13e6d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13e6d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="13e6d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13e6d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13e6d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13e6d-111">Not supported.</span></span>    |
|<span data-ttu-id="13e6d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13e6d-112">Application</span></span> | <span data-ttu-id="13e6d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13e6d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13e6d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13e6d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="13e6d-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13e6d-115">Request headers</span></span>
| <span data-ttu-id="13e6d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="13e6d-116">Name</span></span>       | <span data-ttu-id="13e6d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="13e6d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="13e6d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13e6d-118">Authorization</span></span>  | <span data-ttu-id="13e6d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13e6d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13e6d-121">Идентификатор сеанса работы с книгой</span><span class="sxs-lookup"><span data-stu-id="13e6d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="13e6d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="13e6d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13e6d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13e6d-124">Request body</span></span>
<span data-ttu-id="13e6d-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="13e6d-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="13e6d-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="13e6d-126">Parameter</span></span>           | <span data-ttu-id="13e6d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="13e6d-127">Type</span></span>      |<span data-ttu-id="13e6d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="13e6d-128">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="13e6d-129">Адрес</span><span class="sxs-lookup"><span data-stu-id="13e6d-129">Address</span></span>  | <span data-ttu-id="13e6d-130">string</span><span class="sxs-lookup"><span data-stu-id="13e6d-130">string</span></span>| <span data-ttu-id="13e6d-p104">Адрес диапазона. При вызове этого API из пути `worksheets/{id or name}/tables/add` не нужно указывать префикс имя листа в адресе. Однако при вызове этого API из пути `workbook/tables/add` нужно указать имя листа, на котором требуется создать таблицу (например: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="13e6d-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="13e6d-134">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="13e6d-134">hasHeaders</span></span>  | <span data-ttu-id="13e6d-135">boolean</span><span class="sxs-lookup"><span data-stu-id="13e6d-135">boolean</span></span>|<span data-ttu-id="13e6d-p105">Логическое значение, указывающее, имеет ли диапазон метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="13e6d-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="13e6d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="13e6d-139">Response</span></span>

<span data-ttu-id="13e6d-140">В случае успеха этот метод возвращает `201 Created` код отклика и объект [WorkbookTable](../resources/table.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="13e6d-140">If successful, this method returns `201 Created` response code and [groupSetting](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13e6d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="13e6d-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13e6d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="13e6d-142">Request</span></span>
<span data-ttu-id="13e6d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13e6d-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="13e6d-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="13e6d-144">Response</span></span>
<span data-ttu-id="13e6d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13e6d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
