# <a name="range-intersection"></a><span data-ttu-id="f3c54-101">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="f3c54-101">Range: Intersection</span></span>

<span data-ttu-id="f3c54-102">Возвращает объект диапазона, представляющий собой прямоугольное пересечение заданных диапазонов.</span><span class="sxs-lookup"><span data-stu-id="f3c54-102">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3c54-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c54-103">Permissions</span></span>
<span data-ttu-id="f3c54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f3c54-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c54-106">Permission type</span></span>      | <span data-ttu-id="f3c54-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3c54-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3c54-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3c54-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f3c54-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3c54-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f3c54-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3c54-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3c54-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c54-111">Not supported.</span></span>    |
|<span data-ttu-id="f3c54-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3c54-112">Application</span></span> | <span data-ttu-id="f3c54-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c54-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3c54-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3c54-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(<address>)/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="f3c54-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3c54-115">Request headers</span></span>
| <span data-ttu-id="f3c54-116">Имя</span><span class="sxs-lookup"><span data-stu-id="f3c54-116">Name</span></span>       | <span data-ttu-id="f3c54-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f3c54-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3c54-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3c54-118">Authorization</span></span>  | <span data-ttu-id="f3c54-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3c54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3c54-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3c54-121">Request body</span></span>
<span data-ttu-id="f3c54-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f3c54-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f3c54-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="f3c54-123">Parameter</span></span>    | <span data-ttu-id="f3c54-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f3c54-124">Type</span></span>   |<span data-ttu-id="f3c54-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f3c54-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3c54-126">anotherRange</span><span class="sxs-lookup"><span data-stu-id="f3c54-126">anotherRange</span></span>|<span data-ttu-id="f3c54-127">string</span><span class="sxs-lookup"><span data-stu-id="f3c54-127">string</span></span>|<span data-ttu-id="f3c54-128">Объект или адрес диапазона, который будет использоваться для определения пересечения диапазонов.</span><span class="sxs-lookup"><span data-stu-id="f3c54-128">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="f3c54-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c54-129">Response</span></span>

<span data-ttu-id="f3c54-130">В случае успеха этот метод возвращает код отклика `200, OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f3c54-130">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3c54-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f3c54-131">Example</span></span>
<span data-ttu-id="f3c54-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f3c54-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f3c54-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3c54-133">Request</span></span>
<span data-ttu-id="f3c54-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3c54-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="f3c54-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3c54-135">Response</span></span>
<span data-ttu-id="f3c54-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f3c54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->