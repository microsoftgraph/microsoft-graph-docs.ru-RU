---
title: Обновление объекта managedDeviceOverview
description: Обновление свойств объекта managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3808c35b9aae428975ed976b31634c27e7a41286
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585043"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="f3c88-103">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f3c88-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="f3c88-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3c88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3c88-105">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f3c88-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3c88-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f3c88-106">Prerequisites</span></span>
<span data-ttu-id="f3c88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3c88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3c88-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c88-109">Permission type</span></span>|<span data-ttu-id="f3c88-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3c88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3c88-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3c88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3c88-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3c88-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3c88-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3c88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3c88-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c88-114">Not supported.</span></span>|
|<span data-ttu-id="f3c88-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3c88-115">Application</span></span>|<span data-ttu-id="f3c88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3c88-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3c88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="f3c88-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3c88-118">Request headers</span></span>
|<span data-ttu-id="f3c88-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3c88-119">Header</span></span>|<span data-ttu-id="f3c88-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f3c88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3c88-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3c88-121">Authorization</span></span>|<span data-ttu-id="f3c88-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3c88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3c88-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f3c88-123">Accept</span></span>|<span data-ttu-id="f3c88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3c88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3c88-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3c88-125">Request body</span></span>
<span data-ttu-id="f3c88-126">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3c88-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="f3c88-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f3c88-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="f3c88-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3c88-128">Property</span></span>|<span data-ttu-id="f3c88-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f3c88-129">Type</span></span>|<span data-ttu-id="f3c88-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f3c88-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3c88-131">id</span><span class="sxs-lookup"><span data-stu-id="f3c88-131">id</span></span>|<span data-ttu-id="f3c88-132">String</span><span class="sxs-lookup"><span data-stu-id="f3c88-132">String</span></span>|<span data-ttu-id="f3c88-133">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="f3c88-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="f3c88-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3c88-134">enrolledDeviceCount</span></span>|<span data-ttu-id="f3c88-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f3c88-135">Int32</span></span>|<span data-ttu-id="f3c88-136">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="f3c88-136">Total enrolled device count.</span></span> <span data-ttu-id="f3c88-137">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="f3c88-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="f3c88-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="f3c88-138">mdmEnrolledCount</span></span>|<span data-ttu-id="f3c88-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f3c88-139">Int32</span></span>|<span data-ttu-id="f3c88-140">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="f3c88-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="f3c88-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3c88-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="f3c88-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f3c88-142">Int32</span></span>|<span data-ttu-id="f3c88-143">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="f3c88-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="f3c88-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f3c88-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="f3c88-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f3c88-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="f3c88-146">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="f3c88-146">Device operating system summary.</span></span>|
|<span data-ttu-id="f3c88-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f3c88-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="f3c88-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f3c88-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="f3c88-149">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="f3c88-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="f3c88-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c88-150">Response</span></span>
<span data-ttu-id="f3c88-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f3c88-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3c88-152">Пример</span><span class="sxs-lookup"><span data-stu-id="f3c88-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3c88-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3c88-153">Request</span></span>
<span data-ttu-id="f3c88-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3c88-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3c88-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c88-155">Response</span></span>
<span data-ttu-id="f3c88-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3c88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



