---
title: Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration
description: Список свойств и связей объектов deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a71cd00a47fb4547c05ba986f3459b9e3d26d04c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978762"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="38687-103">Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="38687-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

> <span data-ttu-id="38687-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="38687-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38687-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38687-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38687-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="38687-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38687-107">Список свойств и связей объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38687-107">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38687-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="38687-108">Prerequisites</span></span>
<span data-ttu-id="38687-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38687-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38687-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38687-111">Permission type</span></span>|<span data-ttu-id="38687-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38687-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38687-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38687-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38687-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="38687-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="38687-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38687-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38687-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38687-116">Not supported.</span></span>|
|<span data-ttu-id="38687-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38687-117">Application</span></span>|<span data-ttu-id="38687-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38687-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38687-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38687-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="38687-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38687-120">Request headers</span></span>
|<span data-ttu-id="38687-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38687-121">Header</span></span>|<span data-ttu-id="38687-122">Значение</span><span class="sxs-lookup"><span data-stu-id="38687-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38687-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38687-123">Authorization</span></span>|<span data-ttu-id="38687-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="38687-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38687-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38687-125">Accept</span></span>|<span data-ttu-id="38687-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38687-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38687-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38687-127">Request body</span></span>
<span data-ttu-id="38687-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38687-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38687-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="38687-129">Response</span></span>
<span data-ttu-id="38687-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="38687-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38687-131">Пример</span><span class="sxs-lookup"><span data-stu-id="38687-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="38687-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="38687-132">Request</span></span>
<span data-ttu-id="38687-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38687-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="38687-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="38687-134">Response</span></span>
<span data-ttu-id="38687-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="38687-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2664

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
      "androidForWorkRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "macRestriction": {
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





