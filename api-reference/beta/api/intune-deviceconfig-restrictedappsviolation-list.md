---
title: Список restrictedAppsViolations
description: Свойства списка и связей объектов restrictedAppsViolation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 284eeac8ca2220058ac1233540d3d845b55d1bd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410184"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="3fb07-103">Список restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="3fb07-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="3fb07-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3fb07-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3fb07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fb07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fb07-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fb07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fb07-107">Свойства списка и связей объектов [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="3fb07-107">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fb07-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="3fb07-108">Prerequisites</span></span>
<span data-ttu-id="3fb07-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3fb07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3fb07-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fb07-111">Permission type</span></span>|<span data-ttu-id="3fb07-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fb07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fb07-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fb07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fb07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fb07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3fb07-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fb07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fb07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fb07-116">Not supported.</span></span>|
|<span data-ttu-id="3fb07-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fb07-117">Application</span></span>|<span data-ttu-id="3fb07-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fb07-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fb07-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fb07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="3fb07-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fb07-120">Request headers</span></span>
|<span data-ttu-id="3fb07-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fb07-121">Header</span></span>|<span data-ttu-id="3fb07-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3fb07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fb07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fb07-123">Authorization</span></span>|<span data-ttu-id="3fb07-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3fb07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fb07-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3fb07-125">Accept</span></span>|<span data-ttu-id="3fb07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fb07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fb07-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fb07-127">Request body</span></span>
<span data-ttu-id="3fb07-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fb07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fb07-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fb07-129">Response</span></span>
<span data-ttu-id="3fb07-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3fb07-130">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fb07-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3fb07-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fb07-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fb07-132">Request</span></span>
<span data-ttu-id="3fb07-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fb07-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="3fb07-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fb07-134">Response</span></span>
<span data-ttu-id="3fb07-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3fb07-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 710

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedAppsViolation",
      "id": "53f99903-9903-53f9-0399-f9530399f953",
      "userId": "User Id value",
      "userName": "User Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value",
      "deviceConfigurationId": "Device Configuration Id value",
      "deviceConfigurationName": "Device Configuration Name value",
      "platformType": "androidForWork",
      "restrictedAppsState": "notApprovedApps",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.managedDeviceReportedApp",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```




