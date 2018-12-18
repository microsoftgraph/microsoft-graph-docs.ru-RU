---
title: получение оповещения;
description: " Извлечение свойств и связи оповещения объекта."
author: Preetikr
ms.openlocfilehash: fe265f82e6013081a33abeaa25baa78e0e87fdcb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326126"
---
# <a name="get-alert"></a><span data-ttu-id="89214-103">получение оповещения;</span><span class="sxs-lookup"><span data-stu-id="89214-103">Get alert</span></span>

 <span data-ttu-id="89214-104">Извлечение свойств и связи объекта [оповещение](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="89214-104">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="89214-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89214-105">Permissions</span></span>

<span data-ttu-id="89214-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89214-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89214-108">Permission type</span></span>      | <span data-ttu-id="89214-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89214-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89214-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89214-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="89214-111">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89214-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="89214-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89214-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="89214-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89214-113">Not supported.</span></span>  |
|<span data-ttu-id="89214-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89214-114">Application</span></span> | <span data-ttu-id="89214-115">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89214-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89214-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89214-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="89214-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89214-117">Request headers</span></span>

| <span data-ttu-id="89214-118">Имя</span><span class="sxs-lookup"><span data-stu-id="89214-118">Name</span></span>      |<span data-ttu-id="89214-119">Описание</span><span class="sxs-lookup"><span data-stu-id="89214-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="89214-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89214-120">Authorization</span></span>  | <span data-ttu-id="89214-p102">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89214-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89214-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89214-123">Request body</span></span>

<span data-ttu-id="89214-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89214-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89214-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="89214-125">Response</span></span>

<span data-ttu-id="89214-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **оповещения** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="89214-126">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="89214-127">Если код состояния, отличный от 2xx или 404 возвращается у поставщика или если поставщик времени ожидания, ответ будет `206 Partial Content` код состояния с ответа поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="89214-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="89214-128">Для получения дополнительных сведений см [Microsoft Graph безопасности API сообщений об ошибках](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="89214-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="89214-129">Пример</span><span class="sxs-lookup"><span data-stu-id="89214-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="89214-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="89214-130">Request</span></span>

<span data-ttu-id="89214-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89214-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
```

### <a name="response"></a><span data-ttu-id="89214-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="89214-132">Response</span></span>

<span data-ttu-id="89214-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="89214-133">The following is an example of the response.</span></span>
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
