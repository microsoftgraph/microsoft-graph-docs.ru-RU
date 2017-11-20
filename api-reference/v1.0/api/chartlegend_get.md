# <a name="get-chartlegend"></a><span data-ttu-id="20350-101">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="20350-101">Get ChartLegend</span></span>

<span data-ttu-id="20350-102">Получение свойств и связей объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="20350-102">Retrieve the properties and relationships of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="20350-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20350-103">Permissions</span></span>
<span data-ttu-id="20350-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="20350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="20350-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20350-106">Permission type</span></span>      | <span data-ttu-id="20350-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20350-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20350-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20350-108">Delegated (work or school account)</span></span> | <span data-ttu-id="20350-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20350-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20350-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20350-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20350-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20350-111">Not supported.</span></span>    |
|<span data-ttu-id="20350-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20350-112">Application</span></span> | <span data-ttu-id="20350-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20350-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20350-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20350-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20350-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="20350-115">Optional query parameters</span></span>
<span data-ttu-id="20350-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="20350-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20350-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20350-117">Request headers</span></span>
| <span data-ttu-id="20350-118">Имя</span><span class="sxs-lookup"><span data-stu-id="20350-118">Name</span></span>      |<span data-ttu-id="20350-119">Описание</span><span class="sxs-lookup"><span data-stu-id="20350-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20350-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20350-120">Authorization</span></span>  | <span data-ttu-id="20350-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20350-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20350-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="20350-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="20350-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="20350-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20350-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20350-126">Request body</span></span>
<span data-ttu-id="20350-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20350-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20350-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="20350-128">Response</span></span>

<span data-ttu-id="20350-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartLegend](../resources/chartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20350-129">If successful, this method returns a `200 OK` response code and [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20350-130">Пример</span><span class="sxs-lookup"><span data-stu-id="20350-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20350-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="20350-131">Request</span></span>
<span data-ttu-id="20350-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20350-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartlegend"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
```
##### <a name="response"></a><span data-ttu-id="20350-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="20350-133">Response</span></span>
<span data-ttu-id="20350-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="20350-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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