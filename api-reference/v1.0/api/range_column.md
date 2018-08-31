# <a name="range-column"></a><span data-ttu-id="60879-101">Range: Column</span><span class="sxs-lookup"><span data-stu-id="60879-101">Range: Column</span></span>

<span data-ttu-id="60879-102">Возвращает столбец в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="60879-102">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="60879-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60879-103">Permissions</span></span>
<span data-ttu-id="60879-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="60879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="60879-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60879-106">Permission type</span></span>      | <span data-ttu-id="60879-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60879-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60879-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60879-108">Delegated (work or school account)</span></span> | <span data-ttu-id="60879-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60879-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60879-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60879-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60879-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60879-111">Not supported.</span></span>    |
|<span data-ttu-id="60879-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60879-112">Application</span></span> | <span data-ttu-id="60879-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60879-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60879-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60879-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="60879-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60879-115">Request headers</span></span>
| <span data-ttu-id="60879-116">Имя</span><span class="sxs-lookup"><span data-stu-id="60879-116">Name</span></span>       | <span data-ttu-id="60879-117">Описание</span><span class="sxs-lookup"><span data-stu-id="60879-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="60879-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60879-118">Authorization</span></span>  | <span data-ttu-id="60879-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60879-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60879-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="60879-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="60879-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="60879-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="60879-124">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="60879-124">Path parameters</span></span>
<span data-ttu-id="60879-125">В пути запроса укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="60879-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60879-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="60879-126">Parameter</span></span>    | <span data-ttu-id="60879-127">Тип</span><span class="sxs-lookup"><span data-stu-id="60879-127">Type</span></span>   |<span data-ttu-id="60879-128">Описание</span><span class="sxs-lookup"><span data-stu-id="60879-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60879-129">column</span><span class="sxs-lookup"><span data-stu-id="60879-129">column</span></span>|<span data-ttu-id="60879-130">Int32</span><span class="sxs-lookup"><span data-stu-id="60879-130">Int32</span></span>|<span data-ttu-id="60879-p104">Номер столбца диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="60879-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="60879-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="60879-133">Response</span></span>

<span data-ttu-id="60879-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="60879-134">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60879-135">Пример</span><span class="sxs-lookup"><span data-stu-id="60879-135">Example</span></span>
<span data-ttu-id="60879-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="60879-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="60879-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="60879-137">Request</span></span>
<span data-ttu-id="60879-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60879-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```

##### <a name="response"></a><span data-ttu-id="60879-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="60879-139">Response</span></span>
<span data-ttu-id="60879-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60879-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->