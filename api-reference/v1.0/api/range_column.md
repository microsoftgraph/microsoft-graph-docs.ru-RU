# <a name="range-column"></a><span data-ttu-id="072e6-101">Range: Column</span><span class="sxs-lookup"><span data-stu-id="072e6-101">Range: Column</span></span>

<span data-ttu-id="072e6-102">Возвращает столбец в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="072e6-102">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="072e6-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="072e6-103">Permissions</span></span>
<span data-ttu-id="072e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="072e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="072e6-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="072e6-106">Permission type</span></span>      | <span data-ttu-id="072e6-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="072e6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="072e6-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="072e6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="072e6-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="072e6-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="072e6-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="072e6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="072e6-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="072e6-111">Not supported.</span></span>    |
|<span data-ttu-id="072e6-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="072e6-112">Application</span></span> | <span data-ttu-id="072e6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="072e6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="072e6-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="072e6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Column
GET /workbook/worksheets/{id|name}/range(<address>)/Column
GET /workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="072e6-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="072e6-115">Request headers</span></span>
| <span data-ttu-id="072e6-116">Имя</span><span class="sxs-lookup"><span data-stu-id="072e6-116">Name</span></span>       | <span data-ttu-id="072e6-117">Описание</span><span class="sxs-lookup"><span data-stu-id="072e6-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="072e6-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="072e6-118">Authorization</span></span>  | <span data-ttu-id="072e6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="072e6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="072e6-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="072e6-121">Request body</span></span>
<span data-ttu-id="072e6-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="072e6-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="072e6-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="072e6-123">Parameter</span></span>    | <span data-ttu-id="072e6-124">Тип</span><span class="sxs-lookup"><span data-stu-id="072e6-124">Type</span></span>   |<span data-ttu-id="072e6-125">Описание</span><span class="sxs-lookup"><span data-stu-id="072e6-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="072e6-126">column</span><span class="sxs-lookup"><span data-stu-id="072e6-126">column</span></span>|<span data-ttu-id="072e6-127">number</span><span class="sxs-lookup"><span data-stu-id="072e6-127">number</span></span>|<span data-ttu-id="072e6-p103">Номер столбца диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="072e6-p103">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="072e6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="072e6-130">Response</span></span>

<span data-ttu-id="072e6-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="072e6-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="072e6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="072e6-132">Example</span></span>
<span data-ttu-id="072e6-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="072e6-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="072e6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="072e6-134">Request</span></span>
<span data-ttu-id="072e6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="072e6-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Column
Content-type: application/json
Content-length: 21

{
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="072e6-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="072e6-136">Response</span></span>
<span data-ttu-id="072e6-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="072e6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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