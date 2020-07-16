---
title: Обновление объекта deviceConfigurationDeviceOverview
description: Обновление свойств объекта deviceConfigurationDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73ab98258b40129c9ef64776a0c775b74bd64eb2
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792963"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="38944-103">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="38944-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="38944-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38944-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38944-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38944-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38944-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38944-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38944-107">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="38944-107">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38944-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="38944-108">Prerequisites</span></span>
<span data-ttu-id="38944-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38944-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38944-111">Permission type</span></span>|<span data-ttu-id="38944-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38944-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38944-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38944-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38944-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38944-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38944-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38944-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38944-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38944-116">Not supported.</span></span>|
|<span data-ttu-id="38944-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38944-117">Application</span></span>|<span data-ttu-id="38944-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38944-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38944-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38944-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="38944-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="38944-120">Request headers</span></span>
|<span data-ttu-id="38944-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38944-121">Header</span></span>|<span data-ttu-id="38944-122">Значение</span><span class="sxs-lookup"><span data-stu-id="38944-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38944-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38944-123">Authorization</span></span>|<span data-ttu-id="38944-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38944-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38944-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38944-125">Accept</span></span>|<span data-ttu-id="38944-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38944-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38944-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38944-127">Request body</span></span>
<span data-ttu-id="38944-128">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38944-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="38944-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="38944-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="38944-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="38944-130">Property</span></span>|<span data-ttu-id="38944-131">Тип</span><span class="sxs-lookup"><span data-stu-id="38944-131">Type</span></span>|<span data-ttu-id="38944-132">Описание</span><span class="sxs-lookup"><span data-stu-id="38944-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38944-133">id</span><span class="sxs-lookup"><span data-stu-id="38944-133">id</span></span>|<span data-ttu-id="38944-134">String</span><span class="sxs-lookup"><span data-stu-id="38944-134">String</span></span>|<span data-ttu-id="38944-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="38944-135">Key of the entity.</span></span>|
|<span data-ttu-id="38944-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="38944-136">pendingCount</span></span>|<span data-ttu-id="38944-137">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-137">Int32</span></span>|<span data-ttu-id="38944-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="38944-138">Number of pending devices</span></span>|
|<span data-ttu-id="38944-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="38944-139">notApplicableCount</span></span>|<span data-ttu-id="38944-140">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-140">Int32</span></span>|<span data-ttu-id="38944-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="38944-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="38944-142">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="38944-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="38944-143">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-143">Int32</span></span>|<span data-ttu-id="38944-144">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="38944-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="38944-145">successCount</span><span class="sxs-lookup"><span data-stu-id="38944-145">successCount</span></span>|<span data-ttu-id="38944-146">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-146">Int32</span></span>|<span data-ttu-id="38944-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="38944-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="38944-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="38944-148">errorCount</span></span>|<span data-ttu-id="38944-149">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-149">Int32</span></span>|<span data-ttu-id="38944-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="38944-150">Number of error devices</span></span>|
|<span data-ttu-id="38944-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="38944-151">failedCount</span></span>|<span data-ttu-id="38944-152">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-152">Int32</span></span>|<span data-ttu-id="38944-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="38944-153">Number of failed devices</span></span>|
|<span data-ttu-id="38944-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="38944-154">conflictCount</span></span>|<span data-ttu-id="38944-155">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-155">Int32</span></span>|<span data-ttu-id="38944-156">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="38944-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="38944-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="38944-157">lastUpdateDateTime</span></span>|<span data-ttu-id="38944-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38944-158">DateTimeOffset</span></span>|<span data-ttu-id="38944-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="38944-159">Last update time</span></span>|
|<span data-ttu-id="38944-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="38944-160">configurationVersion</span></span>|<span data-ttu-id="38944-161">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-161">Int32</span></span>|<span data-ttu-id="38944-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="38944-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="38944-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="38944-163">Response</span></span>
<span data-ttu-id="38944-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38944-164">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38944-165">Пример</span><span class="sxs-lookup"><span data-stu-id="38944-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="38944-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="38944-166">Request</span></span>
<span data-ttu-id="38944-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38944-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38944-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="38944-168">Response</span></span>
<span data-ttu-id="38944-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38944-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



