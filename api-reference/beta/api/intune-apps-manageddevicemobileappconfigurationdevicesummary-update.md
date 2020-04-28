---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b832c02b12bda6586af93ae16e3a4f2c3d3ecda8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405749"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="e1cfc-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e1cfc-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="e1cfc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1cfc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1cfc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1cfc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1cfc-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e1cfc-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1cfc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e1cfc-108">Prerequisites</span></span>
<span data-ttu-id="e1cfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1cfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1cfc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1cfc-111">Permission type</span></span>|<span data-ttu-id="e1cfc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1cfc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1cfc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1cfc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1cfc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1cfc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e1cfc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1cfc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1cfc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-116">Not supported.</span></span>|
|<span data-ttu-id="e1cfc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1cfc-117">Application</span></span>|<span data-ttu-id="e1cfc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1cfc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1cfc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1cfc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="e1cfc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e1cfc-120">Request headers</span></span>
|<span data-ttu-id="e1cfc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1cfc-121">Header</span></span>|<span data-ttu-id="e1cfc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1cfc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1cfc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1cfc-123">Authorization</span></span>|<span data-ttu-id="e1cfc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1cfc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1cfc-125">Accept</span></span>|<span data-ttu-id="e1cfc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1cfc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1cfc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1cfc-127">Request body</span></span>
<span data-ttu-id="e1cfc-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="e1cfc-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e1cfc-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="e1cfc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1cfc-130">Property</span></span>|<span data-ttu-id="e1cfc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e1cfc-131">Type</span></span>|<span data-ttu-id="e1cfc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e1cfc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1cfc-133">id</span><span class="sxs-lookup"><span data-stu-id="e1cfc-133">id</span></span>|<span data-ttu-id="e1cfc-134">String</span><span class="sxs-lookup"><span data-stu-id="e1cfc-134">String</span></span>|<span data-ttu-id="e1cfc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-135">Key of the entity.</span></span>|
|<span data-ttu-id="e1cfc-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e1cfc-136">pendingCount</span></span>|<span data-ttu-id="e1cfc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cfc-137">Int32</span></span>|<span data-ttu-id="e1cfc-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-138">Number of pending devices</span></span>|
|<span data-ttu-id="e1cfc-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e1cfc-139">notApplicableCount</span></span>|<span data-ttu-id="e1cfc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cfc-140">Int32</span></span>|<span data-ttu-id="e1cfc-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="e1cfc-142">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="e1cfc-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="e1cfc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cfc-143">Int32</span></span>|<span data-ttu-id="e1cfc-144">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="e1cfc-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="e1cfc-145">successCount</span><span class="sxs-lookup"><span data-stu-id="e1cfc-145">successCount</span></span>|<span data-ttu-id="e1cfc-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cfc-146">Int32</span></span>|<span data-ttu-id="e1cfc-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="e1cfc-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="e1cfc-148">errorCount</span></span>|<span data-ttu-id="e1cfc-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cfc-149">Int32</span></span>|<span data-ttu-id="e1cfc-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-150">Number of error devices</span></span>|
|<span data-ttu-id="e1cfc-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="e1cfc-151">failedCount</span></span>|<span data-ttu-id="e1cfc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cfc-152">Int32</span></span>|<span data-ttu-id="e1cfc-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-153">Number of failed devices</span></span>|
|<span data-ttu-id="e1cfc-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="e1cfc-154">conflictCount</span></span>|<span data-ttu-id="e1cfc-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cfc-155">Int32</span></span>|<span data-ttu-id="e1cfc-156">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="e1cfc-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="e1cfc-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e1cfc-157">lastUpdateDateTime</span></span>|<span data-ttu-id="e1cfc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1cfc-158">DateTimeOffset</span></span>|<span data-ttu-id="e1cfc-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-159">Last update time</span></span>|
|<span data-ttu-id="e1cfc-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e1cfc-160">configurationVersion</span></span>|<span data-ttu-id="e1cfc-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cfc-161">Int32</span></span>|<span data-ttu-id="e1cfc-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="e1cfc-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1cfc-163">Response</span></span>
<span data-ttu-id="e1cfc-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-164">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1cfc-165">Пример</span><span class="sxs-lookup"><span data-stu-id="e1cfc-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1cfc-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1cfc-166">Request</span></span>
<span data-ttu-id="e1cfc-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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

### <a name="response"></a><span data-ttu-id="e1cfc-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1cfc-168">Response</span></span>
<span data-ttu-id="e1cfc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1cfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
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



