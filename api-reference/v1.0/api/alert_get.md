# <a name="get-alert"></a><span data-ttu-id="174e5-101">Получение объекта alert (оповещение)</span><span class="sxs-lookup"><span data-stu-id="174e5-101">Get alert</span></span>

 <span data-ttu-id="174e5-102">Получение свойств и связей объекта [alert](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="174e5-102">Retrieve the properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="174e5-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="174e5-103">Permissions</span></span>

<span data-ttu-id="174e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="174e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="174e5-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="174e5-106">Permission type</span></span>      | <span data-ttu-id="174e5-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="174e5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="174e5-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="174e5-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="174e5-109">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="174e5-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="174e5-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="174e5-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="174e5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="174e5-111">Not supported.</span></span>  |
|<span data-ttu-id="174e5-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="174e5-112">Application</span></span> | <span data-ttu-id="174e5-113">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="174e5-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="174e5-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="174e5-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="174e5-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="174e5-115">Request headers</span></span>

| <span data-ttu-id="174e5-116">Имя</span><span class="sxs-lookup"><span data-stu-id="174e5-116">Name</span></span>      |<span data-ttu-id="174e5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="174e5-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="174e5-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="174e5-118">Authorization</span></span>  | <span data-ttu-id="174e5-p102">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="174e5-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="174e5-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="174e5-121">Request body</span></span>

<span data-ttu-id="174e5-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="174e5-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="174e5-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="174e5-123">Response</span></span>

<span data-ttu-id="174e5-124">В случае успеха этот метод возвращает `200 OK` код отклика и объект **alert** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="174e5-124">If successful, this method returns a `200 OK` response code and an updated **androidStoreApp** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="174e5-125">Пример</span><span class="sxs-lookup"><span data-stu-id="174e5-125">Example</span></span>

### <a name="request"></a><span data-ttu-id="174e5-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="174e5-126">Request</span></span>

<span data-ttu-id="174e5-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="174e5-127">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
```

### <a name="response"></a><span data-ttu-id="174e5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="174e5-128">Response</span></span>

<span data-ttu-id="174e5-129">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="174e5-129">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [
    {
      "destinationServiceIp": "String",
      "destinationServiceName": "String",
      "riskScore": "String"
    }
  ],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [
    {
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "name": "String",
      "path": "String",
      "riskScore": "String"
    }
  ],
  "hostStates": [
    {
      "fqdn": "String",
      "isAzureAadJoined": true,
      "isAzureAadRegistered": true,
      "isHybridAzureDomainJoined": true,
      "netBiosName": "String",
      "os": "String",
      "privateIpAddress": "String",
      "publicIpAddress": "String",
      "riskScore": "String"
    }
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [
    {
      "category": "String",
      "family": "String",
      "name": "String",
      "severity": "String",
      "wasRunning": true
    }
  ],
  "networkConnections": [
    {
      "applicationName": "String",
      "destinationAddress": "String",
      "destinationDomain": "String",
      "destinationPort": "String",
      "destinationUrl": "String",
      "direction": "@odata.type: microsoft.graph.connectionDirection",
      "domainRegisteredDateTime": "String (timestamp)",
      "localDnsName": "String",
      "natDestinationAddress": "String",
      "natDestinationPort": "String",
      "natSourceAddress": "String",
      "natSourcePort": "String",
      "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
      "riskScore": "String",
      "sourceAddress": "String",
      "sourcePort": "String",
      "status": "@odata.type: microsoft.graph.connectionStatus",
      "urlParameters": "String"
    }
  ],
  "processes": [
    {
      "accountName": "String",
      "commandLine": "String",
      "createdDateTime": "String (timestamp)",
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
      "isElevated": true,
      "name": "String",
      "parentProcessCreatedDateTime": "String (timestamp)",
      "parentProcessId": 1024,
      "parentProcessName": "String",
      "path": "String",
      "processId": 1024
    }
  ],
  "recommendedActions": ["String"],
  "registryKeyStates": [
    {
      "hive": "@odata.type: microsoft.graph.registryHive",
      "key": "String",
      "oldKey": "String",
      "oldValueData": "String",
      "oldValueName": "String",
      "operation": "@odata.type: microsoft.graph.registryOperation",
      "processId": 1024,
      "valueData": "String",
      "valueName": "String",
      "valueType": "@odata.type: microsoft.graph.registryValueType"
    }
  ],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [
    {
      "name": "String",
      "type": "String",
      "value": "String"
    }
  ],
  "userStates": [
    {
      "aadUserId": "String",
      "accountName": "String",
      "domainName": "String",
      "emailRole": "@odata.type: microsoft.graph.emailRole",
      "isVpn": true,
      "logonDateTime": "String (timestamp)",
      "logonId": "String",
      "logonIp": "String",
      "logonLocation": "String",
      "logonType": "@odata.type: microsoft.graph.logonType",
      "onPremisesSecurityIdentifier": "String",
      "riskScore": "String",
      "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
      "userPrincipalName": "String"
    }
  ],
  "vendorInformation": {
    "provider": "String",
    "providerVersion": "String",
    "subProvider": "String",
    "vendor": "String"
  },
  "vulnerabilityStates": [
    {
      "cve": "String",
      "severity": "String",
      "wasRunning": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get glert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
