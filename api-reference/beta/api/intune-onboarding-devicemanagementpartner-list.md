---
title: Список объектов deviceManagementPartner
description: Список свойств и связей объектов deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9813361f4748d260a8b9cd503f9430fed1a6c7da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000037"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="91212-103">Список объектов deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="91212-103">List deviceManagementPartners</span></span>

<span data-ttu-id="91212-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91212-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91212-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91212-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91212-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91212-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91212-107">Список свойств и связей объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="91212-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91212-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="91212-108">Prerequisites</span></span>
<span data-ttu-id="91212-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91212-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91212-111">Permission type</span></span>|<span data-ttu-id="91212-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91212-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91212-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91212-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91212-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="91212-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="91212-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91212-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91212-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91212-116">Not supported.</span></span>|
|<span data-ttu-id="91212-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91212-117">Application</span></span>|<span data-ttu-id="91212-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="91212-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91212-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91212-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="91212-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="91212-120">Request headers</span></span>
|<span data-ttu-id="91212-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91212-121">Header</span></span>|<span data-ttu-id="91212-122">Значение</span><span class="sxs-lookup"><span data-stu-id="91212-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91212-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91212-123">Authorization</span></span>|<span data-ttu-id="91212-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91212-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91212-125">Accept</span><span class="sxs-lookup"><span data-stu-id="91212-125">Accept</span></span>|<span data-ttu-id="91212-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91212-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91212-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91212-127">Request body</span></span>
<span data-ttu-id="91212-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91212-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91212-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="91212-129">Response</span></span>
<span data-ttu-id="91212-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91212-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91212-131">Пример</span><span class="sxs-lookup"><span data-stu-id="91212-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="91212-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="91212-132">Request</span></span>
<span data-ttu-id="91212-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91212-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="91212-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="91212-134">Response</span></span>
<span data-ttu-id="91212-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91212-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1242

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "partnerAppType": "singleTenantApp",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
      "groupsRequiringPartnerEnrollment": [
        {
          "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
            "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
            "deviceAndAppManagementAssignmentFilterType": "include"
          }
        }
      ]
    }
  ]
}
```






