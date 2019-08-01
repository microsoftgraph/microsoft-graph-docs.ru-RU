---
title: Get managedDeviceOverview
description: Чтение свойств и связей объекта managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27ed01c6b4a09b04c2688742008210b00451b203
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018563"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="9961d-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9961d-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="9961d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9961d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9961d-105">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="9961d-105">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9961d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9961d-106">Prerequisites</span></span>
<span data-ttu-id="9961d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9961d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9961d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9961d-109">Permission type</span></span>|<span data-ttu-id="9961d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9961d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9961d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9961d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9961d-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9961d-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9961d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9961d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9961d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9961d-114">Not supported.</span></span>|
|<span data-ttu-id="9961d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9961d-115">Application</span></span>|<span data-ttu-id="9961d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9961d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9961d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9961d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9961d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9961d-118">Optional query parameters</span></span>
<span data-ttu-id="9961d-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9961d-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9961d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9961d-120">Request headers</span></span>
|<span data-ttu-id="9961d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9961d-121">Header</span></span>|<span data-ttu-id="9961d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9961d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9961d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9961d-123">Authorization</span></span>|<span data-ttu-id="9961d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9961d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9961d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9961d-125">Accept</span></span>|<span data-ttu-id="9961d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9961d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9961d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9961d-127">Request body</span></span>
<span data-ttu-id="9961d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9961d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9961d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9961d-129">Response</span></span>
<span data-ttu-id="9961d-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9961d-130">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9961d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9961d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9961d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9961d-132">Request</span></span>
<span data-ttu-id="9961d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9961d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="9961d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9961d-134">Response</span></span>
<span data-ttu-id="9961d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9961d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



