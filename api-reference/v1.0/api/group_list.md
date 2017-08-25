# <a name="list-groups"></a><span data-ttu-id="d3459-101">Список групп</span><span class="sxs-lookup"><span data-stu-id="d3459-101">List groups</span></span>

<span data-ttu-id="d3459-p101">Список всех групп, доступных в организации, в том числе из функции "Группы Office 365". Возвращаются [свойства по умолчанию](../api/group_get.md#default-properties) для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="d3459-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group_get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="d3459-104">Чтобы получить только результаты из функции "Группы Office 365" (т. н. единые группы), примените фильтр **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="d3459-104">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="d3459-105">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="d3459-105">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```


## <a name="permissions"></a><span data-ttu-id="d3459-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3459-106">Permissions</span></span>
<span data-ttu-id="d3459-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3459-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d3459-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3459-109">Permission type</span></span>      | <span data-ttu-id="d3459-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3459-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d3459-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3459-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3459-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3459-112">Group.Read.All, Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="d3459-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3459-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3459-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3459-114">Not supported.</span></span>    | 
|<span data-ttu-id="d3459-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3459-115">Application</span></span> | <span data-ttu-id="d3459-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3459-116">Group.Read.All, Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d3459-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3459-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3459-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d3459-118">Optional query parameters</span></span>
<span data-ttu-id="d3459-119">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d3459-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d3459-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3459-120">Request headers</span></span>
| <span data-ttu-id="d3459-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d3459-121">Name</span></span>       | <span data-ttu-id="d3459-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d3459-122">Type</span></span> | <span data-ttu-id="d3459-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d3459-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d3459-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3459-124">Authorization</span></span>  | <span data-ttu-id="d3459-125">string</span><span class="sxs-lookup"><span data-stu-id="d3459-125">string</span></span>  | <span data-ttu-id="d3459-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3459-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3459-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3459-128">Request body</span></span>
<span data-ttu-id="d3459-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3459-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3459-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3459-130">Response</span></span>

<span data-ttu-id="d3459-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3459-131">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3459-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d3459-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3459-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3459-133">Request</span></span>
<span data-ttu-id="d3459-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3459-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```
##### <a name="response"></a><span data-ttu-id="d3459-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3459-135">Response</span></span>
<span data-ttu-id="d3459-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3459-136">Here is an example of the response.</span></span>

<span data-ttu-id="d3459-p104">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове возвращаются [все свойства](../api/group_get.md#default-properties).</span><span class="sxs-lookup"><span data-stu-id="d3459-p104">Note: The response object shown here may be truncated for brevity. The [default properties](../api/group_get.md#default-properties) will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
