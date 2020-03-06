---
title: Обновление объекта deviceConfigurationDeviceOverview
description: Обновление свойств объекта deviceConfigurationDeviceOverview.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33f68bb41e2f22dac51f0805bb0b1305361446c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514798"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="b4c23-103">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b4c23-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="b4c23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4c23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4c23-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4c23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4c23-106">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b4c23-106">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4c23-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b4c23-107">Prerequisites</span></span>
<span data-ttu-id="b4c23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4c23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4c23-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4c23-110">Permission type</span></span>|<span data-ttu-id="b4c23-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4c23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4c23-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4c23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4c23-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4c23-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4c23-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4c23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4c23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4c23-115">Not supported.</span></span>|
|<span data-ttu-id="b4c23-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4c23-116">Application</span></span>|<span data-ttu-id="b4c23-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4c23-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4c23-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4c23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="b4c23-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4c23-119">Request headers</span></span>
|<span data-ttu-id="b4c23-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4c23-120">Header</span></span>|<span data-ttu-id="b4c23-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b4c23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4c23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4c23-122">Authorization</span></span>|<span data-ttu-id="b4c23-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4c23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4c23-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b4c23-124">Accept</span></span>|<span data-ttu-id="b4c23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4c23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4c23-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4c23-126">Request body</span></span>
<span data-ttu-id="b4c23-127">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4c23-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="b4c23-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b4c23-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="b4c23-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4c23-129">Property</span></span>|<span data-ttu-id="b4c23-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b4c23-130">Type</span></span>|<span data-ttu-id="b4c23-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b4c23-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4c23-132">id</span><span class="sxs-lookup"><span data-stu-id="b4c23-132">id</span></span>|<span data-ttu-id="b4c23-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b4c23-133">String</span></span>|<span data-ttu-id="b4c23-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b4c23-134">Key of the entity.</span></span>|
|<span data-ttu-id="b4c23-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="b4c23-135">pendingCount</span></span>|<span data-ttu-id="b4c23-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c23-136">Int32</span></span>|<span data-ttu-id="b4c23-137">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="b4c23-137">Number of pending devices</span></span>|
|<span data-ttu-id="b4c23-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b4c23-138">notApplicableCount</span></span>|<span data-ttu-id="b4c23-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c23-139">Int32</span></span>|<span data-ttu-id="b4c23-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="b4c23-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="b4c23-141">successCount</span><span class="sxs-lookup"><span data-stu-id="b4c23-141">successCount</span></span>|<span data-ttu-id="b4c23-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c23-142">Int32</span></span>|<span data-ttu-id="b4c23-143">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="b4c23-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="b4c23-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="b4c23-144">errorCount</span></span>|<span data-ttu-id="b4c23-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c23-145">Int32</span></span>|<span data-ttu-id="b4c23-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="b4c23-146">Number of error devices</span></span>|
|<span data-ttu-id="b4c23-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="b4c23-147">failedCount</span></span>|<span data-ttu-id="b4c23-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c23-148">Int32</span></span>|<span data-ttu-id="b4c23-149">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="b4c23-149">Number of failed devices</span></span>|
|<span data-ttu-id="b4c23-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b4c23-150">lastUpdateDateTime</span></span>|<span data-ttu-id="b4c23-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c23-151">DateTimeOffset</span></span>|<span data-ttu-id="b4c23-152">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="b4c23-152">Last update time</span></span>|
|<span data-ttu-id="b4c23-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="b4c23-153">configurationVersion</span></span>|<span data-ttu-id="b4c23-154">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c23-154">Int32</span></span>|<span data-ttu-id="b4c23-155">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="b4c23-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="b4c23-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4c23-156">Response</span></span>
<span data-ttu-id="b4c23-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4c23-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4c23-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b4c23-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4c23-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4c23-159">Request</span></span>
<span data-ttu-id="b4c23-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4c23-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="b4c23-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4c23-161">Response</span></span>
<span data-ttu-id="b4c23-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4c23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




