---
title: Получение оповещения
description: Получение свойств и связей объекта Alert
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 22ea8d250c7e7b61260e0b2e5503850d251f669a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258571"
---
# <a name="get-alert"></a><span data-ttu-id="e1142-103">Получение оповещения</span><span class="sxs-lookup"><span data-stu-id="e1142-103">Get alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1142-104">Получение свойств и связей объекта [Alert](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="e1142-104">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1142-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1142-105">Permissions</span></span>

<span data-ttu-id="e1142-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1142-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1142-108">Permission type</span></span>      | <span data-ttu-id="e1142-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1142-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1142-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1142-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e1142-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1142-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="e1142-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1142-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e1142-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1142-113">Not supported.</span></span>  |
|<span data-ttu-id="e1142-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="e1142-114">Application</span></span> | <span data-ttu-id="e1142-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1142-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1142-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1142-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e1142-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1142-117">Request headers</span></span>

| <span data-ttu-id="e1142-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e1142-118">Name</span></span>      |<span data-ttu-id="e1142-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e1142-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1142-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1142-120">Authorization</span></span>  | <span data-ttu-id="e1142-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="e1142-121">Bearer {code}.</span></span> <span data-ttu-id="e1142-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="e1142-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1142-123">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="e1142-123">Request body</span></span>

<span data-ttu-id="e1142-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1142-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1142-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1142-125">Response</span></span>

<span data-ttu-id="e1142-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **Alert** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1142-126">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="e1142-127">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="e1142-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="e1142-128">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="e1142-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="e1142-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e1142-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1142-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1142-130">Request</span></span>

<span data-ttu-id="e1142-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1142-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts/{id}
```

### <a name="response"></a><span data-ttu-id="e1142-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1142-132">Response</span></span>

<span data-ttu-id="e1142-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1142-133">The following is an example of the response.</span></span>
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
  "historyStates": [
    {
      "appId": "appId-value",
      "assignedTo": "assignedTo-value",
      "comments": [
        "comments-value"
      ],
      "feedback": "feedback-value",
      "status": "status-value",
      "updatedDateTime": "datetime-value",
      "user": "user-value"
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
      "protocol": "String",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1142-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e1142-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1142-135">C#</span><span class="sxs-lookup"><span data-stu-id="e1142-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_alert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1142-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1142-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_alert-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e1142-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e1142-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_alert-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get glert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/alert-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
