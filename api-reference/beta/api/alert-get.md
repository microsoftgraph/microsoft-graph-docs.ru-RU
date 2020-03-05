---
title: Получение оповещения
description: Получение свойств и связей объекта Alert
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3bcb4d9c198d4b53e589322d0f597cfb5fd88350
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441629"
---
# <a name="get-alert"></a><span data-ttu-id="c7c91-103">Получение оповещения</span><span class="sxs-lookup"><span data-stu-id="c7c91-103">Get alert</span></span>

<span data-ttu-id="c7c91-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c7c91-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7c91-105">Получение свойств и связей объекта [Alert](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="c7c91-105">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7c91-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7c91-106">Permissions</span></span>

<span data-ttu-id="c7c91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7c91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c91-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7c91-109">Permission type</span></span>      | <span data-ttu-id="c7c91-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7c91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7c91-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7c91-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c7c91-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c91-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="c7c91-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7c91-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c7c91-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7c91-114">Not supported.</span></span>  |
|<span data-ttu-id="c7c91-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c7c91-115">Application</span></span> | <span data-ttu-id="c7c91-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c91-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7c91-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7c91-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c7c91-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7c91-118">Request headers</span></span>

| <span data-ttu-id="c7c91-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c7c91-119">Name</span></span>      |<span data-ttu-id="c7c91-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c7c91-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7c91-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7c91-121">Authorization</span></span>  | <span data-ttu-id="c7c91-122">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="c7c91-122">Bearer {code}.</span></span> <span data-ttu-id="c7c91-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c7c91-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c91-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7c91-124">Request body</span></span>

<span data-ttu-id="c7c91-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7c91-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7c91-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7c91-126">Response</span></span>

<span data-ttu-id="c7c91-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **Alert** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7c91-127">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="c7c91-128">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="c7c91-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="c7c91-129">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="c7c91-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="c7c91-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c7c91-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7c91-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7c91-131">Request</span></span>

<span data-ttu-id="c7c91-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7c91-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7c91-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7c91-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/alerts/{id}
```
# <a name="c"></a>[<span data-ttu-id="c7c91-134">C#</span><span class="sxs-lookup"><span data-stu-id="c7c91-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7c91-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7c91-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7c91-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7c91-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7c91-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7c91-137">Response</span></span>

<span data-ttu-id="c7c91-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c7c91-138">The following is an example of the response.</span></span>
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
  ]
}
-->
