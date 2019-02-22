---
title: Обновление объекта managedDeviceOverview
description: Обновление свойств объекта managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 642d565a7555446da1728c0a697598de4d5459cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147847"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="61294-103">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="61294-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="61294-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61294-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61294-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61294-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61294-106">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="61294-106">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61294-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="61294-107">Prerequisites</span></span>
<span data-ttu-id="61294-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="61294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="61294-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61294-110">Permission type</span></span>|<span data-ttu-id="61294-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="61294-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61294-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61294-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61294-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61294-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="61294-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61294-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61294-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61294-115">Not supported.</span></span>|
|<span data-ttu-id="61294-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61294-116">Application</span></span>|<span data-ttu-id="61294-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61294-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61294-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61294-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="61294-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61294-119">Request headers</span></span>
|<span data-ttu-id="61294-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61294-120">Header</span></span>|<span data-ttu-id="61294-121">Значение</span><span class="sxs-lookup"><span data-stu-id="61294-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61294-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61294-122">Authorization</span></span>|<span data-ttu-id="61294-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="61294-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61294-124">Accept</span><span class="sxs-lookup"><span data-stu-id="61294-124">Accept</span></span>|<span data-ttu-id="61294-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61294-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61294-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="61294-126">Request body</span></span>
<span data-ttu-id="61294-127">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61294-127">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="61294-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="61294-128">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="61294-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="61294-129">Property</span></span>|<span data-ttu-id="61294-130">Тип</span><span class="sxs-lookup"><span data-stu-id="61294-130">Type</span></span>|<span data-ttu-id="61294-131">Описание</span><span class="sxs-lookup"><span data-stu-id="61294-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61294-132">id</span><span class="sxs-lookup"><span data-stu-id="61294-132">id</span></span>|<span data-ttu-id="61294-133">String</span><span class="sxs-lookup"><span data-stu-id="61294-133">String</span></span>|<span data-ttu-id="61294-134">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="61294-134">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="61294-135">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61294-135">enrolledDeviceCount</span></span>|<span data-ttu-id="61294-136">Int32</span><span class="sxs-lookup"><span data-stu-id="61294-136">Int32</span></span>|<span data-ttu-id="61294-137">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="61294-137">Total enrolled device count.</span></span> <span data-ttu-id="61294-138">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="61294-138">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="61294-139">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="61294-139">mdmEnrolledCount</span></span>|<span data-ttu-id="61294-140">Int32</span><span class="sxs-lookup"><span data-stu-id="61294-140">Int32</span></span>|<span data-ttu-id="61294-141">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="61294-141">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="61294-142">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61294-142">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="61294-143">Int32</span><span class="sxs-lookup"><span data-stu-id="61294-143">Int32</span></span>|<span data-ttu-id="61294-144">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="61294-144">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="61294-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="61294-145">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="61294-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="61294-146">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="61294-147">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="61294-147">Device operating system summary.</span></span>|
|<span data-ttu-id="61294-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="61294-148">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="61294-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="61294-149">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="61294-150">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="61294-150">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="61294-151">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="61294-151">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="61294-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="61294-152">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="61294-153">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="61294-153">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="61294-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61294-154">lastModifiedDateTime</span></span>|<span data-ttu-id="61294-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61294-155">DateTimeOffset</span></span>|<span data-ttu-id="61294-156">Общие сведения о дате и времени последнего изменения устройства</span><span class="sxs-lookup"><span data-stu-id="61294-156">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="61294-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="61294-157">Response</span></span>
<span data-ttu-id="61294-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="61294-158">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61294-159">Пример</span><span class="sxs-lookup"><span data-stu-id="61294-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="61294-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="61294-160">Request</span></span>
<span data-ttu-id="61294-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61294-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 943

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

### <a name="response"></a><span data-ttu-id="61294-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="61294-162">Response</span></span>
<span data-ttu-id="61294-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61294-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1056

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




