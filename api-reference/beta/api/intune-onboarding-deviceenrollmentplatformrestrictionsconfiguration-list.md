---
title: Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration
description: Список свойств и связей объектов deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76f7f0a6c927df04c9d9ec5a0c6052d0f13779ad
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158880"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="98ca8-103">Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="98ca8-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

<span data-ttu-id="98ca8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98ca8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98ca8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98ca8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98ca8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98ca8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98ca8-107">Список свойств и связей объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="98ca8-107">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98ca8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="98ca8-108">Prerequisites</span></span>
<span data-ttu-id="98ca8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98ca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98ca8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98ca8-111">Permission type</span></span>|<span data-ttu-id="98ca8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98ca8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98ca8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98ca8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98ca8-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98ca8-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="98ca8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98ca8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98ca8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98ca8-116">Not supported.</span></span>|
|<span data-ttu-id="98ca8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="98ca8-117">Application</span></span>|<span data-ttu-id="98ca8-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98ca8-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98ca8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98ca8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="98ca8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98ca8-120">Request headers</span></span>
|<span data-ttu-id="98ca8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98ca8-121">Header</span></span>|<span data-ttu-id="98ca8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98ca8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98ca8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98ca8-123">Authorization</span></span>|<span data-ttu-id="98ca8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98ca8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98ca8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98ca8-125">Accept</span></span>|<span data-ttu-id="98ca8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98ca8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98ca8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98ca8-127">Request body</span></span>
<span data-ttu-id="98ca8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98ca8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98ca8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="98ca8-129">Response</span></span>
<span data-ttu-id="98ca8-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="98ca8-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98ca8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="98ca8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="98ca8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="98ca8-132">Request</span></span>
<span data-ttu-id="98ca8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98ca8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="98ca8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="98ca8-134">Response</span></span>
<span data-ttu-id="98ca8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98ca8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4798

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
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "iosRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ],
        "blockedSkus": [
          "Blocked Skus value"
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
        ],
        "blockedSkus": [
          "Blocked Skus value"
        ]
      },
      "windowsHomeSkuRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ],
        "blockedSkus": [
          "Blocked Skus value"
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
        ],
        "blockedSkus": [
          "Blocked Skus value"
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
        ],
        "blockedSkus": [
          "Blocked Skus value"
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
        ],
        "blockedSkus": [
          "Blocked Skus value"
        ]
      },
      "aospRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ],
        "blockedSkus": [
          "Blocked Skus value"
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
        ],
        "blockedSkus": [
          "Blocked Skus value"
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
        ],
        "blockedSkus": [
          "Blocked Skus value"
        ]
      }
    }
  ]
}
```




