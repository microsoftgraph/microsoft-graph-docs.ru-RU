---
title: Обновление объекта managedDeviceOverview
description: Обновление свойств объекта managedDeviceOverview.
ms.openlocfilehash: e17c084aafa7925419b4143b273e61703c08fc06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027141"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="6634a-103">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6634a-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="6634a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6634a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6634a-105">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="6634a-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6634a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6634a-106">Prerequisites</span></span>
<span data-ttu-id="6634a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6634a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6634a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6634a-109">Permission type</span></span>|<span data-ttu-id="6634a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6634a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6634a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6634a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6634a-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6634a-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6634a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6634a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6634a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6634a-114">Not supported.</span></span>|
|<span data-ttu-id="6634a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6634a-115">Application</span></span>|<span data-ttu-id="6634a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6634a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6634a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6634a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="6634a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6634a-118">Request headers</span></span>
|<span data-ttu-id="6634a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6634a-119">Header</span></span>|<span data-ttu-id="6634a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6634a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6634a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6634a-121">Authorization</span></span>|<span data-ttu-id="6634a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6634a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6634a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6634a-123">Accept</span></span>|<span data-ttu-id="6634a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6634a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6634a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6634a-125">Request body</span></span>
<span data-ttu-id="6634a-126">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6634a-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="6634a-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="6634a-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="6634a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6634a-128">Property</span></span>|<span data-ttu-id="6634a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6634a-129">Type</span></span>|<span data-ttu-id="6634a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6634a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6634a-131">id</span><span class="sxs-lookup"><span data-stu-id="6634a-131">id</span></span>|<span data-ttu-id="6634a-132">String</span><span class="sxs-lookup"><span data-stu-id="6634a-132">String</span></span>|<span data-ttu-id="6634a-133">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="6634a-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="6634a-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6634a-134">enrolledDeviceCount</span></span>|<span data-ttu-id="6634a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="6634a-135">Int32</span></span>|<span data-ttu-id="6634a-136">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="6634a-136">Total enrolled device count.</span></span> <span data-ttu-id="6634a-137">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="6634a-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="6634a-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="6634a-138">mdmEnrolledCount</span></span>|<span data-ttu-id="6634a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6634a-139">Int32</span></span>|<span data-ttu-id="6634a-140">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="6634a-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="6634a-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6634a-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="6634a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6634a-142">Int32</span></span>|<span data-ttu-id="6634a-143">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="6634a-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="6634a-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="6634a-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="6634a-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="6634a-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="6634a-146">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="6634a-146">Device operating system summary.</span></span>|
|<span data-ttu-id="6634a-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="6634a-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="6634a-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="6634a-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="6634a-149">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="6634a-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="6634a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="6634a-150">Response</span></span>
<span data-ttu-id="6634a-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6634a-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6634a-152">Пример</span><span class="sxs-lookup"><span data-stu-id="6634a-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="6634a-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="6634a-153">Request</span></span>
<span data-ttu-id="6634a-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6634a-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6634a-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="6634a-155">Response</span></span>
<span data-ttu-id="6634a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6634a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



