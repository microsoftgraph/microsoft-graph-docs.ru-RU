---
title: УправлениеDeviceCompliance
description: Ознакомьтесь с свойствами и отношениями объекта managedDeviceCompliance.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: be93e13c483e11327bfe5725d9b779cfccd89354
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402477"
---
# <a name="get-manageddevicecompliance"></a><span data-ttu-id="cd667-103">УправлениеDeviceCompliance</span><span class="sxs-lookup"><span data-stu-id="cd667-103">Get managedDeviceCompliance</span></span>
<span data-ttu-id="cd667-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="cd667-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd667-105">Ознакомьтесь с свойствами и отношениями объекта [managedDeviceCompliance.](../resources/managedtenants-manageddevicecompliance.md)</span><span class="sxs-lookup"><span data-stu-id="cd667-105">Read the properties and relationships of a [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd667-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd667-106">Permissions</span></span>
<span data-ttu-id="cd667-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd667-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd667-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd667-109">Permission type</span></span>|<span data-ttu-id="cd667-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd667-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd667-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd667-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cd667-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd667-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cd667-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd667-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd667-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd667-114">Not supported.</span></span>|
|<span data-ttu-id="cd667-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-115">Application</span></span>|<span data-ttu-id="cd667-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd667-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd667-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd667-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd667-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cd667-118">Optional query parameters</span></span>
<span data-ttu-id="cd667-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="cd667-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd667-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd667-120">Request headers</span></span>
|<span data-ttu-id="cd667-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cd667-121">Name</span></span>|<span data-ttu-id="cd667-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cd667-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cd667-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd667-123">Authorization</span></span>|<span data-ttu-id="cd667-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd667-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd667-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd667-126">Request body</span></span>
<span data-ttu-id="cd667-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd667-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd667-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd667-128">Response</span></span>

<span data-ttu-id="cd667-129">В случае успешного использования этот метод возвращает код отклика и `200 OK` [объект managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cd667-129">If successful, this method returns a `200 OK` response code and a [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd667-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="cd667-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cd667-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd667-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}
```


### <a name="response"></a><span data-ttu-id="cd667-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd667-132">Response</span></span>
><span data-ttu-id="cd667-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cd667-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceCompliance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managedDeviceCompliances/$entity",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b_95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceId": "95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceName": "vm11",
    "complianceStatus": "Compliant",
    "osDescription": "Windows",
    "osVersion": "10.0.19042.1083",
    "lastSyncDateTime": "2021-07-09T14:41:21.9130091Z",
    "ownerType": "Company",
    "model": "Virtual Machine",
    "manufacturer": "Microsoft Corporation",
    "inGracePeriodUntilDateTime": "9999-12-31T23:59:59.9999999Z",
    "lastRefreshedDateTime": "2021-07-11T07:12:41.0336556Z",
    "deviceType": "WindowsRT",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee"
}
```
