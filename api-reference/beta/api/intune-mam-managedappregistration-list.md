---
title: Перечисление объектов managedAppRegistration
description: Список свойств и связей объектов managedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06bf7416ed8dd867c50f6175b0c3516a44ff4269
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177564"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="25d99-103">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="25d99-103">List managedAppRegistrations</span></span>

<span data-ttu-id="25d99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25d99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25d99-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25d99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25d99-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25d99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25d99-107">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="25d99-107">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25d99-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="25d99-108">Prerequisites</span></span>
<span data-ttu-id="25d99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25d99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25d99-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25d99-111">Permission type</span></span>|<span data-ttu-id="25d99-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25d99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25d99-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25d99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25d99-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="25d99-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="25d99-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25d99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25d99-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25d99-116">Not supported.</span></span>|
|<span data-ttu-id="25d99-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25d99-117">Application</span></span>|<span data-ttu-id="25d99-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="25d99-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25d99-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25d99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="25d99-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25d99-120">Request headers</span></span>
|<span data-ttu-id="25d99-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25d99-121">Header</span></span>|<span data-ttu-id="25d99-122">Значение</span><span class="sxs-lookup"><span data-stu-id="25d99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25d99-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25d99-123">Authorization</span></span>|<span data-ttu-id="25d99-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25d99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25d99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="25d99-125">Accept</span></span>|<span data-ttu-id="25d99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25d99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25d99-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25d99-127">Request body</span></span>
<span data-ttu-id="25d99-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25d99-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25d99-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="25d99-129">Response</span></span>
<span data-ttu-id="25d99-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="25d99-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25d99-131">Пример</span><span class="sxs-lookup"><span data-stu-id="25d99-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="25d99-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="25d99-132">Request</span></span>
<span data-ttu-id="25d99-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25d99-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="25d99-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="25d99-134">Response</span></span>
<span data-ttu-id="25d99-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25d99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1063

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppRegistration",
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
      "id": "5496aa60-aa60-5496-60aa-965460aa9654",
      "version": "Version value"
    }
  ]
}
```



