# <a name="get-chartlegend"></a><span data-ttu-id="639d1-101">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="639d1-101">Get ChartLegend</span></span>

<span data-ttu-id="639d1-102">Получение свойств и связей объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="639d1-102">Retrieve the properties and relationships of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="639d1-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="639d1-103">Permissions</span></span>
<span data-ttu-id="639d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="639d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="639d1-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="639d1-106">Permission type</span></span>      | <span data-ttu-id="639d1-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="639d1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="639d1-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="639d1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="639d1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="639d1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="639d1-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="639d1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="639d1-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="639d1-111">Not supported.</span></span>    |
|<span data-ttu-id="639d1-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="639d1-112">Application</span></span> | <span data-ttu-id="639d1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="639d1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="639d1-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="639d1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-query-parameters"></a><span data-ttu-id="639d1-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="639d1-115">Optional query parameters</span></span>
<span data-ttu-id="639d1-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="639d1-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="639d1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="639d1-117">Request headers</span></span>
| <span data-ttu-id="639d1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="639d1-118">Name</span></span>      |<span data-ttu-id="639d1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="639d1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="639d1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="639d1-120">Authorization</span></span>  | <span data-ttu-id="639d1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="639d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="639d1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="639d1-123">Request body</span></span>
<span data-ttu-id="639d1-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="639d1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="639d1-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="639d1-125">Response</span></span>

<span data-ttu-id="639d1-126">В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartLegend](../resources/chartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="639d1-126">If successful, this method returns a `200 OK` response code and [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="639d1-127">Пример</span><span class="sxs-lookup"><span data-stu-id="639d1-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="639d1-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="639d1-128">Request</span></span>
<span data-ttu-id="639d1-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="639d1-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartlegend"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
```
##### <a name="response"></a><span data-ttu-id="639d1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="639d1-130">Response</span></span>
<span data-ttu-id="639d1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="639d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get ChartLegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->