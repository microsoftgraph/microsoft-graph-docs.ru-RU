---
title: Обновление объекта deviceComplianceDeviceOverview
description: Обновление свойств объекта deviceComplianceDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75ee43dd6eb3a1daf605350cb32906dbf5e1a94b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340284"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="9e9ab-103">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9e9ab-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="9e9ab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e9ab-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e9ab-106">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="9e9ab-106">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e9ab-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9e9ab-107">Prerequisites</span></span>
<span data-ttu-id="9e9ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e9ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e9ab-110">Permission type</span></span>|<span data-ttu-id="9e9ab-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e9ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e9ab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e9ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e9ab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e9ab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e9ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e9ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e9ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-115">Not supported.</span></span>|
|<span data-ttu-id="9e9ab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e9ab-116">Application</span></span>|<span data-ttu-id="9e9ab-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e9ab-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e9ab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e9ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="9e9ab-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e9ab-119">Request headers</span></span>
|<span data-ttu-id="9e9ab-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e9ab-120">Header</span></span>|<span data-ttu-id="9e9ab-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9e9ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e9ab-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e9ab-122">Authorization</span></span>|<span data-ttu-id="9e9ab-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e9ab-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9e9ab-124">Accept</span></span>|<span data-ttu-id="9e9ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e9ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e9ab-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e9ab-126">Request body</span></span>
<span data-ttu-id="9e9ab-127">В тексте запроса добавьте представление объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="9e9ab-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="9e9ab-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="9e9ab-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e9ab-129">Property</span></span>|<span data-ttu-id="9e9ab-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9e9ab-130">Type</span></span>|<span data-ttu-id="9e9ab-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9e9ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e9ab-132">id</span><span class="sxs-lookup"><span data-stu-id="9e9ab-132">id</span></span>|<span data-ttu-id="9e9ab-133">String</span><span class="sxs-lookup"><span data-stu-id="9e9ab-133">String</span></span>|<span data-ttu-id="9e9ab-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-134">Key of the entity.</span></span>|
|<span data-ttu-id="9e9ab-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="9e9ab-135">pendingCount</span></span>|<span data-ttu-id="9e9ab-136">Int32</span><span class="sxs-lookup"><span data-stu-id="9e9ab-136">Int32</span></span>|<span data-ttu-id="9e9ab-137">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-137">Number of pending devices</span></span>|
|<span data-ttu-id="9e9ab-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9e9ab-138">notApplicableCount</span></span>|<span data-ttu-id="9e9ab-139">Int32</span><span class="sxs-lookup"><span data-stu-id="9e9ab-139">Int32</span></span>|<span data-ttu-id="9e9ab-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="9e9ab-141">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="9e9ab-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="9e9ab-142">Int32</span><span class="sxs-lookup"><span data-stu-id="9e9ab-142">Int32</span></span>|<span data-ttu-id="9e9ab-143">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="9e9ab-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="9e9ab-144">successCount</span><span class="sxs-lookup"><span data-stu-id="9e9ab-144">successCount</span></span>|<span data-ttu-id="9e9ab-145">Int32</span><span class="sxs-lookup"><span data-stu-id="9e9ab-145">Int32</span></span>|<span data-ttu-id="9e9ab-146">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="9e9ab-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="9e9ab-147">errorCount</span></span>|<span data-ttu-id="9e9ab-148">Int32</span><span class="sxs-lookup"><span data-stu-id="9e9ab-148">Int32</span></span>|<span data-ttu-id="9e9ab-149">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-149">Number of error devices</span></span>|
|<span data-ttu-id="9e9ab-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="9e9ab-150">failedCount</span></span>|<span data-ttu-id="9e9ab-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9e9ab-151">Int32</span></span>|<span data-ttu-id="9e9ab-152">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-152">Number of failed devices</span></span>|
|<span data-ttu-id="9e9ab-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9e9ab-153">conflictCount</span></span>|<span data-ttu-id="9e9ab-154">Int32</span><span class="sxs-lookup"><span data-stu-id="9e9ab-154">Int32</span></span>|<span data-ttu-id="9e9ab-155">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="9e9ab-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="9e9ab-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9e9ab-156">lastUpdateDateTime</span></span>|<span data-ttu-id="9e9ab-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e9ab-157">DateTimeOffset</span></span>|<span data-ttu-id="9e9ab-158">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-158">Last update time</span></span>|
|<span data-ttu-id="9e9ab-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="9e9ab-159">configurationVersion</span></span>|<span data-ttu-id="9e9ab-160">Int32</span><span class="sxs-lookup"><span data-stu-id="9e9ab-160">Int32</span></span>|<span data-ttu-id="9e9ab-161">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="9e9ab-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9ab-162">Response</span></span>
<span data-ttu-id="9e9ab-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-163">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e9ab-164">Пример</span><span class="sxs-lookup"><span data-stu-id="9e9ab-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e9ab-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e9ab-165">Request</span></span>
<span data-ttu-id="9e9ab-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e9ab-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9ab-167">Response</span></span>
<span data-ttu-id="9e9ab-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e9ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






