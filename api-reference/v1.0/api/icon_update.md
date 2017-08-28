# <a name="update-icon"></a><span data-ttu-id="54d2b-101">Обновление значка</span><span class="sxs-lookup"><span data-stu-id="54d2b-101">Update icon</span></span>

<span data-ttu-id="54d2b-102">Обновление свойств объекта значка.</span><span class="sxs-lookup"><span data-stu-id="54d2b-102">Update the properties of icon object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54d2b-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="54d2b-103">Prerequisites</span></span>
<span data-ttu-id="54d2b-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="54d2b-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="54d2b-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="54d2b-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="54d2b-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54d2b-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="54d2b-107">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54d2b-107">Optional request headers</span></span>
| <span data-ttu-id="54d2b-108">Имя</span><span class="sxs-lookup"><span data-stu-id="54d2b-108">Name</span></span>       | <span data-ttu-id="54d2b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="54d2b-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="54d2b-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54d2b-110">Authorization</span></span>  | <span data-ttu-id="54d2b-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54d2b-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54d2b-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54d2b-113">Request body</span></span>
<span data-ttu-id="54d2b-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="54d2b-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="54d2b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="54d2b-117">Property</span></span>     | <span data-ttu-id="54d2b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="54d2b-118">Type</span></span>   |<span data-ttu-id="54d2b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="54d2b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54d2b-120">index</span><span class="sxs-lookup"><span data-stu-id="54d2b-120">index</span></span>|<span data-ttu-id="54d2b-121">int</span><span class="sxs-lookup"><span data-stu-id="54d2b-121">int</span></span>|<span data-ttu-id="54d2b-122">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="54d2b-122">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="54d2b-123">set</span><span class="sxs-lookup"><span data-stu-id="54d2b-123">set</span></span>|<span data-ttu-id="54d2b-124">string</span><span class="sxs-lookup"><span data-stu-id="54d2b-124">string</span></span>|<span data-ttu-id="54d2b-p103">Представляет набор, в который входит значок. Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="54d2b-p103">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="54d2b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="54d2b-127">Response</span></span>

<span data-ttu-id="54d2b-128">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Icon](../resources/icon.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54d2b-128">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54d2b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="54d2b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54d2b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="54d2b-130">Request</span></span>
<span data-ttu-id="54d2b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54d2b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="54d2b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="54d2b-132">Response</span></span>
<span data-ttu-id="54d2b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="54d2b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->