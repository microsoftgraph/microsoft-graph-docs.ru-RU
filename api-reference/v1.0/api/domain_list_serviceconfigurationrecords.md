# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="2553b-101">Перечисление serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="2553b-101">List serviceConfigurationRecords</span></span>

<span data-ttu-id="2553b-102">Получение списка объектов [domainDnsRecord](../resources/domaindnsrecord.md), которые требуются, чтобы включить службы для домена.</span><span class="sxs-lookup"><span data-stu-id="2553b-102">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="2553b-p101">Используйте возвращенный список для добавления записей в файле зоны домена. Это можно сделать с помощью регистратора доменных имен или путем настройки DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="2553b-p101">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="2553b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2553b-105">Permissions</span></span>

<span data-ttu-id="2553b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2553b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="2553b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2553b-108">Permission type</span></span>      | <span data-ttu-id="2553b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2553b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2553b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2553b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2553b-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2553b-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="2553b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2553b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2553b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2553b-113">Not supported.</span></span>    |
|<span data-ttu-id="2553b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2553b-114">Application</span></span> | <span data-ttu-id="2553b-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2553b-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2553b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2553b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2553b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2553b-117">Optional query parameters</span></span>

<span data-ttu-id="2553b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2553b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2553b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2553b-119">Request headers</span></span>

| <span data-ttu-id="2553b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2553b-120">Name</span></span>      |<span data-ttu-id="2553b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2553b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2553b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2553b-122">Authorization</span></span>  | <span data-ttu-id="2553b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2553b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2553b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2553b-125">Content-Type</span></span>  | <span data-ttu-id="2553b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2553b-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2553b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2553b-127">Request body</span></span>

<span data-ttu-id="2553b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2553b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2553b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2553b-129">Response</span></span>

<span data-ttu-id="2553b-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2553b-130">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2553b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2553b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2553b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2553b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="2553b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2553b-133">Response</span></span>
<span data-ttu-id="2553b-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2553b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "@odata.type":"microsoft.graph.domainDnsMxRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "@odata.type":"microsoft.graph.domainDnsTxtRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedService": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->