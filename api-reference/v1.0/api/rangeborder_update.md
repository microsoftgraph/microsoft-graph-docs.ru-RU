# <a name="update-rangeborder"></a><span data-ttu-id="2477d-101">Обновление объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="2477d-101">Update rangeborder</span></span>

<span data-ttu-id="2477d-102">Обновление свойств объекта rangeborder.</span><span class="sxs-lookup"><span data-stu-id="2477d-102">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2477d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2477d-103">Permissions</span></span>
<span data-ttu-id="2477d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2477d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2477d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2477d-106">Permission type</span></span>      | <span data-ttu-id="2477d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2477d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2477d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2477d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2477d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2477d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2477d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2477d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2477d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2477d-111">Not supported.</span></span>    |
|<span data-ttu-id="2477d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2477d-112">Application</span></span> | <span data-ttu-id="2477d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2477d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2477d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2477d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="2477d-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2477d-115">Optional request headers</span></span>
| <span data-ttu-id="2477d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="2477d-116">Name</span></span>       | <span data-ttu-id="2477d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="2477d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2477d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2477d-118">Authorization</span></span>  | <span data-ttu-id="2477d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2477d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2477d-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2477d-121">Request body</span></span>
<span data-ttu-id="2477d-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2477d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2477d-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="2477d-125">Property</span></span>     | <span data-ttu-id="2477d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="2477d-126">Type</span></span>   |<span data-ttu-id="2477d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2477d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2477d-128">color</span><span class="sxs-lookup"><span data-stu-id="2477d-128">color</span></span>|<span data-ttu-id="2477d-129">string</span><span class="sxs-lookup"><span data-stu-id="2477d-129">string</span></span>|<span data-ttu-id="2477d-130">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="2477d-130">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="2477d-131">style</span><span class="sxs-lookup"><span data-stu-id="2477d-131">style</span></span>|<span data-ttu-id="2477d-132">string</span><span class="sxs-lookup"><span data-stu-id="2477d-132">string</span></span>|<span data-ttu-id="2477d-p104">Одна из констант типа линии, определяющая тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="2477d-p104">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="2477d-135">weight</span><span class="sxs-lookup"><span data-stu-id="2477d-135">weight</span></span>|<span data-ttu-id="2477d-136">string</span><span class="sxs-lookup"><span data-stu-id="2477d-136">string</span></span>|<span data-ttu-id="2477d-p105">Определяет толщину границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="2477d-p105">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="2477d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2477d-139">Response</span></span>

<span data-ttu-id="2477d-140">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [RangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2477d-140">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2477d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2477d-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2477d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2477d-142">Request</span></span>
<span data-ttu-id="2477d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2477d-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="2477d-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="2477d-144">Response</span></span>
<span data-ttu-id="2477d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2477d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->