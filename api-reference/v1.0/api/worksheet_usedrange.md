# <a name="worksheet-usedrange"></a><span data-ttu-id="34958-101">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="34958-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="34958-p101">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="34958-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="34958-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34958-104">Permissions</span></span>
<span data-ttu-id="34958-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="34958-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="34958-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34958-107">Permission type</span></span>      | <span data-ttu-id="34958-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34958-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34958-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34958-109">Delegated (work or school account)</span></span> | <span data-ttu-id="34958-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34958-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34958-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34958-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34958-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34958-112">Not supported.</span></span>    |
|<span data-ttu-id="34958-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34958-113">Application</span></span> | <span data-ttu-id="34958-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34958-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34958-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34958-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="34958-116">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="34958-116">Function parameters</span></span>
<span data-ttu-id="34958-117">В URL-адресе запроса можно указать дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="34958-117">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="34958-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="34958-118">Parameter</span></span>    | <span data-ttu-id="34958-119">Тип</span><span class="sxs-lookup"><span data-stu-id="34958-119">Type</span></span>   |<span data-ttu-id="34958-120">Описание</span><span class="sxs-lookup"><span data-stu-id="34958-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34958-121">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="34958-121">valuesOnly</span></span>|<span data-ttu-id="34958-122">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="34958-122">Boolean</span></span>|<span data-ttu-id="34958-p103">Необязательный параметр. Учитывает только ячейки со значениями (игнорирует форматирование).</span><span class="sxs-lookup"><span data-stu-id="34958-p103">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="34958-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34958-125">Request headers</span></span>
| <span data-ttu-id="34958-126">Имя</span><span class="sxs-lookup"><span data-stu-id="34958-126">Name</span></span>       | <span data-ttu-id="34958-127">Описание</span><span class="sxs-lookup"><span data-stu-id="34958-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34958-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34958-128">Authorization</span></span>  | <span data-ttu-id="34958-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34958-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34958-131">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34958-131">Workbook-Session-Id</span></span>  | <span data-ttu-id="34958-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="34958-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34958-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34958-134">Request body</span></span>
<span data-ttu-id="34958-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34958-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34958-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="34958-136">Response</span></span>

<span data-ttu-id="34958-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="34958-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34958-138">Пример</span><span class="sxs-lookup"><span data-stu-id="34958-138">Example</span></span>
<span data-ttu-id="34958-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="34958-139">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="34958-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="34958-140">Request</span></span>
<span data-ttu-id="34958-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34958-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="34958-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="34958-142">Response</span></span>
<span data-ttu-id="34958-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34958-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="34958-146">В ином варианте эта функция может быть вызвана с необязательным параметром `valuesOnly`.</span><span class="sxs-lookup"><span data-stu-id="34958-146">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="34958-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="34958-147">Request</span></span>
<span data-ttu-id="34958-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34958-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="34958-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="34958-149">Response</span></span>
<span data-ttu-id="34958-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34958-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
