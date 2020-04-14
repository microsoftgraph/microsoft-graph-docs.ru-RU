---
title: Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration
description: Список свойств и связей объектов deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 098142fc9b67d25f01a5a6661926f62377703a22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450412"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="4803a-103">Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4803a-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

<span data-ttu-id="4803a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4803a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4803a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4803a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4803a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4803a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4803a-107">Список свойств и связей объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4803a-107">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4803a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4803a-108">Prerequisites</span></span>
<span data-ttu-id="4803a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4803a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4803a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4803a-111">Permission type</span></span>|<span data-ttu-id="4803a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4803a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4803a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4803a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4803a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4803a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4803a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4803a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4803a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4803a-116">Not supported.</span></span>|
|<span data-ttu-id="4803a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4803a-117">Application</span></span>|<span data-ttu-id="4803a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4803a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4803a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4803a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4803a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4803a-120">Request headers</span></span>
|<span data-ttu-id="4803a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4803a-121">Header</span></span>|<span data-ttu-id="4803a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4803a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4803a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4803a-123">Authorization</span></span>|<span data-ttu-id="4803a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4803a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4803a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4803a-125">Accept</span></span>|<span data-ttu-id="4803a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4803a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4803a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4803a-127">Request body</span></span>
<span data-ttu-id="4803a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4803a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4803a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4803a-129">Response</span></span>
<span data-ttu-id="4803a-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4803a-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4803a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4803a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4803a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4803a-132">Request</span></span>
<span data-ttu-id="4803a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4803a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="4803a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4803a-134">Response</span></span>
<span data-ttu-id="4803a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4803a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



