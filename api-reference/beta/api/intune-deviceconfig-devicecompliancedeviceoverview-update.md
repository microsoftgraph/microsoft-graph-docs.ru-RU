---
title: Обновление объекта deviceComplianceDeviceOverview
description: Обновление свойств объекта deviceComplianceDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40f4e3843f098e81f70afba440cd2aec0a474144
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443260"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="e7b4a-103">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e7b4a-103">Update deviceComplianceDeviceOverview</span></span>

<span data-ttu-id="e7b4a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e7b4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7b4a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7b4a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7b4a-107">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="e7b4a-107">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7b4a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7b4a-108">Prerequisites</span></span>
<span data-ttu-id="e7b4a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7b4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7b4a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7b4a-111">Permission type</span></span>|<span data-ttu-id="e7b4a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7b4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7b4a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7b4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7b4a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7b4a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7b4a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7b4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7b4a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-116">Not supported.</span></span>|
|<span data-ttu-id="e7b4a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7b4a-117">Application</span></span>|<span data-ttu-id="e7b4a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7b4a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7b4a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7b4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="e7b4a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e7b4a-120">Request headers</span></span>
|<span data-ttu-id="e7b4a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7b4a-121">Header</span></span>|<span data-ttu-id="e7b4a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e7b4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7b4a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7b4a-123">Authorization</span></span>|<span data-ttu-id="e7b4a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7b4a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e7b4a-125">Accept</span></span>|<span data-ttu-id="e7b4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7b4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7b4a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7b4a-127">Request body</span></span>
<span data-ttu-id="e7b4a-128">В тексте запроса добавьте представление объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="e7b4a-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="e7b4a-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="e7b4a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7b4a-130">Property</span></span>|<span data-ttu-id="e7b4a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e7b4a-131">Type</span></span>|<span data-ttu-id="e7b4a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e7b4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7b4a-133">id</span><span class="sxs-lookup"><span data-stu-id="e7b4a-133">id</span></span>|<span data-ttu-id="e7b4a-134">String</span><span class="sxs-lookup"><span data-stu-id="e7b4a-134">String</span></span>|<span data-ttu-id="e7b4a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-135">Key of the entity.</span></span>|
|<span data-ttu-id="e7b4a-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e7b4a-136">pendingCount</span></span>|<span data-ttu-id="e7b4a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e7b4a-137">Int32</span></span>|<span data-ttu-id="e7b4a-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-138">Number of pending devices</span></span>|
|<span data-ttu-id="e7b4a-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e7b4a-139">notApplicableCount</span></span>|<span data-ttu-id="e7b4a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e7b4a-140">Int32</span></span>|<span data-ttu-id="e7b4a-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="e7b4a-142">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="e7b4a-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="e7b4a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e7b4a-143">Int32</span></span>|<span data-ttu-id="e7b4a-144">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="e7b4a-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="e7b4a-145">successCount</span><span class="sxs-lookup"><span data-stu-id="e7b4a-145">successCount</span></span>|<span data-ttu-id="e7b4a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e7b4a-146">Int32</span></span>|<span data-ttu-id="e7b4a-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="e7b4a-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="e7b4a-148">errorCount</span></span>|<span data-ttu-id="e7b4a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e7b4a-149">Int32</span></span>|<span data-ttu-id="e7b4a-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-150">Number of error devices</span></span>|
|<span data-ttu-id="e7b4a-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="e7b4a-151">failedCount</span></span>|<span data-ttu-id="e7b4a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e7b4a-152">Int32</span></span>|<span data-ttu-id="e7b4a-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-153">Number of failed devices</span></span>|
|<span data-ttu-id="e7b4a-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="e7b4a-154">conflictCount</span></span>|<span data-ttu-id="e7b4a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e7b4a-155">Int32</span></span>|<span data-ttu-id="e7b4a-156">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="e7b4a-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="e7b4a-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e7b4a-157">lastUpdateDateTime</span></span>|<span data-ttu-id="e7b4a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7b4a-158">DateTimeOffset</span></span>|<span data-ttu-id="e7b4a-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-159">Last update time</span></span>|
|<span data-ttu-id="e7b4a-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e7b4a-160">configurationVersion</span></span>|<span data-ttu-id="e7b4a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e7b4a-161">Int32</span></span>|<span data-ttu-id="e7b4a-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="e7b4a-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7b4a-163">Response</span></span>
<span data-ttu-id="e7b4a-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-164">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7b4a-165">Пример</span><span class="sxs-lookup"><span data-stu-id="e7b4a-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7b4a-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7b4a-166">Request</span></span>
<span data-ttu-id="e7b4a-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="e7b4a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7b4a-168">Response</span></span>
<span data-ttu-id="e7b4a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7b4a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





