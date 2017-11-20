# <a name="list-series"></a><span data-ttu-id="ebcfb-101">Список рядов</span><span class="sxs-lookup"><span data-stu-id="ebcfb-101">List series</span></span>

<span data-ttu-id="ebcfb-102">Получение списка объектов chartseries.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-102">Retrieve a list of chartseries objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebcfb-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebcfb-103">Permissions</span></span>
<span data-ttu-id="ebcfb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ebcfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ebcfb-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebcfb-106">Permission type</span></span>      | <span data-ttu-id="ebcfb-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebcfb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebcfb-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebcfb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ebcfb-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebcfb-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebcfb-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebcfb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebcfb-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-111">Not supported.</span></span>    |
|<span data-ttu-id="ebcfb-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebcfb-112">Application</span></span> | <span data-ttu-id="ebcfb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebcfb-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebcfb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebcfb-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ebcfb-115">Optional query parameters</span></span>
<span data-ttu-id="ebcfb-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebcfb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebcfb-117">Request headers</span></span>
| <span data-ttu-id="ebcfb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ebcfb-118">Name</span></span>      |<span data-ttu-id="ebcfb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ebcfb-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ebcfb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebcfb-120">Authorization</span></span>  | <span data-ttu-id="ebcfb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebcfb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ebcfb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ebcfb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebcfb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebcfb-126">Request body</span></span>
<span data-ttu-id="ebcfb-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebcfb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebcfb-128">Response</span></span>

<span data-ttu-id="ebcfb-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ChartSeries](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-129">If successful, this method returns a `200 OK` response code and collection of [ChartSeries](../resources/chartseries.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebcfb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ebcfb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebcfb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebcfb-131">Request</span></span>
<span data-ttu-id="ebcfb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_series"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
```
##### <a name="response"></a><span data-ttu-id="ebcfb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebcfb-133">Response</span></span>
<span data-ttu-id="ebcfb-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ebcfb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 59

{
  "value": [
    {
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List series",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->