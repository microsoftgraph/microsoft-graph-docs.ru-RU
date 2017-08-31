# <a name="update-chartaxistitle"></a><span data-ttu-id="d0469-101">Обновление объекта chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="d0469-101">Update chartaxistitle</span></span>

<span data-ttu-id="d0469-102">Обновление свойств объекта chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="d0469-102">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d0469-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0469-103">Permissions</span></span>
<span data-ttu-id="d0469-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0469-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0469-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0469-106">Permission type</span></span>      | <span data-ttu-id="d0469-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0469-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0469-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0469-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d0469-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0469-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d0469-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0469-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0469-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0469-111">Not supported.</span></span>    |
|<span data-ttu-id="d0469-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0469-112">Application</span></span> | <span data-ttu-id="d0469-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0469-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0469-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0469-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="d0469-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0469-115">Optional request headers</span></span>
| <span data-ttu-id="d0469-116">Имя</span><span class="sxs-lookup"><span data-stu-id="d0469-116">Name</span></span>       | <span data-ttu-id="d0469-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d0469-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d0469-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0469-118">Authorization</span></span>  | <span data-ttu-id="d0469-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0469-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0469-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0469-121">Request body</span></span>
<span data-ttu-id="d0469-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d0469-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d0469-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0469-125">Property</span></span>     | <span data-ttu-id="d0469-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d0469-126">Type</span></span>   |<span data-ttu-id="d0469-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d0469-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0469-128">text</span><span class="sxs-lookup"><span data-stu-id="d0469-128">text</span></span>|<span data-ttu-id="d0469-129">string</span><span class="sxs-lookup"><span data-stu-id="d0469-129">string</span></span>|<span data-ttu-id="d0469-130">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="d0469-130">Represents the axis title.</span></span>|
|<span data-ttu-id="d0469-131">visible</span><span class="sxs-lookup"><span data-stu-id="d0469-131">visible</span></span>|<span data-ttu-id="d0469-132">boolean</span><span class="sxs-lookup"><span data-stu-id="d0469-132">boolean</span></span>|<span data-ttu-id="d0469-133">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="d0469-133">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="d0469-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0469-134">Response</span></span>

<span data-ttu-id="d0469-135">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartAxisTitle](../resources/chartaxistitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0469-135">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0469-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d0469-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0469-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0469-137">Request</span></span>
<span data-ttu-id="d0469-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0469-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="d0469-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0469-139">Response</span></span>
<span data-ttu-id="d0469-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d0469-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->