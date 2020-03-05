---
title: Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration
description: Список свойств и связей объектов deviceEnrollmentPlatformRestrictionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27c1aea8a603bea38c61aa65f3a7d20db097487f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462371"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="4f73f-103">Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f73f-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

<span data-ttu-id="4f73f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4f73f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f73f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f73f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f73f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f73f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f73f-107">Список свойств и связей объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f73f-107">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f73f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f73f-108">Prerequisites</span></span>
<span data-ttu-id="4f73f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f73f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f73f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f73f-111">Permission type</span></span>|<span data-ttu-id="4f73f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f73f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f73f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f73f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f73f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f73f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4f73f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f73f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f73f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f73f-116">Not supported.</span></span>|
|<span data-ttu-id="4f73f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f73f-117">Application</span></span>|<span data-ttu-id="4f73f-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f73f-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f73f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f73f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4f73f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f73f-120">Request headers</span></span>
|<span data-ttu-id="4f73f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f73f-121">Header</span></span>|<span data-ttu-id="4f73f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4f73f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f73f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f73f-123">Authorization</span></span>|<span data-ttu-id="4f73f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f73f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f73f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f73f-125">Accept</span></span>|<span data-ttu-id="4f73f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f73f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f73f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f73f-127">Request body</span></span>
<span data-ttu-id="4f73f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f73f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f73f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f73f-129">Response</span></span>
<span data-ttu-id="4f73f-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4f73f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f73f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4f73f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f73f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f73f-132">Request</span></span>
<span data-ttu-id="4f73f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f73f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="4f73f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f73f-134">Response</span></span>
<span data-ttu-id="4f73f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f73f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3280

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
      "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "iosRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "windowsRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "windowsMobileRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "androidRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "androidForWorkRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "macRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "macOSRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      }
    }
  ]
}
```





