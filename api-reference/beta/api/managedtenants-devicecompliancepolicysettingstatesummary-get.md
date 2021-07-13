---
title: Get deviceCompliancePolicySettingStateSummary
description: Ознакомьтесь с свойствами и отношениями объекта deviceCompliancePolicySettingStateSummary.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e1396b66dda6925be6c895aac741d81122d64c98
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402478"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="dc2b7-103">Get deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="dc2b7-103">Get deviceCompliancePolicySettingStateSummary</span></span>
<span data-ttu-id="dc2b7-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="dc2b7-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc2b7-105">Ознакомьтесь с свойствами и отношениями [объекта deviceCompliancePolicySettingStateSummary.](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="dc2b7-105">Read the properties and relationships of a [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc2b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc2b7-106">Permissions</span></span>
<span data-ttu-id="dc2b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc2b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc2b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc2b7-109">Permission type</span></span>|<span data-ttu-id="dc2b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc2b7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc2b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc2b7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc2b7-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc2b7-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc2b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc2b7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc2b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc2b7-114">Not supported.</span></span>|
|<span data-ttu-id="dc2b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc2b7-115">Application</span></span>|<span data-ttu-id="dc2b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc2b7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc2b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc2b7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummarys/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc2b7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dc2b7-118">Optional query parameters</span></span>
<span data-ttu-id="dc2b7-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="dc2b7-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc2b7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc2b7-120">Request headers</span></span>
|<span data-ttu-id="dc2b7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dc2b7-121">Name</span></span>|<span data-ttu-id="dc2b7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dc2b7-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc2b7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc2b7-123">Authorization</span></span>|<span data-ttu-id="dc2b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc2b7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc2b7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc2b7-126">Request body</span></span>
<span data-ttu-id="dc2b7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc2b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc2b7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc2b7-128">Response</span></span>

<span data-ttu-id="dc2b7-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dc2b7-129">If successful, this method returns a `200 OK` response code and a [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc2b7-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="dc2b7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc2b7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc2b7-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devicecompliancepolicysettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummarys/{deviceCompliancePolicySettingStateSummaryId}
```


### <a name="response"></a><span data-ttu-id="dc2b7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc2b7-132">Response</span></span>
><span data-ttu-id="dc2b7-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dc2b7-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b_277f9230-81f7-ffc3-af78-4662ec3dca09",
    "intuneAccountId": "6f3e6534-b466-4fac-9a31-4c305cc40833",
    "intuneSettingId": "277f9230-81f7-ffc3-af78-4662ec3dca09",
    "policyType": "DefaultDeviceCompliancePolicy",
    "settingName": "RequireDeviceCompliancePolicyAssigned",
    "failedDeviceCount": 0,
    "errorDeviceCount": 4,
    "conflictDeviceCount": 0,
    "lastRefreshedDateTime": "2021-07-11T00:00:00Z",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee"
}
```
