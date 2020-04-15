---
title: Обновление объекта managedDeviceOverview
description: Обновление свойств объекта managedDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45b164859bd5d53dc05e22c47aa1ca99335b18f3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388737"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="4c487-103">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="4c487-103">Update managedDeviceOverview</span></span>

<span data-ttu-id="4c487-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c487-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c487-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c487-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c487-106">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="4c487-106">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c487-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c487-107">Prerequisites</span></span>
<span data-ttu-id="4c487-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c487-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c487-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c487-110">Permission type</span></span>|<span data-ttu-id="4c487-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c487-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c487-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c487-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c487-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c487-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4c487-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c487-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c487-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c487-115">Not supported.</span></span>|
|<span data-ttu-id="4c487-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c487-116">Application</span></span>|<span data-ttu-id="4c487-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c487-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c487-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c487-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="4c487-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4c487-119">Request headers</span></span>
|<span data-ttu-id="4c487-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c487-120">Header</span></span>|<span data-ttu-id="4c487-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4c487-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c487-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c487-122">Authorization</span></span>|<span data-ttu-id="4c487-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c487-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c487-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4c487-124">Accept</span></span>|<span data-ttu-id="4c487-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c487-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c487-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c487-126">Request body</span></span>
<span data-ttu-id="4c487-127">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c487-127">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="4c487-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="4c487-128">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="4c487-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c487-129">Property</span></span>|<span data-ttu-id="4c487-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4c487-130">Type</span></span>|<span data-ttu-id="4c487-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4c487-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c487-132">id</span><span class="sxs-lookup"><span data-stu-id="4c487-132">id</span></span>|<span data-ttu-id="4c487-133">String</span><span class="sxs-lookup"><span data-stu-id="4c487-133">String</span></span>|<span data-ttu-id="4c487-134">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="4c487-134">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="4c487-135">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c487-135">enrolledDeviceCount</span></span>|<span data-ttu-id="4c487-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4c487-136">Int32</span></span>|<span data-ttu-id="4c487-137">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="4c487-137">Total enrolled device count.</span></span> <span data-ttu-id="4c487-138">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="4c487-138">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="4c487-139">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="4c487-139">mdmEnrolledCount</span></span>|<span data-ttu-id="4c487-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4c487-140">Int32</span></span>|<span data-ttu-id="4c487-141">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="4c487-141">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="4c487-142">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c487-142">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="4c487-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4c487-143">Int32</span></span>|<span data-ttu-id="4c487-144">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="4c487-144">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="4c487-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="4c487-145">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="4c487-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="4c487-146">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="4c487-147">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="4c487-147">Device operating system summary.</span></span>|
|<span data-ttu-id="4c487-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="4c487-148">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="4c487-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="4c487-149">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="4c487-150">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="4c487-150">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="4c487-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c487-151">Response</span></span>
<span data-ttu-id="4c487-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4c487-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c487-153">Пример</span><span class="sxs-lookup"><span data-stu-id="4c487-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c487-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c487-154">Request</span></span>
<span data-ttu-id="4c487-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c487-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 685

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
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
```

### <a name="response"></a><span data-ttu-id="4c487-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c487-156">Response</span></span>
<span data-ttu-id="4c487-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c487-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

{
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
```






