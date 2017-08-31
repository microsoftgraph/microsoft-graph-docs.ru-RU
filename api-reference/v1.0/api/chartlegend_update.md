# <a name="update-chartlegend"></a><span data-ttu-id="f819a-101">Обновление объекта chartlegend</span><span class="sxs-lookup"><span data-stu-id="f819a-101">Update chartlegend</span></span>

<span data-ttu-id="f819a-102">Обновление свойств объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="f819a-102">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f819a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f819a-103">Permissions</span></span>
<span data-ttu-id="f819a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f819a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f819a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f819a-106">Permission type</span></span>      | <span data-ttu-id="f819a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f819a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f819a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f819a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f819a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f819a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f819a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f819a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f819a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f819a-111">Not supported.</span></span>    |
|<span data-ttu-id="f819a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f819a-112">Application</span></span> | <span data-ttu-id="f819a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f819a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f819a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f819a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="f819a-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f819a-115">Optional request headers</span></span>
| <span data-ttu-id="f819a-116">Имя</span><span class="sxs-lookup"><span data-stu-id="f819a-116">Name</span></span>       | <span data-ttu-id="f819a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f819a-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f819a-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f819a-118">Authorization</span></span>  | <span data-ttu-id="f819a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f819a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f819a-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f819a-121">Request body</span></span>
<span data-ttu-id="f819a-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f819a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f819a-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="f819a-125">Property</span></span>     | <span data-ttu-id="f819a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="f819a-126">Type</span></span>   |<span data-ttu-id="f819a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="f819a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f819a-128">overlay</span><span class="sxs-lookup"><span data-stu-id="f819a-128">overlay</span></span>|<span data-ttu-id="f819a-129">boolean</span><span class="sxs-lookup"><span data-stu-id="f819a-129">boolean</span></span>|<span data-ttu-id="f819a-130">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="f819a-130">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="f819a-131">position</span><span class="sxs-lookup"><span data-stu-id="f819a-131">position</span></span>|<span data-ttu-id="f819a-132">string</span><span class="sxs-lookup"><span data-stu-id="f819a-132">string</span></span>|<span data-ttu-id="f819a-p104">Представляет расположение легенды на диаграмме. Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="f819a-p104">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="f819a-135">visible</span><span class="sxs-lookup"><span data-stu-id="f819a-135">visible</span></span>|<span data-ttu-id="f819a-136">boolean</span><span class="sxs-lookup"><span data-stu-id="f819a-136">boolean</span></span>|<span data-ttu-id="f819a-137">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="f819a-137">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="f819a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f819a-138">Response</span></span>

<span data-ttu-id="f819a-139">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartLegend](../resources/chartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f819a-139">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f819a-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f819a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f819a-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f819a-141">Request</span></span>
<span data-ttu-id="f819a-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f819a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="f819a-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="f819a-143">Response</span></span>
<span data-ttu-id="f819a-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f819a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->