---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc63d8466f3cacf35d5adfaa3785d056873e24d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961527"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="e7018-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e7018-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="e7018-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7018-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7018-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7018-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7018-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e7018-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7018-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7018-107">Prerequisites</span></span>
<span data-ttu-id="e7018-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7018-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7018-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7018-110">Permission type</span></span>|<span data-ttu-id="e7018-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7018-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7018-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7018-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7018-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7018-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e7018-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7018-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7018-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7018-115">Not supported.</span></span>|
|<span data-ttu-id="e7018-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7018-116">Application</span></span>|<span data-ttu-id="e7018-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7018-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7018-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7018-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="e7018-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7018-119">Request headers</span></span>
|<span data-ttu-id="e7018-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7018-120">Header</span></span>|<span data-ttu-id="e7018-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e7018-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7018-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7018-122">Authorization</span></span>|<span data-ttu-id="e7018-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7018-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7018-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e7018-124">Accept</span></span>|<span data-ttu-id="e7018-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7018-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7018-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7018-126">Request body</span></span>
<span data-ttu-id="e7018-127">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7018-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="e7018-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e7018-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="e7018-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7018-129">Property</span></span>|<span data-ttu-id="e7018-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e7018-130">Type</span></span>|<span data-ttu-id="e7018-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e7018-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7018-132">id</span><span class="sxs-lookup"><span data-stu-id="e7018-132">id</span></span>|<span data-ttu-id="e7018-133">String</span><span class="sxs-lookup"><span data-stu-id="e7018-133">String</span></span>|<span data-ttu-id="e7018-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e7018-134">Key of the entity.</span></span>|
|<span data-ttu-id="e7018-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e7018-135">pendingCount</span></span>|<span data-ttu-id="e7018-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e7018-136">Int32</span></span>|<span data-ttu-id="e7018-137">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="e7018-137">Number of pending devices</span></span>|
|<span data-ttu-id="e7018-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e7018-138">notApplicableCount</span></span>|<span data-ttu-id="e7018-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e7018-139">Int32</span></span>|<span data-ttu-id="e7018-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e7018-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="e7018-141">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="e7018-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="e7018-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e7018-142">Int32</span></span>|<span data-ttu-id="e7018-143">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="e7018-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="e7018-144">successCount</span><span class="sxs-lookup"><span data-stu-id="e7018-144">successCount</span></span>|<span data-ttu-id="e7018-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e7018-145">Int32</span></span>|<span data-ttu-id="e7018-146">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="e7018-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="e7018-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="e7018-147">errorCount</span></span>|<span data-ttu-id="e7018-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e7018-148">Int32</span></span>|<span data-ttu-id="e7018-149">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e7018-149">Number of error devices</span></span>|
|<span data-ttu-id="e7018-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="e7018-150">failedCount</span></span>|<span data-ttu-id="e7018-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e7018-151">Int32</span></span>|<span data-ttu-id="e7018-152">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="e7018-152">Number of failed devices</span></span>|
|<span data-ttu-id="e7018-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="e7018-153">conflictCount</span></span>|<span data-ttu-id="e7018-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e7018-154">Int32</span></span>|<span data-ttu-id="e7018-155">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="e7018-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="e7018-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e7018-156">lastUpdateDateTime</span></span>|<span data-ttu-id="e7018-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7018-157">DateTimeOffset</span></span>|<span data-ttu-id="e7018-158">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="e7018-158">Last update time</span></span>|
|<span data-ttu-id="e7018-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e7018-159">configurationVersion</span></span>|<span data-ttu-id="e7018-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e7018-160">Int32</span></span>|<span data-ttu-id="e7018-161">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="e7018-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="e7018-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7018-162">Response</span></span>
<span data-ttu-id="e7018-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7018-163">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7018-164">Пример</span><span class="sxs-lookup"><span data-stu-id="e7018-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7018-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7018-165">Request</span></span>
<span data-ttu-id="e7018-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7018-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7018-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7018-167">Response</span></span>
<span data-ttu-id="e7018-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7018-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





