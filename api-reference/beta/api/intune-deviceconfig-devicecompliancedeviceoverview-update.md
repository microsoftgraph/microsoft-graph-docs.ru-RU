---
title: Обновление объекта deviceComplianceDeviceOverview
description: Обновление свойств объекта deviceComplianceDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 786c774ac4d0b10492b946eb9e8395799d3d08a0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949758"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="71d52-103">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="71d52-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="71d52-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71d52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71d52-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71d52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71d52-106">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="71d52-106">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71d52-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="71d52-107">Prerequisites</span></span>
<span data-ttu-id="71d52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71d52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71d52-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71d52-110">Permission type</span></span>|<span data-ttu-id="71d52-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71d52-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71d52-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71d52-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71d52-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71d52-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71d52-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71d52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71d52-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71d52-115">Not supported.</span></span>|
|<span data-ttu-id="71d52-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71d52-116">Application</span></span>|<span data-ttu-id="71d52-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71d52-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71d52-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71d52-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="71d52-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="71d52-119">Request headers</span></span>
|<span data-ttu-id="71d52-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71d52-120">Header</span></span>|<span data-ttu-id="71d52-121">Значение</span><span class="sxs-lookup"><span data-stu-id="71d52-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71d52-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71d52-122">Authorization</span></span>|<span data-ttu-id="71d52-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71d52-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71d52-124">Accept</span><span class="sxs-lookup"><span data-stu-id="71d52-124">Accept</span></span>|<span data-ttu-id="71d52-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71d52-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71d52-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71d52-126">Request body</span></span>
<span data-ttu-id="71d52-127">В тексте запроса добавьте представление объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71d52-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="71d52-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="71d52-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="71d52-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="71d52-129">Property</span></span>|<span data-ttu-id="71d52-130">Тип</span><span class="sxs-lookup"><span data-stu-id="71d52-130">Type</span></span>|<span data-ttu-id="71d52-131">Описание</span><span class="sxs-lookup"><span data-stu-id="71d52-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d52-132">id</span><span class="sxs-lookup"><span data-stu-id="71d52-132">id</span></span>|<span data-ttu-id="71d52-133">Строка</span><span class="sxs-lookup"><span data-stu-id="71d52-133">String</span></span>|<span data-ttu-id="71d52-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71d52-134">Key of the entity.</span></span>|
|<span data-ttu-id="71d52-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="71d52-135">pendingCount</span></span>|<span data-ttu-id="71d52-136">Int32</span><span class="sxs-lookup"><span data-stu-id="71d52-136">Int32</span></span>|<span data-ttu-id="71d52-137">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="71d52-137">Number of pending devices</span></span>|
|<span data-ttu-id="71d52-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="71d52-138">notApplicableCount</span></span>|<span data-ttu-id="71d52-139">Int32</span><span class="sxs-lookup"><span data-stu-id="71d52-139">Int32</span></span>|<span data-ttu-id="71d52-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="71d52-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="71d52-141">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="71d52-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="71d52-142">Int32</span><span class="sxs-lookup"><span data-stu-id="71d52-142">Int32</span></span>|<span data-ttu-id="71d52-143">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="71d52-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="71d52-144">successCount</span><span class="sxs-lookup"><span data-stu-id="71d52-144">successCount</span></span>|<span data-ttu-id="71d52-145">Int32</span><span class="sxs-lookup"><span data-stu-id="71d52-145">Int32</span></span>|<span data-ttu-id="71d52-146">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="71d52-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="71d52-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="71d52-147">errorCount</span></span>|<span data-ttu-id="71d52-148">Int32</span><span class="sxs-lookup"><span data-stu-id="71d52-148">Int32</span></span>|<span data-ttu-id="71d52-149">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="71d52-149">Number of error devices</span></span>|
|<span data-ttu-id="71d52-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="71d52-150">failedCount</span></span>|<span data-ttu-id="71d52-151">Int32</span><span class="sxs-lookup"><span data-stu-id="71d52-151">Int32</span></span>|<span data-ttu-id="71d52-152">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="71d52-152">Number of failed devices</span></span>|
|<span data-ttu-id="71d52-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="71d52-153">conflictCount</span></span>|<span data-ttu-id="71d52-154">Int32</span><span class="sxs-lookup"><span data-stu-id="71d52-154">Int32</span></span>|<span data-ttu-id="71d52-155">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="71d52-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="71d52-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="71d52-156">lastUpdateDateTime</span></span>|<span data-ttu-id="71d52-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71d52-157">DateTimeOffset</span></span>|<span data-ttu-id="71d52-158">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="71d52-158">Last update time</span></span>|
|<span data-ttu-id="71d52-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="71d52-159">configurationVersion</span></span>|<span data-ttu-id="71d52-160">Int32</span><span class="sxs-lookup"><span data-stu-id="71d52-160">Int32</span></span>|<span data-ttu-id="71d52-161">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="71d52-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="71d52-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="71d52-162">Response</span></span>
<span data-ttu-id="71d52-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71d52-163">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71d52-164">Пример</span><span class="sxs-lookup"><span data-stu-id="71d52-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="71d52-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="71d52-165">Request</span></span>
<span data-ttu-id="71d52-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71d52-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="71d52-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="71d52-167">Response</span></span>
<span data-ttu-id="71d52-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71d52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





