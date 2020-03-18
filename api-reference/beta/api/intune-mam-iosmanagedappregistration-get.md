---
title: Get iosManagedAppRegistration
description: Чтение свойств и связей объекта iosManagedAppRegistration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39cb2b8157d8bd518f7d32e0caf84553f310fcca
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803640"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="e76f9-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e76f9-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="e76f9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e76f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e76f9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e76f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e76f9-106">Чтение свойств и связей объекта [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e76f9-106">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e76f9-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e76f9-107">Prerequisites</span></span>
<span data-ttu-id="e76f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e76f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e76f9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e76f9-110">Permission type</span></span>|<span data-ttu-id="e76f9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e76f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e76f9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e76f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e76f9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e76f9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e76f9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e76f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e76f9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e76f9-115">Not supported.</span></span>|
|<span data-ttu-id="e76f9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e76f9-116">Application</span></span>|<span data-ttu-id="e76f9-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e76f9-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e76f9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e76f9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e76f9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e76f9-119">Optional query parameters</span></span>
<span data-ttu-id="e76f9-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e76f9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e76f9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e76f9-121">Request headers</span></span>
|<span data-ttu-id="e76f9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e76f9-122">Header</span></span>|<span data-ttu-id="e76f9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e76f9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e76f9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e76f9-124">Authorization</span></span>|<span data-ttu-id="e76f9-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e76f9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e76f9-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e76f9-126">Accept</span></span>|<span data-ttu-id="e76f9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e76f9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e76f9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e76f9-128">Request body</span></span>
<span data-ttu-id="e76f9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e76f9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e76f9-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e76f9-130">Response</span></span>
<span data-ttu-id="e76f9-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e76f9-131">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e76f9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e76f9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e76f9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e76f9-133">Request</span></span>
<span data-ttu-id="e76f9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e76f9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="e76f9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e76f9-135">Response</span></span>
<span data-ttu-id="e76f9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e76f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

{
  "value": {
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
}
```




