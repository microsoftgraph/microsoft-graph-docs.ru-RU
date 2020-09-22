---
title: Перечисление объектов androidManagedAppRegistration
description: Список свойств и связей объектов androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b7dac2c597007cccf14b36a7a56ce3df3188bbc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000352"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="83942-103">Перечисление объектов androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="83942-103">List androidManagedAppRegistrations</span></span>

<span data-ttu-id="83942-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83942-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83942-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83942-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83942-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83942-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83942-107">Список свойств и связей объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="83942-107">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83942-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="83942-108">Prerequisites</span></span>
<span data-ttu-id="83942-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83942-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83942-111">Permission type</span></span>|<span data-ttu-id="83942-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83942-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83942-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83942-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83942-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="83942-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="83942-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83942-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83942-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83942-116">Not supported.</span></span>|
|<span data-ttu-id="83942-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83942-117">Application</span></span>|<span data-ttu-id="83942-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="83942-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83942-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83942-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="83942-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="83942-120">Request headers</span></span>
|<span data-ttu-id="83942-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83942-121">Header</span></span>|<span data-ttu-id="83942-122">Значение</span><span class="sxs-lookup"><span data-stu-id="83942-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83942-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83942-123">Authorization</span></span>|<span data-ttu-id="83942-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83942-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83942-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83942-125">Accept</span></span>|<span data-ttu-id="83942-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83942-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83942-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83942-127">Request body</span></span>
<span data-ttu-id="83942-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83942-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83942-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="83942-129">Response</span></span>
<span data-ttu-id="83942-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="83942-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83942-131">Пример</span><span class="sxs-lookup"><span data-stu-id="83942-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="83942-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="83942-132">Request</span></span>
<span data-ttu-id="83942-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83942-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="83942-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="83942-134">Response</span></span>
<span data-ttu-id="83942-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83942-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1116

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value",
      "patchVersion": "Patch Version value"
    }
  ]
}
```






