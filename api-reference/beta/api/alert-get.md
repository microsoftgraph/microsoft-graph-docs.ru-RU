---
title: получение оповещения;
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 5f5a7330476de71308680b41e87e51d5d228b2e0
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184485"
---
# <a name="get-alert"></a><span data-ttu-id="ddf3b-104">получение оповещения;</span><span class="sxs-lookup"><span data-stu-id="ddf3b-104">Get alert</span></span>

 > <span data-ttu-id="ddf3b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddf3b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ddf3b-107">Извлечение свойств и связи объекта [оповещение](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="ddf3b-107">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddf3b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddf3b-108">Permissions</span></span>

<span data-ttu-id="ddf3b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddf3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddf3b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddf3b-111">Permission type</span></span>      | <span data-ttu-id="ddf3b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddf3b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddf3b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddf3b-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="ddf3b-114">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddf3b-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="ddf3b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddf3b-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ddf3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-116">Not supported.</span></span>  |
|<span data-ttu-id="ddf3b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddf3b-117">Application</span></span> | <span data-ttu-id="ddf3b-118">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddf3b-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddf3b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddf3b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ddf3b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddf3b-120">Request headers</span></span>

| <span data-ttu-id="ddf3b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ddf3b-121">Name</span></span>      |<span data-ttu-id="ddf3b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ddf3b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ddf3b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddf3b-123">Authorization</span></span>  | <span data-ttu-id="ddf3b-p104">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddf3b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddf3b-126">Request body</span></span>

<span data-ttu-id="ddf3b-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddf3b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddf3b-128">Response</span></span>

<span data-ttu-id="ddf3b-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **оповещения** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-129">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="ddf3b-130">Если код состояния, отличный от 2xx или 404 возвращается у поставщика или если поставщик времени ожидания, ответ будет `206 Partial Content` код состояния с ответа поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-130">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="ddf3b-131">Для получения дополнительных сведений см [Microsoft Graph безопасности API сообщений об ошибках](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="ddf3b-131">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="ddf3b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ddf3b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddf3b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddf3b-133">Request</span></span>

<span data-ttu-id="ddf3b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts/{id}
```

### <a name="response"></a><span data-ttu-id="ddf3b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddf3b-135">Response</span></span>

<span data-ttu-id="ddf3b-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-136">The following is an example of the response.</span></span>
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
