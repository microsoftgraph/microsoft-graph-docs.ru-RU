---
title: Перечисление объектов iosManagedAppRegistration
description: Список свойств и связей объектов iosManagedAppRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b929a2a01126b1ec1803f005be1bf4e14f63938
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193328"
---
# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="28050-103">Перечисление объектов iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="28050-103">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="28050-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28050-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28050-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28050-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28050-106">Список свойств и связей объектов [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="28050-106">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28050-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="28050-107">Prerequisites</span></span>
<span data-ttu-id="28050-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28050-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28050-110">Permission type</span></span>|<span data-ttu-id="28050-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28050-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28050-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28050-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28050-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="28050-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="28050-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28050-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28050-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28050-115">Not supported.</span></span>|
|<span data-ttu-id="28050-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28050-116">Application</span></span>|<span data-ttu-id="28050-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="28050-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28050-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28050-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="28050-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28050-119">Request headers</span></span>
|<span data-ttu-id="28050-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28050-120">Header</span></span>|<span data-ttu-id="28050-121">Значение</span><span class="sxs-lookup"><span data-stu-id="28050-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28050-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28050-122">Authorization</span></span>|<span data-ttu-id="28050-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28050-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28050-124">Accept</span><span class="sxs-lookup"><span data-stu-id="28050-124">Accept</span></span>|<span data-ttu-id="28050-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28050-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28050-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28050-126">Request body</span></span>
<span data-ttu-id="28050-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28050-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28050-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="28050-128">Response</span></span>
<span data-ttu-id="28050-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28050-129">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28050-130">Пример</span><span class="sxs-lookup"><span data-stu-id="28050-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="28050-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="28050-131">Request</span></span>
<span data-ttu-id="28050-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28050-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="28050-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="28050-133">Response</span></span>
<span data-ttu-id="28050-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28050-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




