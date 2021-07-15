---
title: Список устройствCompliancePolicySettingStateSummary
description: Получите список объектов deviceCompliancePolicySettingStateSummary и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: ec117e3f93732e3134f6451c83477eb342a98d39
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442026"
---
# <a name="list-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="f2b0c-103">Список устройствCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f2b0c-103">List deviceCompliancePolicySettingStateSummary</span></span>
<span data-ttu-id="f2b0c-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f2b0c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2b0c-105">Получите список объектов [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-105">Get a list of the [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2b0c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2b0c-106">Permissions</span></span>
<span data-ttu-id="f2b0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2b0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b0c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2b0c-109">Permission type</span></span>|<span data-ttu-id="f2b0c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2b0c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2b0c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2b0c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2b0c-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b0c-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f2b0c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2b0c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2b0c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-114">Not supported.</span></span>|
|<span data-ttu-id="f2b0c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2b0c-115">Application</span></span>|<span data-ttu-id="f2b0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2b0c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2b0c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2b0c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2b0c-118">Optional query parameters</span></span>
<span data-ttu-id="f2b0c-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="f2b0c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2b0c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2b0c-120">Request headers</span></span>
|<span data-ttu-id="f2b0c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f2b0c-121">Name</span></span>|<span data-ttu-id="f2b0c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f2b0c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2b0c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2b0c-123">Authorization</span></span>|<span data-ttu-id="f2b0c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2b0c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2b0c-126">Request body</span></span>
<span data-ttu-id="f2b0c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2b0c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2b0c-128">Response</span></span>

<span data-ttu-id="f2b0c-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2b0c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2b0c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2b0c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2b0c-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f2b0c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b0c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_devicecompliancepolicysettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary
```
# <a name="c"></a>[<span data-ttu-id="f2b0c-133">C#</span><span class="sxs-lookup"><span data-stu-id="f2b0c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-devicecompliancepolicysettingstatesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2b0c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2b0c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-devicecompliancepolicysettingstatesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2b0c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2b0c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-devicecompliancepolicysettingstatesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2b0c-136">Java</span><span class="sxs-lookup"><span data-stu-id="f2b0c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-devicecompliancepolicysettingstatesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f2b0c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2b0c-137">Response</span></span>
><span data-ttu-id="f2b0c-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
      "id": "9f6922d9-5a58-4f4d-b6e3-708f7659e5b2",
      "tenantId": "String",
      "tenantDisplayName": "String",
      "conflictDeviceCount": "Integer",
      "errorDeviceCount": "Integer",
      "failedDeviceCount": "Integer",
      "intuneAccountId": "String",
      "intuneSettingId": "String",
      "notApplicableDeviceCount": "Integer",
      "pendingDeviceCount": "Integer",
      "policyType": "String",
      "settingName": "String",
      "succeededDeviceCount": "Integer",
      "lastRefreshedDateTime": "String (timestamp)"
    }
  ]
}
```
