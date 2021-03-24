---
title: Перечисление объектов iosManagedAppRegistration
description: Список свойств и связей объектов iosManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c143b9670c74feac60ea810050aa899da28b874b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149368"
---
# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="15078-103">Перечисление объектов iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="15078-103">List iosManagedAppRegistrations</span></span>

<span data-ttu-id="15078-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15078-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15078-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15078-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15078-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15078-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15078-107">Список свойств и связей объектов [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="15078-107">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15078-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="15078-108">Prerequisites</span></span>
<span data-ttu-id="15078-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15078-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15078-111">Permission type</span></span>|<span data-ttu-id="15078-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15078-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15078-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15078-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15078-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15078-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15078-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15078-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15078-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15078-116">Not supported.</span></span>|
|<span data-ttu-id="15078-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="15078-117">Application</span></span>|<span data-ttu-id="15078-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15078-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15078-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15078-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="15078-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15078-120">Request headers</span></span>
|<span data-ttu-id="15078-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15078-121">Header</span></span>|<span data-ttu-id="15078-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15078-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15078-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15078-123">Authorization</span></span>|<span data-ttu-id="15078-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15078-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15078-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15078-125">Accept</span></span>|<span data-ttu-id="15078-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15078-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15078-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15078-127">Request body</span></span>
<span data-ttu-id="15078-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15078-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15078-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="15078-129">Response</span></span>
<span data-ttu-id="15078-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="15078-130">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15078-131">Пример</span><span class="sxs-lookup"><span data-stu-id="15078-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="15078-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="15078-132">Request</span></span>
<span data-ttu-id="15078-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15078-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="15078-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="15078-134">Response</span></span>
<span data-ttu-id="15078-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15078-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1060

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "managedDeviceId": "Managed Device Id value",
      "azureADDeviceId": "Azure ADDevice Id value",
      "deviceModel": "Device Model value",
      "deviceManufacturer": "Device Manufacturer value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
        "bundleId": "Bundle Id value"
      },
      "id": "47632c19-2c19-4763-192c-6347192c6347",
      "version": "Version value"
    }
  ]
}
```




