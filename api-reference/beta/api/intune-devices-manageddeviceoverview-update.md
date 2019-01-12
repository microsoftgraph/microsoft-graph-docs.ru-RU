---
title: Обновление объекта managedDeviceOverview
description: Обновление свойств объекта managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 239c70e441c6dbfdaf593c9c0261e8a6ba4be653
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982864"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="7dad2-103">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7dad2-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="7dad2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7dad2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7dad2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dad2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7dad2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7dad2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7dad2-107">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7dad2-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7dad2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7dad2-108">Prerequisites</span></span>
<span data-ttu-id="7dad2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dad2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dad2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dad2-111">Permission type</span></span>|<span data-ttu-id="7dad2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dad2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dad2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dad2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7dad2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dad2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7dad2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dad2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dad2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dad2-116">Not supported.</span></span>|
|<span data-ttu-id="7dad2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dad2-117">Application</span></span>|<span data-ttu-id="7dad2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dad2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dad2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dad2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="7dad2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dad2-120">Request headers</span></span>
|<span data-ttu-id="7dad2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7dad2-121">Header</span></span>|<span data-ttu-id="7dad2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7dad2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dad2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dad2-123">Authorization</span></span>|<span data-ttu-id="7dad2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7dad2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dad2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7dad2-125">Accept</span></span>|<span data-ttu-id="7dad2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7dad2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dad2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7dad2-127">Request body</span></span>
<span data-ttu-id="7dad2-128">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dad2-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="7dad2-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7dad2-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="7dad2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dad2-130">Property</span></span>|<span data-ttu-id="7dad2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7dad2-131">Type</span></span>|<span data-ttu-id="7dad2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7dad2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dad2-133">id</span><span class="sxs-lookup"><span data-stu-id="7dad2-133">id</span></span>|<span data-ttu-id="7dad2-134">String</span><span class="sxs-lookup"><span data-stu-id="7dad2-134">String</span></span>|<span data-ttu-id="7dad2-135">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="7dad2-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="7dad2-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7dad2-136">enrolledDeviceCount</span></span>|<span data-ttu-id="7dad2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7dad2-137">Int32</span></span>|<span data-ttu-id="7dad2-138">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="7dad2-138">Total enrolled device count.</span></span> <span data-ttu-id="7dad2-139">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="7dad2-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="7dad2-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="7dad2-140">mdmEnrolledCount</span></span>|<span data-ttu-id="7dad2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7dad2-141">Int32</span></span>|<span data-ttu-id="7dad2-142">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="7dad2-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="7dad2-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7dad2-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="7dad2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7dad2-144">Int32</span></span>|<span data-ttu-id="7dad2-145">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="7dad2-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="7dad2-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7dad2-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="7dad2-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7dad2-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="7dad2-148">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="7dad2-148">Device operating system summary.</span></span>|
|<span data-ttu-id="7dad2-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7dad2-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="7dad2-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7dad2-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="7dad2-151">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="7dad2-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="7dad2-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="7dad2-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="7dad2-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="7dad2-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="7dad2-154">Модели и производители meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="7dad2-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="7dad2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dad2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="7dad2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dad2-156">DateTimeOffset</span></span>|<span data-ttu-id="7dad2-157">Время последнего изменения Обзор устройства</span><span class="sxs-lookup"><span data-stu-id="7dad2-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="7dad2-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dad2-158">Response</span></span>
<span data-ttu-id="7dad2-159">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7dad2-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dad2-160">Пример</span><span class="sxs-lookup"><span data-stu-id="7dad2-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="7dad2-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dad2-161">Request</span></span>
<span data-ttu-id="7dad2-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dad2-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 947

{
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

### <a name="response"></a><span data-ttu-id="7dad2-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="7dad2-163">Response</span></span>
<span data-ttu-id="7dad2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7dad2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





