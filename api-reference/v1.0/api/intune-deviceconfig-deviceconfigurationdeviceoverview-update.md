---
title: Обновление объекта deviceConfigurationDeviceOverview
description: Обновление свойств объекта deviceConfigurationDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39b434d2a6e3ddabeea11689332c74c334e7adfb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051874"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="735ae-103">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="735ae-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="735ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="735ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="735ae-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="735ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="735ae-106">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="735ae-106">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="735ae-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="735ae-107">Prerequisites</span></span>
<span data-ttu-id="735ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="735ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="735ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="735ae-110">Permission type</span></span>|<span data-ttu-id="735ae-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="735ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="735ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="735ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="735ae-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="735ae-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="735ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="735ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="735ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="735ae-115">Not supported.</span></span>|
|<span data-ttu-id="735ae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="735ae-116">Application</span></span>|<span data-ttu-id="735ae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="735ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="735ae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="735ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="735ae-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="735ae-119">Request headers</span></span>
|<span data-ttu-id="735ae-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="735ae-120">Header</span></span>|<span data-ttu-id="735ae-121">Значение</span><span class="sxs-lookup"><span data-stu-id="735ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="735ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="735ae-122">Authorization</span></span>|<span data-ttu-id="735ae-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="735ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="735ae-124">Accept</span><span class="sxs-lookup"><span data-stu-id="735ae-124">Accept</span></span>|<span data-ttu-id="735ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="735ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="735ae-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="735ae-126">Request body</span></span>
<span data-ttu-id="735ae-127">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="735ae-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="735ae-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="735ae-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="735ae-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="735ae-129">Property</span></span>|<span data-ttu-id="735ae-130">Тип</span><span class="sxs-lookup"><span data-stu-id="735ae-130">Type</span></span>|<span data-ttu-id="735ae-131">Описание</span><span class="sxs-lookup"><span data-stu-id="735ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="735ae-132">id</span><span class="sxs-lookup"><span data-stu-id="735ae-132">id</span></span>|<span data-ttu-id="735ae-133">String</span><span class="sxs-lookup"><span data-stu-id="735ae-133">String</span></span>|<span data-ttu-id="735ae-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="735ae-134">Key of the entity.</span></span>|
|<span data-ttu-id="735ae-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="735ae-135">pendingCount</span></span>|<span data-ttu-id="735ae-136">Int32</span><span class="sxs-lookup"><span data-stu-id="735ae-136">Int32</span></span>|<span data-ttu-id="735ae-137">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="735ae-137">Number of pending devices</span></span>|
|<span data-ttu-id="735ae-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="735ae-138">notApplicableCount</span></span>|<span data-ttu-id="735ae-139">Int32</span><span class="sxs-lookup"><span data-stu-id="735ae-139">Int32</span></span>|<span data-ttu-id="735ae-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="735ae-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="735ae-141">successCount</span><span class="sxs-lookup"><span data-stu-id="735ae-141">successCount</span></span>|<span data-ttu-id="735ae-142">Int32</span><span class="sxs-lookup"><span data-stu-id="735ae-142">Int32</span></span>|<span data-ttu-id="735ae-143">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="735ae-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="735ae-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="735ae-144">errorCount</span></span>|<span data-ttu-id="735ae-145">Int32</span><span class="sxs-lookup"><span data-stu-id="735ae-145">Int32</span></span>|<span data-ttu-id="735ae-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="735ae-146">Number of error devices</span></span>|
|<span data-ttu-id="735ae-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="735ae-147">failedCount</span></span>|<span data-ttu-id="735ae-148">Int32</span><span class="sxs-lookup"><span data-stu-id="735ae-148">Int32</span></span>|<span data-ttu-id="735ae-149">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="735ae-149">Number of failed devices</span></span>|
|<span data-ttu-id="735ae-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="735ae-150">lastUpdateDateTime</span></span>|<span data-ttu-id="735ae-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="735ae-151">DateTimeOffset</span></span>|<span data-ttu-id="735ae-152">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="735ae-152">Last update time</span></span>|
|<span data-ttu-id="735ae-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="735ae-153">configurationVersion</span></span>|<span data-ttu-id="735ae-154">Int32</span><span class="sxs-lookup"><span data-stu-id="735ae-154">Int32</span></span>|<span data-ttu-id="735ae-155">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="735ae-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="735ae-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="735ae-156">Response</span></span>
<span data-ttu-id="735ae-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="735ae-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="735ae-158">Пример</span><span class="sxs-lookup"><span data-stu-id="735ae-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="735ae-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="735ae-159">Request</span></span>
<span data-ttu-id="735ae-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="735ae-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="735ae-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="735ae-161">Response</span></span>
<span data-ttu-id="735ae-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="735ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









