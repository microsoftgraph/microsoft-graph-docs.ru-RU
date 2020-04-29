---
title: Get managedDeviceOverview
description: Чтение свойств и связей объекта managedDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5051f4a3bb1b75b610ab913415b94fe2861a033
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474407"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="1a7bb-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1a7bb-103">Get managedDeviceOverview</span></span>

<span data-ttu-id="1a7bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a7bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a7bb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a7bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a7bb-106">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="1a7bb-106">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a7bb-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1a7bb-107">Prerequisites</span></span>
<span data-ttu-id="1a7bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a7bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a7bb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a7bb-110">Permission type</span></span>|<span data-ttu-id="1a7bb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a7bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a7bb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a7bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a7bb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a7bb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1a7bb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a7bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a7bb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a7bb-115">Not supported.</span></span>|
|<span data-ttu-id="1a7bb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a7bb-116">Application</span></span>|<span data-ttu-id="1a7bb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a7bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a7bb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a7bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a7bb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1a7bb-119">Optional query parameters</span></span>
<span data-ttu-id="1a7bb-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1a7bb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a7bb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a7bb-121">Request headers</span></span>
|<span data-ttu-id="1a7bb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a7bb-122">Header</span></span>|<span data-ttu-id="1a7bb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1a7bb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a7bb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a7bb-124">Authorization</span></span>|<span data-ttu-id="1a7bb-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a7bb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a7bb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1a7bb-126">Accept</span></span>|<span data-ttu-id="1a7bb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1a7bb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a7bb-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a7bb-128">Request body</span></span>
<span data-ttu-id="1a7bb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a7bb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a7bb-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a7bb-130">Response</span></span>
<span data-ttu-id="1a7bb-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1a7bb-131">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a7bb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1a7bb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a7bb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a7bb-133">Request</span></span>
<span data-ttu-id="1a7bb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a7bb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="1a7bb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a7bb-135">Response</span></span>
<span data-ttu-id="1a7bb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a7bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceOverview",
    "id": "42a91653-1653-42a9-5316-a9425316a942",
    "enrolledDeviceCount": 3,
    "mdmEnrolledCount": 0,
    "dualEnrolledDeviceCount": 7,
    "deviceOperatingSystemSummary": {
      "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
      "androidCount": 12,
      "iosCount": 8,
      "macOSCount": 10,
      "windowsMobileCount": 2,
      "windowsCount": 12,
      "unknownCount": 12
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    }
  }
}
```






