---
title: Get managedDeviceOverview
description: Чтение свойств и связей объекта managedDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35b91b36bfaf190a69c8f4d78d717e5c71cb312a
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122709"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="e2ca1-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e2ca1-103">Get managedDeviceOverview</span></span>

<span data-ttu-id="e2ca1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2ca1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2ca1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2ca1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2ca1-107">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="e2ca1-107">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2ca1-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e2ca1-108">Prerequisites</span></span>
<span data-ttu-id="e2ca1-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e2ca1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2ca1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2ca1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2ca1-111">Permission type</span></span>|<span data-ttu-id="e2ca1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2ca1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2ca1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2ca1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2ca1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2ca1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e2ca1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2ca1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2ca1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-116">Not supported.</span></span>|
|<span data-ttu-id="e2ca1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2ca1-117">Application</span></span>|<span data-ttu-id="e2ca1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2ca1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2ca1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2ca1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2ca1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e2ca1-120">Optional query parameters</span></span>
<span data-ttu-id="e2ca1-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2ca1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2ca1-122">Request headers</span></span>
|<span data-ttu-id="e2ca1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2ca1-123">Header</span></span>|<span data-ttu-id="e2ca1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e2ca1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2ca1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2ca1-125">Authorization</span></span>|<span data-ttu-id="e2ca1-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2ca1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e2ca1-127">Accept</span></span>|<span data-ttu-id="e2ca1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e2ca1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2ca1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2ca1-129">Request body</span></span>
<span data-ttu-id="e2ca1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2ca1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2ca1-131">Response</span></span>
<span data-ttu-id="e2ca1-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-132">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2ca1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e2ca1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2ca1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2ca1-134">Request</span></span>
<span data-ttu-id="e2ca1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="e2ca1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2ca1-136">Response</span></span>
<span data-ttu-id="e2ca1-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-137">Here is an example of the response.</span></span> <span data-ttu-id="e2ca1-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e2ca1-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e2ca1-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1366

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceOverview",
    "id": "42a91653-1653-42a9-5316-a9425316a942",
    "enrolledDeviceCount": 3,
    "mdmEnrolledCount": 0,
    "dualEnrolledDeviceCount": 7,
    "deviceOperatingSystemSummary": {
      "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
      "androidCount": 12,
      "iosCount": 8,
      "macOSCount": 10,
      "windowsMobileCount": 2,
      "windowsCount": 12,
      "unknownCount": 12,
      "androidDedicatedCount": 5,
      "androidDeviceAdminCount": 7,
      "androidFullyManagedCount": 8,
      "androidWorkProfileCount": 7,
      "androidCorporateWorkProfileCount": 0,
      "configMgrDeviceCount": 4
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    },
    "managedDeviceModelsAndManufacturers": {
      "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
      "deviceModels": [
        "Device Models value"
      ],
      "deviceManufacturers": [
        "Device Manufacturers value"
      ]
    },
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```



