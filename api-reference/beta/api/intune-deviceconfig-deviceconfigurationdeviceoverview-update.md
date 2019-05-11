---
title: Обновление объекта deviceConfigurationDeviceOverview
description: Обновление свойств объекта deviceConfigurationDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c536d5dbd1f295ea85e58c0fa6592969253a717f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927421"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="56220-103">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="56220-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="56220-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56220-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56220-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56220-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56220-106">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="56220-106">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56220-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="56220-107">Prerequisites</span></span>
<span data-ttu-id="56220-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56220-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56220-110">Permission type</span></span>|<span data-ttu-id="56220-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56220-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56220-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56220-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56220-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56220-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56220-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56220-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56220-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56220-115">Not supported.</span></span>|
|<span data-ttu-id="56220-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56220-116">Application</span></span>|<span data-ttu-id="56220-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56220-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56220-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56220-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="56220-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56220-119">Request headers</span></span>
|<span data-ttu-id="56220-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56220-120">Header</span></span>|<span data-ttu-id="56220-121">Значение</span><span class="sxs-lookup"><span data-stu-id="56220-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56220-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56220-122">Authorization</span></span>|<span data-ttu-id="56220-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56220-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56220-124">Accept</span><span class="sxs-lookup"><span data-stu-id="56220-124">Accept</span></span>|<span data-ttu-id="56220-125">application/json</span><span class="sxs-lookup"><span data-stu-id="56220-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56220-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56220-126">Request body</span></span>
<span data-ttu-id="56220-127">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56220-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="56220-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="56220-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="56220-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="56220-129">Property</span></span>|<span data-ttu-id="56220-130">Тип</span><span class="sxs-lookup"><span data-stu-id="56220-130">Type</span></span>|<span data-ttu-id="56220-131">Описание</span><span class="sxs-lookup"><span data-stu-id="56220-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56220-132">id</span><span class="sxs-lookup"><span data-stu-id="56220-132">id</span></span>|<span data-ttu-id="56220-133">Строка</span><span class="sxs-lookup"><span data-stu-id="56220-133">String</span></span>|<span data-ttu-id="56220-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="56220-134">Key of the entity.</span></span>|
|<span data-ttu-id="56220-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="56220-135">pendingCount</span></span>|<span data-ttu-id="56220-136">Int32</span><span class="sxs-lookup"><span data-stu-id="56220-136">Int32</span></span>|<span data-ttu-id="56220-137">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="56220-137">Number of pending devices</span></span>|
|<span data-ttu-id="56220-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="56220-138">notApplicableCount</span></span>|<span data-ttu-id="56220-139">Int32</span><span class="sxs-lookup"><span data-stu-id="56220-139">Int32</span></span>|<span data-ttu-id="56220-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="56220-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="56220-141">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="56220-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="56220-142">Int32</span><span class="sxs-lookup"><span data-stu-id="56220-142">Int32</span></span>|<span data-ttu-id="56220-143">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="56220-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="56220-144">successCount</span><span class="sxs-lookup"><span data-stu-id="56220-144">successCount</span></span>|<span data-ttu-id="56220-145">Int32</span><span class="sxs-lookup"><span data-stu-id="56220-145">Int32</span></span>|<span data-ttu-id="56220-146">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="56220-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="56220-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="56220-147">errorCount</span></span>|<span data-ttu-id="56220-148">Int32</span><span class="sxs-lookup"><span data-stu-id="56220-148">Int32</span></span>|<span data-ttu-id="56220-149">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="56220-149">Number of error devices</span></span>|
|<span data-ttu-id="56220-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="56220-150">failedCount</span></span>|<span data-ttu-id="56220-151">Int32</span><span class="sxs-lookup"><span data-stu-id="56220-151">Int32</span></span>|<span data-ttu-id="56220-152">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="56220-152">Number of failed devices</span></span>|
|<span data-ttu-id="56220-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="56220-153">conflictCount</span></span>|<span data-ttu-id="56220-154">Int32</span><span class="sxs-lookup"><span data-stu-id="56220-154">Int32</span></span>|<span data-ttu-id="56220-155">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="56220-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="56220-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="56220-156">lastUpdateDateTime</span></span>|<span data-ttu-id="56220-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56220-157">DateTimeOffset</span></span>|<span data-ttu-id="56220-158">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="56220-158">Last update time</span></span>|
|<span data-ttu-id="56220-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="56220-159">configurationVersion</span></span>|<span data-ttu-id="56220-160">Int32</span><span class="sxs-lookup"><span data-stu-id="56220-160">Int32</span></span>|<span data-ttu-id="56220-161">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="56220-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="56220-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="56220-162">Response</span></span>
<span data-ttu-id="56220-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56220-163">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56220-164">Пример</span><span class="sxs-lookup"><span data-stu-id="56220-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="56220-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="56220-165">Request</span></span>
<span data-ttu-id="56220-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56220-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
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

### <a name="response"></a><span data-ttu-id="56220-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="56220-167">Response</span></span>
<span data-ttu-id="56220-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56220-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
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




