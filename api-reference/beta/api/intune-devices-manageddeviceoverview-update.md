---
title: Обновление объекта managedDeviceOverview
description: Обновление свойств объекта managedDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: debb09cb12191f025a70a2dde5d4b476b6cd4592
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944605"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="f8a23-103">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f8a23-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="f8a23-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8a23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8a23-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8a23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8a23-106">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f8a23-106">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8a23-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8a23-107">Prerequisites</span></span>
<span data-ttu-id="f8a23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8a23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8a23-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8a23-110">Permission type</span></span>|<span data-ttu-id="f8a23-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8a23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8a23-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8a23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8a23-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8a23-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f8a23-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8a23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8a23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8a23-115">Not supported.</span></span>|
|<span data-ttu-id="f8a23-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8a23-116">Application</span></span>|<span data-ttu-id="f8a23-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8a23-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8a23-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8a23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="f8a23-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f8a23-119">Request headers</span></span>
|<span data-ttu-id="f8a23-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8a23-120">Header</span></span>|<span data-ttu-id="f8a23-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f8a23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8a23-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8a23-122">Authorization</span></span>|<span data-ttu-id="f8a23-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8a23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8a23-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f8a23-124">Accept</span></span>|<span data-ttu-id="f8a23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8a23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8a23-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f8a23-126">Request body</span></span>
<span data-ttu-id="f8a23-127">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8a23-127">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="f8a23-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f8a23-128">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="f8a23-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8a23-129">Property</span></span>|<span data-ttu-id="f8a23-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f8a23-130">Type</span></span>|<span data-ttu-id="f8a23-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f8a23-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8a23-132">id</span><span class="sxs-lookup"><span data-stu-id="f8a23-132">id</span></span>|<span data-ttu-id="f8a23-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f8a23-133">String</span></span>|<span data-ttu-id="f8a23-134">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="f8a23-134">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="f8a23-135">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f8a23-135">enrolledDeviceCount</span></span>|<span data-ttu-id="f8a23-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f8a23-136">Int32</span></span>|<span data-ttu-id="f8a23-137">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="f8a23-137">Total enrolled device count.</span></span> <span data-ttu-id="f8a23-138">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="f8a23-138">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="f8a23-139">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="f8a23-139">mdmEnrolledCount</span></span>|<span data-ttu-id="f8a23-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f8a23-140">Int32</span></span>|<span data-ttu-id="f8a23-141">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="f8a23-141">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="f8a23-142">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f8a23-142">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="f8a23-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f8a23-143">Int32</span></span>|<span data-ttu-id="f8a23-144">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="f8a23-144">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="f8a23-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f8a23-145">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="f8a23-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f8a23-146">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="f8a23-147">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="f8a23-147">Device operating system summary.</span></span>|
|<span data-ttu-id="f8a23-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f8a23-148">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="f8a23-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f8a23-149">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="f8a23-150">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="f8a23-150">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="f8a23-151">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f8a23-151">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="f8a23-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f8a23-152">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="f8a23-153">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="f8a23-153">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="f8a23-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8a23-154">lastModifiedDateTime</span></span>|<span data-ttu-id="f8a23-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8a23-155">DateTimeOffset</span></span>|<span data-ttu-id="f8a23-156">Общие сведения о дате и времени последнего изменения устройства</span><span class="sxs-lookup"><span data-stu-id="f8a23-156">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="f8a23-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8a23-157">Response</span></span>
<span data-ttu-id="f8a23-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f8a23-158">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8a23-159">Пример</span><span class="sxs-lookup"><span data-stu-id="f8a23-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8a23-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8a23-160">Request</span></span>
<span data-ttu-id="f8a23-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8a23-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 1082

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
    "unknownCount": 12,
    "androidDedicatedCount": 5,
    "androidDeviceAdminCount": 7,
    "androidFullyManagedCount": 8,
    "androidWorkProfileCount": 7
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "Device Models value"
    ],
    "deviceManufacturers": [
      "Device Manufacturers value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="f8a23-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8a23-162">Response</span></span>
<span data-ttu-id="f8a23-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8a23-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1195

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
    "unknownCount": 12,
    "androidDedicatedCount": 5,
    "androidDeviceAdminCount": 7,
    "androidFullyManagedCount": 8,
    "androidWorkProfileCount": 7
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "Device Models value"
    ],
    "deviceManufacturers": [
      "Device Manufacturers value"
    ]
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





