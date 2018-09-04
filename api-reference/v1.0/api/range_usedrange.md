# <a name="range-usedrange"></a><span data-ttu-id="967f5-101">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="967f5-101">Range: UsedRange</span></span>

<span data-ttu-id="967f5-102">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="967f5-102">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="967f5-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="967f5-103">Permissions</span></span>
<span data-ttu-id="967f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="967f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="967f5-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="967f5-106">Permission type</span></span>      | <span data-ttu-id="967f5-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="967f5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="967f5-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="967f5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="967f5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="967f5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="967f5-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="967f5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="967f5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="967f5-111">Not supported.</span></span>    |
|<span data-ttu-id="967f5-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="967f5-112">Application</span></span> | <span data-ttu-id="967f5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="967f5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="967f5-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="967f5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="967f5-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="967f5-115">Request headers</span></span>
| <span data-ttu-id="967f5-116">Имя</span><span class="sxs-lookup"><span data-stu-id="967f5-116">Name</span></span>       | <span data-ttu-id="967f5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="967f5-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="967f5-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="967f5-118">Authorization</span></span>  | <span data-ttu-id="967f5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="967f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="967f5-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="967f5-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="967f5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="967f5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="967f5-124">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="967f5-124">Path parameters</span></span>
| <span data-ttu-id="967f5-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="967f5-125">Parameter</span></span>    | <span data-ttu-id="967f5-126">Тип</span><span class="sxs-lookup"><span data-stu-id="967f5-126">Type</span></span>   |<span data-ttu-id="967f5-127">Описание</span><span class="sxs-lookup"><span data-stu-id="967f5-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="967f5-128">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="967f5-128">valuesOnly</span></span>|<span data-ttu-id="967f5-129">логический</span><span class="sxs-lookup"><span data-stu-id="967f5-129">boolean</span></span>|<span data-ttu-id="967f5-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="967f5-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="967f5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="967f5-132">Response</span></span>

<span data-ttu-id="967f5-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="967f5-133">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="967f5-134">Пример</span><span class="sxs-lookup"><span data-stu-id="967f5-134">Example</span></span>
<span data-ttu-id="967f5-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="967f5-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="967f5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="967f5-136">Request</span></span>
<span data-ttu-id="967f5-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="967f5-137">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="967f5-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="967f5-138">Response</span></span>
<span data-ttu-id="967f5-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="967f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="967f5-142">Ниже приведен пример указания необязательного `valuesOnly` параметр.</span><span class="sxs-lookup"><span data-stu-id="967f5-142">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="967f5-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="967f5-143">Request</span></span>
<span data-ttu-id="967f5-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="967f5-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="967f5-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="967f5-145">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->