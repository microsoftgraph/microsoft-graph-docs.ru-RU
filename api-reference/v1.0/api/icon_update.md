# <a name="update-icon"></a><span data-ttu-id="16eab-101">Обновление значка</span><span class="sxs-lookup"><span data-stu-id="16eab-101">Update icon</span></span>

<span data-ttu-id="16eab-102">Обновление свойств объекта значка.</span><span class="sxs-lookup"><span data-stu-id="16eab-102">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="16eab-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16eab-103">Permissions</span></span>
<span data-ttu-id="16eab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="16eab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16eab-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16eab-106">Permission type</span></span>      | <span data-ttu-id="16eab-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16eab-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="16eab-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16eab-108">Delegated (work or school account)</span></span> | <span data-ttu-id="16eab-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16eab-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="16eab-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16eab-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16eab-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16eab-111">Not supported.</span></span>    | 
|<span data-ttu-id="16eab-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16eab-112">Application</span></span> | <span data-ttu-id="16eab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16eab-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="16eab-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16eab-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="16eab-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16eab-115">Optional request headers</span></span>
| <span data-ttu-id="16eab-116">Имя</span><span class="sxs-lookup"><span data-stu-id="16eab-116">Name</span></span>       | <span data-ttu-id="16eab-117">Описание</span><span class="sxs-lookup"><span data-stu-id="16eab-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="16eab-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16eab-118">Authorization</span></span>  | <span data-ttu-id="16eab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16eab-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="16eab-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16eab-121">Request body</span></span>
<span data-ttu-id="16eab-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="16eab-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="16eab-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="16eab-125">Property</span></span>     | <span data-ttu-id="16eab-126">Тип</span><span class="sxs-lookup"><span data-stu-id="16eab-126">Type</span></span>   |<span data-ttu-id="16eab-127">Описание</span><span class="sxs-lookup"><span data-stu-id="16eab-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16eab-128">index</span><span class="sxs-lookup"><span data-stu-id="16eab-128">index</span></span>|<span data-ttu-id="16eab-129">int</span><span class="sxs-lookup"><span data-stu-id="16eab-129">int</span></span>|<span data-ttu-id="16eab-130">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="16eab-130">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="16eab-131">set</span><span class="sxs-lookup"><span data-stu-id="16eab-131">set</span></span>|<span data-ttu-id="16eab-132">string</span><span class="sxs-lookup"><span data-stu-id="16eab-132">string</span></span>|<span data-ttu-id="16eab-133">Представляет множество, частью которого является этот значок.</span><span class="sxs-lookup"><span data-stu-id="16eab-133">Represents the set that the icon is part of. Possible values are: , , , , , , , , , , , , , , , , , , , , .</span></span> <span data-ttu-id="16eab-134">Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="16eab-134">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="16eab-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="16eab-135">Response</span></span>

<span data-ttu-id="16eab-136">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Icon](../resources/icon.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16eab-136">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16eab-137">Пример</span><span class="sxs-lookup"><span data-stu-id="16eab-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16eab-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="16eab-138">Request</span></span>
<span data-ttu-id="16eab-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16eab-139">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="16eab-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="16eab-140">Response</span></span>
<span data-ttu-id="16eab-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16eab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
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