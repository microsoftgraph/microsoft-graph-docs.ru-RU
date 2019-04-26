---
title: Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration
description: Список свойств и связей объектов deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b0e374a83277df6d078464f7b9b116f71b575e9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561686"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="31016-103">Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="31016-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

> <span data-ttu-id="31016-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31016-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31016-105">Список свойств и связей объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31016-105">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31016-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="31016-106">Prerequisites</span></span>
<span data-ttu-id="31016-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31016-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31016-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31016-109">Permission type</span></span>|<span data-ttu-id="31016-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31016-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31016-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31016-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31016-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="31016-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="31016-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31016-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31016-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31016-114">Not supported.</span></span>|
|<span data-ttu-id="31016-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31016-115">Application</span></span>|<span data-ttu-id="31016-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31016-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31016-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31016-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="31016-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31016-118">Request headers</span></span>
|<span data-ttu-id="31016-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31016-119">Header</span></span>|<span data-ttu-id="31016-120">Значение</span><span class="sxs-lookup"><span data-stu-id="31016-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31016-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31016-121">Authorization</span></span>|<span data-ttu-id="31016-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31016-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31016-123">Accept</span><span class="sxs-lookup"><span data-stu-id="31016-123">Accept</span></span>|<span data-ttu-id="31016-124">application/json</span><span class="sxs-lookup"><span data-stu-id="31016-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31016-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31016-125">Request body</span></span>
<span data-ttu-id="31016-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31016-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31016-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="31016-127">Response</span></span>
<span data-ttu-id="31016-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="31016-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31016-129">Пример</span><span class="sxs-lookup"><span data-stu-id="31016-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="31016-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="31016-130">Request</span></span>
<span data-ttu-id="31016-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31016-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="31016-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="31016-132">Response</span></span>
<span data-ttu-id="31016-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31016-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2027

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
        "osMaximumVersion": "Os Maximum Version value"
      },
      "windowsRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "windowsMobileRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "androidRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "macOSRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      }
    }
  ]
}
```



