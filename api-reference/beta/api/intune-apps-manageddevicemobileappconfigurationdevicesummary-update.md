---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4228b321fef3dbda9ba8be6addebeddb68e345c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445143"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="4e610-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="4e610-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="4e610-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4e610-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e610-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e610-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e610-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e610-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e610-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4e610-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e610-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e610-108">Prerequisites</span></span>
<span data-ttu-id="4e610-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e610-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e610-111">Permission type</span></span>|<span data-ttu-id="4e610-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e610-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e610-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e610-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e610-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e610-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e610-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e610-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e610-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e610-116">Not supported.</span></span>|
|<span data-ttu-id="4e610-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e610-117">Application</span></span>|<span data-ttu-id="4e610-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e610-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e610-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e610-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="4e610-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e610-120">Request headers</span></span>
|<span data-ttu-id="4e610-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e610-121">Header</span></span>|<span data-ttu-id="4e610-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e610-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e610-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e610-123">Authorization</span></span>|<span data-ttu-id="4e610-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e610-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e610-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e610-125">Accept</span></span>|<span data-ttu-id="4e610-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e610-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e610-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e610-127">Request body</span></span>
<span data-ttu-id="4e610-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e610-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="4e610-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4e610-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="4e610-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e610-130">Property</span></span>|<span data-ttu-id="4e610-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e610-131">Type</span></span>|<span data-ttu-id="4e610-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e610-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e610-133">id</span><span class="sxs-lookup"><span data-stu-id="4e610-133">id</span></span>|<span data-ttu-id="4e610-134">String</span><span class="sxs-lookup"><span data-stu-id="4e610-134">String</span></span>|<span data-ttu-id="4e610-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4e610-135">Key of the entity.</span></span>|
|<span data-ttu-id="4e610-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4e610-136">pendingCount</span></span>|<span data-ttu-id="4e610-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4e610-137">Int32</span></span>|<span data-ttu-id="4e610-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="4e610-138">Number of pending devices</span></span>|
|<span data-ttu-id="4e610-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4e610-139">notApplicableCount</span></span>|<span data-ttu-id="4e610-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4e610-140">Int32</span></span>|<span data-ttu-id="4e610-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="4e610-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="4e610-142">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="4e610-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="4e610-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4e610-143">Int32</span></span>|<span data-ttu-id="4e610-144">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="4e610-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="4e610-145">successCount</span><span class="sxs-lookup"><span data-stu-id="4e610-145">successCount</span></span>|<span data-ttu-id="4e610-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4e610-146">Int32</span></span>|<span data-ttu-id="4e610-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="4e610-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="4e610-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="4e610-148">errorCount</span></span>|<span data-ttu-id="4e610-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4e610-149">Int32</span></span>|<span data-ttu-id="4e610-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="4e610-150">Number of error devices</span></span>|
|<span data-ttu-id="4e610-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="4e610-151">failedCount</span></span>|<span data-ttu-id="4e610-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4e610-152">Int32</span></span>|<span data-ttu-id="4e610-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="4e610-153">Number of failed devices</span></span>|
|<span data-ttu-id="4e610-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="4e610-154">conflictCount</span></span>|<span data-ttu-id="4e610-155">Int32</span><span class="sxs-lookup"><span data-stu-id="4e610-155">Int32</span></span>|<span data-ttu-id="4e610-156">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="4e610-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="4e610-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4e610-157">lastUpdateDateTime</span></span>|<span data-ttu-id="4e610-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e610-158">DateTimeOffset</span></span>|<span data-ttu-id="4e610-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="4e610-159">Last update time</span></span>|
|<span data-ttu-id="4e610-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4e610-160">configurationVersion</span></span>|<span data-ttu-id="4e610-161">Int32</span><span class="sxs-lookup"><span data-stu-id="4e610-161">Int32</span></span>|<span data-ttu-id="4e610-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="4e610-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="4e610-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e610-163">Response</span></span>
<span data-ttu-id="4e610-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e610-164">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e610-165">Пример</span><span class="sxs-lookup"><span data-stu-id="4e610-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e610-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e610-166">Request</span></span>
<span data-ttu-id="4e610-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e610-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e610-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e610-168">Response</span></span>
<span data-ttu-id="4e610-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e610-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





