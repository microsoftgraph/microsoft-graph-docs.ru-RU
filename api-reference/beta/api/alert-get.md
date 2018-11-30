---
title: получение оповещения;
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: a3c8acb8ab748636d7a79b7ce3995a61699f7946
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076023"
---
# <a name="get-alert"></a><span data-ttu-id="3ee38-104">получение оповещения;</span><span class="sxs-lookup"><span data-stu-id="3ee38-104">Get alert</span></span>

 > <span data-ttu-id="3ee38-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3ee38-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ee38-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ee38-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ee38-107">Извлечение свойств и связи объекта [оповещение](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="3ee38-107">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ee38-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ee38-108">Permissions</span></span>

<span data-ttu-id="3ee38-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ee38-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ee38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ee38-111">Permission type</span></span>      | <span data-ttu-id="3ee38-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ee38-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ee38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ee38-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="3ee38-114">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ee38-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="3ee38-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ee38-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3ee38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ee38-116">Not supported.</span></span>  |
|<span data-ttu-id="3ee38-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3ee38-117">Application</span></span> | <span data-ttu-id="3ee38-118">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ee38-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ee38-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ee38-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3ee38-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ee38-120">Request headers</span></span>

| <span data-ttu-id="3ee38-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3ee38-121">Name</span></span>      |<span data-ttu-id="3ee38-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3ee38-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3ee38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ee38-123">Authorization</span></span>  | <span data-ttu-id="3ee38-p104">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ee38-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ee38-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ee38-126">Request body</span></span>

<span data-ttu-id="3ee38-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ee38-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ee38-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ee38-128">Response</span></span>

<span data-ttu-id="3ee38-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **оповещения** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3ee38-129">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="3ee38-130">Если код состояния, отличный от 2xx или 404 возвращается у поставщика или если поставщик времени ожидания, ответ будет `206 Partial Content` код состояния с ответом поставщиков в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="3ee38-130">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="3ee38-131">Для получения дополнительных сведений см [Microsoft Graph безопасности API сообщений об ошибках](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="3ee38-131">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="3ee38-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3ee38-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ee38-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ee38-133">Request</span></span>

<span data-ttu-id="3ee38-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ee38-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts/{id}
```

### <a name="response"></a><span data-ttu-id="3ee38-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ee38-135">Response</span></span>

<span data-ttu-id="3ee38-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3ee38-136">The following is an example of the response.</span></span>
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
