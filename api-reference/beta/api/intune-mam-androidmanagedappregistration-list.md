---
title: Перечисление объектов androidManagedAppRegistration
description: Список свойств и связей объектов androidManagedAppRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b63189ebeb25b4135bc60718de997413225576e5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980056"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="eb9b8-103">Перечисление объектов androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="eb9b8-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="eb9b8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb9b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb9b8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb9b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb9b8-106">Список свойств и связей объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="eb9b8-106">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb9b8-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eb9b8-107">Prerequisites</span></span>
<span data-ttu-id="eb9b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb9b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb9b8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb9b8-110">Permission type</span></span>|<span data-ttu-id="eb9b8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb9b8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb9b8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb9b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb9b8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb9b8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eb9b8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb9b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb9b8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb9b8-115">Not supported.</span></span>|
|<span data-ttu-id="eb9b8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb9b8-116">Application</span></span>|<span data-ttu-id="eb9b8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb9b8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb9b8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb9b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="eb9b8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb9b8-119">Request headers</span></span>
|<span data-ttu-id="eb9b8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb9b8-120">Header</span></span>|<span data-ttu-id="eb9b8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eb9b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb9b8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb9b8-122">Authorization</span></span>|<span data-ttu-id="eb9b8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb9b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb9b8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eb9b8-124">Accept</span></span>|<span data-ttu-id="eb9b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb9b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb9b8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb9b8-126">Request body</span></span>
<span data-ttu-id="eb9b8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb9b8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb9b8-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb9b8-128">Response</span></span>
<span data-ttu-id="eb9b8-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eb9b8-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb9b8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="eb9b8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb9b8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb9b8-131">Request</span></span>
<span data-ttu-id="eb9b8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb9b8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="eb9b8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb9b8-133">Response</span></span>
<span data-ttu-id="eb9b8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb9b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





