# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="fe72c-101">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="fe72c-101">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="fe72c-102">Возвращает столбец на основании его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="fe72c-102">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe72c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe72c-103">Permissions</span></span>
<span data-ttu-id="fe72c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe72c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe72c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe72c-106">Permission type</span></span>      | <span data-ttu-id="fe72c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe72c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe72c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe72c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fe72c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe72c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe72c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe72c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe72c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe72c-111">Not supported.</span></span>    |
|<span data-ttu-id="fe72c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe72c-112">Application</span></span> | <span data-ttu-id="fe72c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe72c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe72c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe72c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="fe72c-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe72c-115">Request headers</span></span>
| <span data-ttu-id="fe72c-116">Имя</span><span class="sxs-lookup"><span data-stu-id="fe72c-116">Name</span></span>       | <span data-ttu-id="fe72c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fe72c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fe72c-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe72c-118">Authorization</span></span>  | <span data-ttu-id="fe72c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe72c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe72c-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fe72c-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="fe72c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fe72c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe72c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe72c-124">Request body</span></span>
<span data-ttu-id="fe72c-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fe72c-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fe72c-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="fe72c-126">Parameter</span></span>    | <span data-ttu-id="fe72c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fe72c-127">Type</span></span>   |<span data-ttu-id="fe72c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fe72c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe72c-129">index</span><span class="sxs-lookup"><span data-stu-id="fe72c-129">index</span></span>|<span data-ttu-id="fe72c-130">Int32</span><span class="sxs-lookup"><span data-stu-id="fe72c-130">Int32</span></span>|<span data-ttu-id="fe72c-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="fe72c-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="fe72c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe72c-133">Response</span></span>

<span data-ttu-id="fe72c-134">В случае успеха этот метод возвращает код ответа `200 OK`  и обновленный объект [ WorkbookTableColumn](../resources/tablecolumn.md)  в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fe72c-134">If successful, this method returns `200 OK` response code and [groupSetting](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe72c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="fe72c-135">Example</span></span>
<span data-ttu-id="fe72c-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fe72c-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fe72c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe72c-137">Request</span></span>
<span data-ttu-id="fe72c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe72c-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumncollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 3
}
```

##### <a name="response"></a><span data-ttu-id="fe72c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe72c-139">Response</span></span>
<span data-ttu-id="fe72c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe72c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->