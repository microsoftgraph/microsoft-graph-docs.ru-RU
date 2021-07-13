---
title: Get managedDeviceComplianceTrend
description: Ознакомьтесь с свойствами и отношениями объекта managedDeviceComplianceTrend.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 046b110c0aad542db3994bc6eecbba9b1d414feb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402472"
---
# <a name="get-manageddevicecompliancetrend"></a><span data-ttu-id="3a353-103">Get managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="3a353-103">Get managedDeviceComplianceTrend</span></span>
<span data-ttu-id="3a353-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="3a353-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a353-105">Ознакомьтесь с свойствами и отношениями объекта [managedDeviceComplianceTrend.](../resources/managedtenants-manageddevicecompliancetrend.md)</span><span class="sxs-lookup"><span data-stu-id="3a353-105">Read the properties and relationships of a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a353-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a353-106">Permissions</span></span>
<span data-ttu-id="3a353-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a353-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a353-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a353-109">Permission type</span></span>|<span data-ttu-id="3a353-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a353-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a353-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a353-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a353-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a353-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3a353-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a353-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a353-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a353-114">Not supported.</span></span>|
|<span data-ttu-id="3a353-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a353-115">Application</span></span>|<span data-ttu-id="3a353-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a353-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a353-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a353-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a353-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a353-118">Optional query parameters</span></span>
<span data-ttu-id="3a353-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="3a353-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a353-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a353-120">Request headers</span></span>
|<span data-ttu-id="3a353-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3a353-121">Name</span></span>|<span data-ttu-id="3a353-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3a353-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3a353-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a353-123">Authorization</span></span>|<span data-ttu-id="3a353-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a353-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a353-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a353-126">Request body</span></span>
<span data-ttu-id="3a353-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a353-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a353-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a353-128">Response</span></span>

<span data-ttu-id="3a353-129">В случае успешного использования этот метод возвращает код ответа и объект `200 OK` [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3a353-129">If successful, this method returns a `200 OK` response code and a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a353-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a353-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a353-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a353-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecompliancetrend"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```


### <a name="response"></a><span data-ttu-id="3a353-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a353-132">Response</span></span>
><span data-ttu-id="3a353-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a353-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b_2021-07-11T00:00:00Z",
  "tenantDisplayName": "Fourth Coffee",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "unknownDeviceCount": 2,
  "compliantDeviceCount": 0,
  "noncompliantDeviceCount": 41,
  "errorDeviceCount": 1,
  "inGracePeriodDeviceCount": 0,
  "configManagerDeviceCount": 0,
  "totalDeviceCount": 44,
  "countDateTime": "2021-07-11T00:00:00Z"
}
```
