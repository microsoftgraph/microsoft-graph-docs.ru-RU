---
title: Список windowsProtectionStates
description: Получите список объектов WindowsProtectionState и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: ae7de7e8edbb0141df25db91464a45ac1a6499fe
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442311"
---
# <a name="list-windowsprotectionstates"></a><span data-ttu-id="ddbc3-103">Список windowsProtectionStates</span><span class="sxs-lookup"><span data-stu-id="ddbc3-103">List windowsProtectionStates</span></span>
<span data-ttu-id="ddbc3-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ddbc3-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddbc3-105">Получите список объектов [WindowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="ddbc3-105">Get a list of the [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddbc3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddbc3-106">Permissions</span></span>
<span data-ttu-id="ddbc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddbc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddbc3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddbc3-109">Permission type</span></span>|<span data-ttu-id="ddbc3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddbc3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddbc3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddbc3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ddbc3-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddbc3-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ddbc3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddbc3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddbc3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddbc3-114">Not supported.</span></span>|
|<span data-ttu-id="ddbc3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddbc3-115">Application</span></span>|<span data-ttu-id="ddbc3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddbc3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddbc3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddbc3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/windowsProtectionStates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddbc3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ddbc3-118">Optional query parameters</span></span>
<span data-ttu-id="ddbc3-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="ddbc3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddbc3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddbc3-120">Request headers</span></span>
|<span data-ttu-id="ddbc3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ddbc3-121">Name</span></span>|<span data-ttu-id="ddbc3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ddbc3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ddbc3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddbc3-123">Authorization</span></span>|<span data-ttu-id="ddbc3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddbc3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddbc3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddbc3-126">Request body</span></span>
<span data-ttu-id="ddbc3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddbc3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddbc3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddbc3-128">Response</span></span>

<span data-ttu-id="ddbc3-129">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов WindowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ddbc3-129">If successful, this method returns a `200 OK` response code and a collection of [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddbc3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ddbc3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddbc3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddbc3-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ddbc3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddbc3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_windowsprotectionstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/windowsProtectionStates
```
# <a name="c"></a>[<span data-ttu-id="ddbc3-133">C#</span><span class="sxs-lookup"><span data-stu-id="ddbc3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-windowsprotectionstate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddbc3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddbc3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-windowsprotectionstate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddbc3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddbc3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-windowsprotectionstate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddbc3-136">Java</span><span class="sxs-lookup"><span data-stu-id="ddbc3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-windowsprotectionstate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ddbc3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddbc3-137">Response</span></span>
><span data-ttu-id="ddbc3-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ddbc3-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.windowsProtectionState)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/windowsProtectionStates",
    "value": [
        {
            "id": "34298981-4fc8-4974-9486-c8909ed1521b_95378ac4-eded-4671-8fa2-4e42e5de3463",
            "managedDeviceId": "95378ac4-eded-4671-8fa2-4e42e5de3463",
            "managedDeviceName": "vm11",
            "malwareProtectionEnabled": true,
            "managedDeviceHealthState": "Clean",
            "realTimeProtectionEnabled": true,
            "networkInspectionSystemEnabled": true,
            "quickScanOverdue": false,
            "fullScanOverdue": false,
            "signatureUpdateOverdue": false,
            "rebootRequired": false,
            "attentionRequired": false,
            "fullScanRequired": false,
            "engineVersion": "1.1.18300.4",
            "signatureVersion": "1.343.642.0",
            "antiMalwareVersion": "4.18.2106.6",
            "lastQuickScanDateTime": "2021-06-24T14:50:28Z",
            "lastFullScanDateTime": null,
            "lastQuickScanSignatureVersion": "1.341.1288.0",
            "lastFullScanSignatureVersion": "0.0.0.0",
            "lastReportedDateTime": "2021-07-09T14:43:45Z",
            "devicePropertiesRefreshTime": "2021-07-09T14:44:28Z",
            "deviceDeleted": false,
            "lastRefreshedDateTime": "2021-07-11T02:02:35.9816065Z",
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
            "tenantDisplayName": "Fourth Coffee",
            "devicePropertiesRefreshDateTime": "2021-07-09T14:44:28Z"
        },
        {
            "id": "38227791-a88b-4fcc-81c5-58cf77668320_49ed91f1-32ac-4881-9c1b-b709ba29e31b",
            "managedDeviceId": "49ed91f1-32ac-4881-9c1b-b709ba29e31b",
            "managedDeviceName": "VM4511",
            "malwareProtectionEnabled": true,
            "managedDeviceHealthState": "Clean",
            "realTimeProtectionEnabled": true,
            "networkInspectionSystemEnabled": true,
            "quickScanOverdue": false,
            "fullScanOverdue": false,
            "signatureUpdateOverdue": false,
            "rebootRequired": false,
            "attentionRequired": false,
            "fullScanRequired": false,
            "engineVersion": "1.1.18300.4",
            "signatureVersion": "1.343.618.0",
            "antiMalwareVersion": "4.18.2105.5",
            "lastQuickScanDateTime": "2021-06-21T15:05:41Z",
            "lastFullScanDateTime": "2021-04-19T20:03:26Z",
            "lastQuickScanSignatureVersion": "1.341.1157.0",
            "lastFullScanSignatureVersion": "1.303.25.0",
            "lastReportedDateTime": "2021-07-09T14:43:52Z",
            "devicePropertiesRefreshTime": "2021-07-09T14:44:28Z",
            "deviceDeleted": false,
            "lastRefreshedDateTime": "2021-07-11T02:02:35.9816065Z",
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
            "tenantDisplayName": "Consolidated Messenger",
            "devicePropertiesRefreshDateTime": "2021-07-09T14:44:28Z"
        }
    ]
}
```
