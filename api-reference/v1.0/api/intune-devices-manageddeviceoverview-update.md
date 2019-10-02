---
title: Обновление объекта managedDeviceOverview
description: Обновление свойств объекта managedDeviceOverview.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf354ee25a0b38c336af3f50eba70560b5b057ab
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364181"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="faf34-103">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="faf34-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="faf34-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="faf34-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faf34-105">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="faf34-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faf34-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="faf34-106">Prerequisites</span></span>
<span data-ttu-id="faf34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faf34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faf34-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="faf34-109">Permission type</span></span>|<span data-ttu-id="faf34-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="faf34-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faf34-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="faf34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="faf34-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf34-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="faf34-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="faf34-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faf34-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faf34-114">Not supported.</span></span>|
|<span data-ttu-id="faf34-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="faf34-115">Application</span></span>|<span data-ttu-id="faf34-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faf34-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faf34-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="faf34-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="faf34-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="faf34-118">Request headers</span></span>
|<span data-ttu-id="faf34-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="faf34-119">Header</span></span>|<span data-ttu-id="faf34-120">Значение</span><span class="sxs-lookup"><span data-stu-id="faf34-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faf34-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="faf34-121">Authorization</span></span>|<span data-ttu-id="faf34-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="faf34-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faf34-123">Accept</span><span class="sxs-lookup"><span data-stu-id="faf34-123">Accept</span></span>|<span data-ttu-id="faf34-124">application/json</span><span class="sxs-lookup"><span data-stu-id="faf34-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faf34-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="faf34-125">Request body</span></span>
<span data-ttu-id="faf34-126">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="faf34-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="faf34-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="faf34-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="faf34-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="faf34-128">Property</span></span>|<span data-ttu-id="faf34-129">Тип</span><span class="sxs-lookup"><span data-stu-id="faf34-129">Type</span></span>|<span data-ttu-id="faf34-130">Описание</span><span class="sxs-lookup"><span data-stu-id="faf34-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faf34-131">id</span><span class="sxs-lookup"><span data-stu-id="faf34-131">id</span></span>|<span data-ttu-id="faf34-132">String</span><span class="sxs-lookup"><span data-stu-id="faf34-132">String</span></span>|<span data-ttu-id="faf34-133">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="faf34-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="faf34-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="faf34-134">enrolledDeviceCount</span></span>|<span data-ttu-id="faf34-135">Int32</span><span class="sxs-lookup"><span data-stu-id="faf34-135">Int32</span></span>|<span data-ttu-id="faf34-136">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="faf34-136">Total enrolled device count.</span></span> <span data-ttu-id="faf34-137">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="faf34-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="faf34-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="faf34-138">mdmEnrolledCount</span></span>|<span data-ttu-id="faf34-139">Int32</span><span class="sxs-lookup"><span data-stu-id="faf34-139">Int32</span></span>|<span data-ttu-id="faf34-140">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="faf34-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="faf34-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="faf34-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="faf34-142">Int32</span><span class="sxs-lookup"><span data-stu-id="faf34-142">Int32</span></span>|<span data-ttu-id="faf34-143">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="faf34-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="faf34-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="faf34-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="faf34-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="faf34-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="faf34-146">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="faf34-146">Device operating system summary.</span></span>|
|<span data-ttu-id="faf34-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="faf34-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="faf34-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="faf34-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="faf34-149">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="faf34-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="faf34-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="faf34-150">Response</span></span>
<span data-ttu-id="faf34-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="faf34-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faf34-152">Пример</span><span class="sxs-lookup"><span data-stu-id="faf34-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="faf34-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="faf34-153">Request</span></span>
<span data-ttu-id="faf34-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="faf34-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="faf34-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="faf34-155">Response</span></span>
<span data-ttu-id="faf34-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="faf34-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




