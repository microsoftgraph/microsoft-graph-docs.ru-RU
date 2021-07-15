---
title: Get deviceCompliancePolicySettingStateSummary
description: Ознакомьтесь с свойствами и отношениями объекта deviceCompliancePolicySettingStateSummary.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 6e94a2f241f78112b08146e5bb639a4966c5a24f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439998"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="f47df-103">Get deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f47df-103">Get deviceCompliancePolicySettingStateSummary</span></span>
<span data-ttu-id="f47df-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f47df-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f47df-105">Ознакомьтесь с свойствами и отношениями [объекта deviceCompliancePolicySettingStateSummary.](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f47df-105">Read the properties and relationships of a [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f47df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f47df-106">Permissions</span></span>
<span data-ttu-id="f47df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f47df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f47df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f47df-109">Permission type</span></span>|<span data-ttu-id="f47df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f47df-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f47df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f47df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f47df-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f47df-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f47df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f47df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f47df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f47df-114">Not supported.</span></span>|
|<span data-ttu-id="f47df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f47df-115">Application</span></span>|<span data-ttu-id="f47df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f47df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f47df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f47df-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummarys/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f47df-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f47df-118">Optional query parameters</span></span>
<span data-ttu-id="f47df-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="f47df-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f47df-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f47df-120">Request headers</span></span>
|<span data-ttu-id="f47df-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f47df-121">Name</span></span>|<span data-ttu-id="f47df-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f47df-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f47df-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f47df-123">Authorization</span></span>|<span data-ttu-id="f47df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f47df-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f47df-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f47df-126">Request body</span></span>
<span data-ttu-id="f47df-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f47df-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f47df-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f47df-128">Response</span></span>

<span data-ttu-id="f47df-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f47df-129">If successful, this method returns a `200 OK` response code and a [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f47df-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f47df-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f47df-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f47df-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f47df-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f47df-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devicecompliancepolicysettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummarys/{deviceCompliancePolicySettingStateSummaryId}
```
# <a name="c"></a>[<span data-ttu-id="f47df-133">C#</span><span class="sxs-lookup"><span data-stu-id="f47df-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devicecompliancepolicysettingstatesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f47df-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f47df-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devicecompliancepolicysettingstatesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f47df-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f47df-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devicecompliancepolicysettingstatesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f47df-136">Java</span><span class="sxs-lookup"><span data-stu-id="f47df-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devicecompliancepolicysettingstatesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f47df-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f47df-137">Response</span></span>
><span data-ttu-id="f47df-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f47df-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
