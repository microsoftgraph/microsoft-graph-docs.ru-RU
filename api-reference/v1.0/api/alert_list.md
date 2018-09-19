# <a name="list-alerts"></a><span data-ttu-id="88222-101">Списки оповещений</span><span class="sxs-lookup"><span data-stu-id="88222-101">List alerts</span></span>

<span data-ttu-id="88222-102">Получение списка объектов [alert](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="88222-102">Retrieve a list of nameditem objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="88222-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88222-103">Permissions</span></span>

<span data-ttu-id="88222-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="88222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="88222-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88222-106">Permission type</span></span>      | <span data-ttu-id="88222-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88222-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88222-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88222-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="88222-109">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88222-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="88222-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88222-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="88222-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88222-111">Not supported.</span></span>  |
|<span data-ttu-id="88222-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88222-112">Application</span></span> | <span data-ttu-id="88222-113">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88222-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88222-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88222-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88222-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="88222-115">Optional query parameters</span></span>

<span data-ttu-id="88222-116">Этот метод поддерживает следующие [параметры запроса OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="88222-116">This method supports the following [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="88222-117">`$top` Выводит обобщенные лучшие результаты от каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="88222-117">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="88222-118">Чтобы вывести альтернативный набор свойств, используйте параметр запроса OData `$select` для определения набора нужных свойств **alert**.</span><span class="sxs-lookup"><span data-stu-id="88222-118">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="88222-119">Например, чтобы вывести свойства **assignedTo**, **category** и **severity**, добавьте следующие элементы в запрос: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="88222-119">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88222-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88222-120">Request headers</span></span>

| <span data-ttu-id="88222-121">Имя</span><span class="sxs-lookup"><span data-stu-id="88222-121">Name</span></span>      |<span data-ttu-id="88222-122">Описание</span><span class="sxs-lookup"><span data-stu-id="88222-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88222-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88222-123">Authorization</span></span>  | <span data-ttu-id="88222-p103">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88222-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88222-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88222-126">Request body</span></span>

<span data-ttu-id="88222-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88222-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="88222-128">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="88222-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="88222-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="88222-129">Response</span></span>

<span data-ttu-id="88222-130">В случае успешного выполнения операции этот метод выводит код ответа `200 OK` и набор объектов **alert** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="88222-130">If successful, this method returns a `200 OK` response code and collection of **directoryObject** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88222-131">Пример</span><span class="sxs-lookup"><span data-stu-id="88222-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="88222-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="88222-132">Request</span></span>

<span data-ttu-id="88222-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88222-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="88222-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="88222-134">Response</span></span>

<span data-ttu-id="88222-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="88222-135">The following is an example of the response.</span></span>

><span data-ttu-id="88222-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88222-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
