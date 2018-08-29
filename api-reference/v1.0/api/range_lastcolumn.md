# <a name="range-lastcolumn"></a><span data-ttu-id="a1fdc-101">Range: LastColumn</span><span class="sxs-lookup"><span data-stu-id="a1fdc-101">Range: LastColumn</span></span>

<span data-ttu-id="a1fdc-p101">Возвращает последний столбец в диапазоне. Например, последний столбец диапазона B2:D5 — D2:D5.</span><span class="sxs-lookup"><span data-stu-id="a1fdc-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="a1fdc-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1fdc-104">Permissions</span></span>
<span data-ttu-id="a1fdc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1fdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a1fdc-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1fdc-107">Permission type</span></span>      | <span data-ttu-id="a1fdc-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1fdc-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1fdc-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1fdc-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a1fdc-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1fdc-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a1fdc-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1fdc-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1fdc-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1fdc-112">Not supported.</span></span>    |
|<span data-ttu-id="a1fdc-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1fdc-113">Application</span></span> | <span data-ttu-id="a1fdc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1fdc-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1fdc-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1fdc-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastColumn

```
## <a name="request-headers"></a><span data-ttu-id="a1fdc-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1fdc-116">Request headers</span></span>
| <span data-ttu-id="a1fdc-117">Имя</span><span class="sxs-lookup"><span data-stu-id="a1fdc-117">Name</span></span>       | <span data-ttu-id="a1fdc-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a1fdc-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1fdc-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1fdc-119">Authorization</span></span>  | <span data-ttu-id="a1fdc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1fdc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1fdc-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a1fdc-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="a1fdc-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a1fdc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1fdc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1fdc-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a1fdc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1fdc-126">Response</span></span>

<span data-ttu-id="a1fdc-127">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a1fdc-127">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1fdc-128">Пример</span><span class="sxs-lookup"><span data-stu-id="a1fdc-128">Example</span></span>
<span data-ttu-id="a1fdc-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a1fdc-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a1fdc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1fdc-130">Request</span></span>
<span data-ttu-id="a1fdc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1fdc-131">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastColumn
```

##### <a name="response"></a><span data-ttu-id="a1fdc-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1fdc-132">Response</span></span>
<span data-ttu-id="a1fdc-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1fdc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->