---
title: Перечисление объектов managedAppRegistration
description: Список свойств и связей объектов managedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f01663649e8f12008a9de1b17fcf155b5338190
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149095"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="28781-103">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="28781-103">List managedAppRegistrations</span></span>

<span data-ttu-id="28781-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28781-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28781-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28781-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28781-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28781-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28781-107">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="28781-107">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28781-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="28781-108">Prerequisites</span></span>
<span data-ttu-id="28781-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28781-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28781-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28781-111">Permission type</span></span>|<span data-ttu-id="28781-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28781-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28781-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28781-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28781-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28781-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28781-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28781-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28781-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28781-116">Not supported.</span></span>|
|<span data-ttu-id="28781-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="28781-117">Application</span></span>|<span data-ttu-id="28781-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28781-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28781-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28781-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="28781-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28781-120">Request headers</span></span>
|<span data-ttu-id="28781-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28781-121">Header</span></span>|<span data-ttu-id="28781-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28781-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28781-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28781-123">Authorization</span></span>|<span data-ttu-id="28781-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28781-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28781-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28781-125">Accept</span></span>|<span data-ttu-id="28781-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28781-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28781-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28781-127">Request body</span></span>
<span data-ttu-id="28781-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28781-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28781-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="28781-129">Response</span></span>
<span data-ttu-id="28781-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28781-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28781-131">Пример</span><span class="sxs-lookup"><span data-stu-id="28781-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="28781-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="28781-132">Request</span></span>
<span data-ttu-id="28781-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28781-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="28781-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="28781-134">Response</span></span>
<span data-ttu-id="28781-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28781-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1064

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
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "id": "5496aa60-aa60-5496-60aa-965460aa9654",
      "version": "Version value"
    }
  ]
}
```




