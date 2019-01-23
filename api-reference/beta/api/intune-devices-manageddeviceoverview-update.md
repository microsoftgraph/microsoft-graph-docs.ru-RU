---
title: Обновление объекта managedDeviceOverview
description: Обновление свойств объекта managedDeviceOverview.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34271db88490fba3ac635892daac66bf9cf904b8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424534"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="639d8-103">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="639d8-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="639d8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="639d8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="639d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="639d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="639d8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="639d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="639d8-107">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="639d8-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="639d8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="639d8-108">Prerequisites</span></span>
<span data-ttu-id="639d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="639d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="639d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="639d8-111">Permission type</span></span>|<span data-ttu-id="639d8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="639d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="639d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="639d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="639d8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="639d8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="639d8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="639d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="639d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="639d8-116">Not supported.</span></span>|
|<span data-ttu-id="639d8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="639d8-117">Application</span></span>|<span data-ttu-id="639d8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="639d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="639d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="639d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="639d8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="639d8-120">Request headers</span></span>
|<span data-ttu-id="639d8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="639d8-121">Header</span></span>|<span data-ttu-id="639d8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="639d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="639d8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="639d8-123">Authorization</span></span>|<span data-ttu-id="639d8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="639d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="639d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="639d8-125">Accept</span></span>|<span data-ttu-id="639d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="639d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="639d8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="639d8-127">Request body</span></span>
<span data-ttu-id="639d8-128">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="639d8-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="639d8-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="639d8-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="639d8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="639d8-130">Property</span></span>|<span data-ttu-id="639d8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="639d8-131">Type</span></span>|<span data-ttu-id="639d8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="639d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="639d8-133">id</span><span class="sxs-lookup"><span data-stu-id="639d8-133">id</span></span>|<span data-ttu-id="639d8-134">String</span><span class="sxs-lookup"><span data-stu-id="639d8-134">String</span></span>|<span data-ttu-id="639d8-135">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="639d8-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="639d8-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="639d8-136">enrolledDeviceCount</span></span>|<span data-ttu-id="639d8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="639d8-137">Int32</span></span>|<span data-ttu-id="639d8-138">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="639d8-138">Total enrolled device count.</span></span> <span data-ttu-id="639d8-139">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="639d8-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="639d8-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="639d8-140">mdmEnrolledCount</span></span>|<span data-ttu-id="639d8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="639d8-141">Int32</span></span>|<span data-ttu-id="639d8-142">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="639d8-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="639d8-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="639d8-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="639d8-144">Int32</span><span class="sxs-lookup"><span data-stu-id="639d8-144">Int32</span></span>|<span data-ttu-id="639d8-145">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="639d8-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="639d8-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="639d8-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="639d8-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="639d8-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="639d8-148">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="639d8-148">Device operating system summary.</span></span>|
|<span data-ttu-id="639d8-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="639d8-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="639d8-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="639d8-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="639d8-151">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="639d8-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="639d8-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="639d8-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="639d8-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="639d8-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="639d8-154">Модели и производители meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="639d8-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="639d8-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="639d8-155">lastModifiedDateTime</span></span>|<span data-ttu-id="639d8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="639d8-156">DateTimeOffset</span></span>|<span data-ttu-id="639d8-157">Время последнего изменения Обзор устройства</span><span class="sxs-lookup"><span data-stu-id="639d8-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="639d8-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="639d8-158">Response</span></span>
<span data-ttu-id="639d8-159">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="639d8-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="639d8-160">Пример</span><span class="sxs-lookup"><span data-stu-id="639d8-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="639d8-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="639d8-161">Request</span></span>
<span data-ttu-id="639d8-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="639d8-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="639d8-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="639d8-163">Response</span></span>
<span data-ttu-id="639d8-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="639d8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




