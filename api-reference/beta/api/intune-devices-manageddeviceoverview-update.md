---
title: Обновление объекта managedDeviceOverview
description: Обновление свойств объекта managedDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 568cbdff57bc304b5757af6f35aed04e6195130c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155092"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="52fa4-103">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="52fa4-103">Update managedDeviceOverview</span></span>

<span data-ttu-id="52fa4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52fa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52fa4-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52fa4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52fa4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52fa4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52fa4-107">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="52fa4-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52fa4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="52fa4-108">Prerequisites</span></span>
<span data-ttu-id="52fa4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52fa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52fa4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52fa4-111">Permission type</span></span>|<span data-ttu-id="52fa4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52fa4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52fa4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52fa4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52fa4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52fa4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="52fa4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52fa4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52fa4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52fa4-116">Not supported.</span></span>|
|<span data-ttu-id="52fa4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52fa4-117">Application</span></span>|<span data-ttu-id="52fa4-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52fa4-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52fa4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52fa4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="52fa4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52fa4-120">Request headers</span></span>
|<span data-ttu-id="52fa4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52fa4-121">Header</span></span>|<span data-ttu-id="52fa4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52fa4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52fa4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52fa4-123">Authorization</span></span>|<span data-ttu-id="52fa4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52fa4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52fa4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52fa4-125">Accept</span></span>|<span data-ttu-id="52fa4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52fa4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52fa4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52fa4-127">Request body</span></span>
<span data-ttu-id="52fa4-128">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52fa4-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="52fa4-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="52fa4-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="52fa4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="52fa4-130">Property</span></span>|<span data-ttu-id="52fa4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="52fa4-131">Type</span></span>|<span data-ttu-id="52fa4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="52fa4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52fa4-133">id</span><span class="sxs-lookup"><span data-stu-id="52fa4-133">id</span></span>|<span data-ttu-id="52fa4-134">String</span><span class="sxs-lookup"><span data-stu-id="52fa4-134">String</span></span>|<span data-ttu-id="52fa4-135">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="52fa4-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="52fa4-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="52fa4-136">enrolledDeviceCount</span></span>|<span data-ttu-id="52fa4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="52fa4-137">Int32</span></span>|<span data-ttu-id="52fa4-138">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="52fa4-138">Total enrolled device count.</span></span> <span data-ttu-id="52fa4-139">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="52fa4-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="52fa4-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="52fa4-140">mdmEnrolledCount</span></span>|<span data-ttu-id="52fa4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="52fa4-141">Int32</span></span>|<span data-ttu-id="52fa4-142">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="52fa4-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="52fa4-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="52fa4-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="52fa4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="52fa4-144">Int32</span></span>|<span data-ttu-id="52fa4-145">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="52fa4-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="52fa4-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="52fa4-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="52fa4-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="52fa4-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="52fa4-148">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="52fa4-148">Device operating system summary.</span></span>|
|<span data-ttu-id="52fa4-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="52fa4-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="52fa4-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="52fa4-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="52fa4-151">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="52fa4-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="52fa4-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="52fa4-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="52fa4-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="52fa4-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="52fa4-154">Модели и производство в учетной записи для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="52fa4-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="52fa4-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52fa4-155">lastModifiedDateTime</span></span>|<span data-ttu-id="52fa4-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52fa4-156">DateTimeOffset</span></span>|<span data-ttu-id="52fa4-157">Обзор даты последнего изменения устройства</span><span class="sxs-lookup"><span data-stu-id="52fa4-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="52fa4-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="52fa4-158">Response</span></span>
<span data-ttu-id="52fa4-159">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="52fa4-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52fa4-160">Пример</span><span class="sxs-lookup"><span data-stu-id="52fa4-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="52fa4-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="52fa4-161">Request</span></span>
<span data-ttu-id="52fa4-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52fa4-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 1222

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
    "androidWorkProfileCount": 7,
    "androidCorporateWorkProfileCount": 0,
    "configMgrDeviceCount": 4,
    "aospUserlessCount": 1,
    "aospUserAssociatedCount": 7
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

### <a name="response"></a><span data-ttu-id="52fa4-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="52fa4-163">Response</span></span>
<span data-ttu-id="52fa4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52fa4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1335

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
    "androidWorkProfileCount": 7,
    "androidCorporateWorkProfileCount": 0,
    "configMgrDeviceCount": 4,
    "aospUserlessCount": 1,
    "aospUserAssociatedCount": 7
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




