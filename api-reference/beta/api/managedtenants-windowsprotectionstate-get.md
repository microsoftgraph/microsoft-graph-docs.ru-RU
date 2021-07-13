---
title: Get windowsProtectionState
description: Ознакомьтесь с свойствами и отношениями объекта windowsProtectionState.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: dc82bbc7dfa7265471cbc6b99f1463d59db5b526
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403100"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="2ade4-103">Get windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="2ade4-103">Get windowsProtectionState</span></span>
<span data-ttu-id="2ade4-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2ade4-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ade4-105">Ознакомьтесь с свойствами и отношениями [объекта windowsProtectionState.](../resources/managedtenants-windowsprotectionstate.md)</span><span class="sxs-lookup"><span data-stu-id="2ade4-105">Read the properties and relationships of a [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ade4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ade4-106">Permissions</span></span>
<span data-ttu-id="2ade4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ade4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ade4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ade4-109">Permission type</span></span>|<span data-ttu-id="2ade4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ade4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ade4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ade4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ade4-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ade4-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2ade4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ade4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ade4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ade4-114">Not supported.</span></span>|
|<span data-ttu-id="2ade4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ade4-115">Application</span></span>|<span data-ttu-id="2ade4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ade4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ade4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ade4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ade4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2ade4-118">Optional query parameters</span></span>
<span data-ttu-id="2ade4-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="2ade4-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ade4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ade4-120">Request headers</span></span>
|<span data-ttu-id="2ade4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2ade4-121">Name</span></span>|<span data-ttu-id="2ade4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2ade4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2ade4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ade4-123">Authorization</span></span>|<span data-ttu-id="2ade4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ade4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ade4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ade4-126">Request body</span></span>
<span data-ttu-id="2ade4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ade4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ade4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ade4-128">Response</span></span>

<span data-ttu-id="2ade4-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект WindowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2ade4-129">If successful, this method returns a `200 OK` response code and a [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ade4-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ade4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ade4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ade4-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_windowsprotectionstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}
```


### <a name="response"></a><span data-ttu-id="2ade4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ade4-132">Response</span></span>
><span data-ttu-id="2ade4-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ade4-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.windowsProtectionState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/windowsProtectionStates/$entity",
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
}
```
