---
title: Get androidManagedAppRegistration
description: Чтение свойств и связей объекта androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 17c2356e5a21ca725d67b7929ba52703abbae0d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43391781"
---
# <a name="get-androidmanagedappregistration"></a><span data-ttu-id="a6d1b-103">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a6d1b-103">Get androidManagedAppRegistration</span></span>

<span data-ttu-id="a6d1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6d1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6d1b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6d1b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6d1b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6d1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6d1b-107">Чтение свойств и связей объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a6d1b-107">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6d1b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a6d1b-108">Prerequisites</span></span>
<span data-ttu-id="a6d1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6d1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6d1b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6d1b-111">Permission type</span></span>|<span data-ttu-id="a6d1b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6d1b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6d1b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6d1b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6d1b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6d1b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a6d1b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6d1b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6d1b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6d1b-116">Not supported.</span></span>|
|<span data-ttu-id="a6d1b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6d1b-117">Application</span></span>|<span data-ttu-id="a6d1b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6d1b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6d1b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6d1b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6d1b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6d1b-120">Optional query parameters</span></span>
<span data-ttu-id="a6d1b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a6d1b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6d1b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6d1b-122">Request headers</span></span>
|<span data-ttu-id="a6d1b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6d1b-123">Header</span></span>|<span data-ttu-id="a6d1b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a6d1b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6d1b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6d1b-125">Authorization</span></span>|<span data-ttu-id="a6d1b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6d1b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6d1b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a6d1b-127">Accept</span></span>|<span data-ttu-id="a6d1b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a6d1b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6d1b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6d1b-129">Request body</span></span>
<span data-ttu-id="a6d1b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6d1b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6d1b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6d1b-131">Response</span></span>
<span data-ttu-id="a6d1b-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a6d1b-132">If successful, this method returns a `200 OK` response code and [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6d1b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a6d1b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6d1b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6d1b-134">Request</span></span>
<span data-ttu-id="a6d1b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6d1b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="a6d1b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6d1b-136">Response</span></span>
<span data-ttu-id="a6d1b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6d1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

{
  "value": {
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
}
```



