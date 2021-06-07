---
title: Перечисление объектов androidManagedAppRegistration
description: Список свойств и связей объектов androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 538b930d6a2799505298f06f932e059c2238a201
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756143"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="03c6f-103">Перечисление объектов androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="03c6f-103">List androidManagedAppRegistrations</span></span>

<span data-ttu-id="03c6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03c6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03c6f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03c6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03c6f-106">Список свойств и связей объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="03c6f-106">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03c6f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="03c6f-107">Prerequisites</span></span>
<span data-ttu-id="03c6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03c6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03c6f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03c6f-110">Permission type</span></span>|<span data-ttu-id="03c6f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03c6f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03c6f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03c6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03c6f-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03c6f-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="03c6f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03c6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03c6f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03c6f-115">Not supported.</span></span>|
|<span data-ttu-id="03c6f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="03c6f-116">Application</span></span>|<span data-ttu-id="03c6f-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03c6f-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03c6f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03c6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="03c6f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03c6f-119">Request headers</span></span>
|<span data-ttu-id="03c6f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03c6f-120">Header</span></span>|<span data-ttu-id="03c6f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="03c6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03c6f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="03c6f-122">Authorization</span></span>|<span data-ttu-id="03c6f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03c6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03c6f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="03c6f-124">Accept</span></span>|<span data-ttu-id="03c6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03c6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03c6f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03c6f-126">Request body</span></span>
<span data-ttu-id="03c6f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03c6f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03c6f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="03c6f-128">Response</span></span>
<span data-ttu-id="03c6f-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="03c6f-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03c6f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="03c6f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="03c6f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="03c6f-131">Request</span></span>
<span data-ttu-id="03c6f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03c6f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="03c6f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="03c6f-133">Response</span></span>
<span data-ttu-id="03c6f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03c6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

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
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value"
    }
  ]
}
```




