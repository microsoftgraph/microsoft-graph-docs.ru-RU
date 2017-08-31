# <a name="update-charttitle"></a><span data-ttu-id="1967e-101">Обновление объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="1967e-101">Update charttitle</span></span>

<span data-ttu-id="1967e-102">Обновление свойств объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="1967e-102">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1967e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1967e-103">Permissions</span></span>
<span data-ttu-id="1967e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1967e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1967e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1967e-106">Permission type</span></span>      | <span data-ttu-id="1967e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1967e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1967e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1967e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1967e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1967e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1967e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1967e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1967e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1967e-111">Not supported.</span></span>    |
|<span data-ttu-id="1967e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1967e-112">Application</span></span> | <span data-ttu-id="1967e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1967e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1967e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1967e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="1967e-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1967e-115">Optional request headers</span></span>
| <span data-ttu-id="1967e-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1967e-116">Name</span></span>       | <span data-ttu-id="1967e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="1967e-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1967e-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1967e-118">Authorization</span></span>  | <span data-ttu-id="1967e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1967e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1967e-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1967e-121">Request body</span></span>
<span data-ttu-id="1967e-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1967e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1967e-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="1967e-125">Property</span></span>     | <span data-ttu-id="1967e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1967e-126">Type</span></span>   |<span data-ttu-id="1967e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1967e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1967e-128">overlay</span><span class="sxs-lookup"><span data-stu-id="1967e-128">overlay</span></span>|<span data-ttu-id="1967e-129">boolean</span><span class="sxs-lookup"><span data-stu-id="1967e-129">boolean</span></span>|<span data-ttu-id="1967e-130">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="1967e-130">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="1967e-131">text</span><span class="sxs-lookup"><span data-stu-id="1967e-131">text</span></span>|<span data-ttu-id="1967e-132">string</span><span class="sxs-lookup"><span data-stu-id="1967e-132">string</span></span>|<span data-ttu-id="1967e-133">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="1967e-133">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="1967e-134">visible</span><span class="sxs-lookup"><span data-stu-id="1967e-134">visible</span></span>|<span data-ttu-id="1967e-135">boolean</span><span class="sxs-lookup"><span data-stu-id="1967e-135">boolean</span></span>|<span data-ttu-id="1967e-136">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="1967e-136">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="1967e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1967e-137">Response</span></span>

<span data-ttu-id="1967e-138">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartTitle](../resources/charttitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1967e-138">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1967e-139">Пример</span><span class="sxs-lookup"><span data-stu-id="1967e-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1967e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1967e-140">Request</span></span>
<span data-ttu-id="1967e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1967e-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="1967e-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="1967e-142">Response</span></span>
<span data-ttu-id="1967e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1967e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->