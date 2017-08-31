# <a name="update-chartseries"></a><span data-ttu-id="1b05f-101">Обновление объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="1b05f-101">Update chartseries</span></span>

<span data-ttu-id="1b05f-102">Обновление свойств объекта chartseries.</span><span class="sxs-lookup"><span data-stu-id="1b05f-102">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b05f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b05f-103">Permissions</span></span>
<span data-ttu-id="1b05f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b05f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1b05f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b05f-106">Permission type</span></span>      | <span data-ttu-id="1b05f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b05f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b05f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b05f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1b05f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b05f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1b05f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b05f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b05f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b05f-111">Not supported.</span></span>    |
|<span data-ttu-id="1b05f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b05f-112">Application</span></span> | <span data-ttu-id="1b05f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b05f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b05f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b05f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="1b05f-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b05f-115">Optional request headers</span></span>
| <span data-ttu-id="1b05f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1b05f-116">Name</span></span>       | <span data-ttu-id="1b05f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="1b05f-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1b05f-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b05f-118">Authorization</span></span>  | <span data-ttu-id="1b05f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b05f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b05f-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b05f-121">Request body</span></span>
<span data-ttu-id="1b05f-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1b05f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1b05f-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b05f-125">Property</span></span>     | <span data-ttu-id="1b05f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1b05f-126">Type</span></span>   |<span data-ttu-id="1b05f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1b05f-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b05f-128">name</span><span class="sxs-lookup"><span data-stu-id="1b05f-128">name</span></span>|<span data-ttu-id="1b05f-129">string</span><span class="sxs-lookup"><span data-stu-id="1b05f-129">string</span></span>|<span data-ttu-id="1b05f-130">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="1b05f-130">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="1b05f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b05f-131">Response</span></span>

<span data-ttu-id="1b05f-132">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartSeries](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b05f-132">If successful, this method returns a `200 OK` response code and updated [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b05f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1b05f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b05f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b05f-134">Request</span></span>
<span data-ttu-id="1b05f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b05f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="1b05f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b05f-136">Response</span></span>
<span data-ttu-id="1b05f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b05f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->