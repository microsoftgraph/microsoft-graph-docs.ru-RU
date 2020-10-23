---
title: Обновление объекта deviceConfigurationDeviceOverview
description: Обновление свойств объекта deviceConfigurationDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a22f867eb3ac32070537b4423e374dbee294d960
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689813"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="0454d-103">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0454d-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="0454d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0454d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0454d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0454d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0454d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0454d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0454d-107">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="0454d-107">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0454d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0454d-108">Prerequisites</span></span>
<span data-ttu-id="0454d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0454d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0454d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0454d-111">Permission type</span></span>|<span data-ttu-id="0454d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0454d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0454d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0454d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0454d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0454d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0454d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0454d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0454d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0454d-116">Not supported.</span></span>|
|<span data-ttu-id="0454d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0454d-117">Application</span></span>|<span data-ttu-id="0454d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0454d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0454d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0454d-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="0454d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0454d-120">Request headers</span></span>
|<span data-ttu-id="0454d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0454d-121">Header</span></span>|<span data-ttu-id="0454d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0454d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0454d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0454d-123">Authorization</span></span>|<span data-ttu-id="0454d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0454d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0454d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0454d-125">Accept</span></span>|<span data-ttu-id="0454d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0454d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0454d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0454d-127">Request body</span></span>
<span data-ttu-id="0454d-128">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0454d-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="0454d-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="0454d-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="0454d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0454d-130">Property</span></span>|<span data-ttu-id="0454d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0454d-131">Type</span></span>|<span data-ttu-id="0454d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0454d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0454d-133">id</span><span class="sxs-lookup"><span data-stu-id="0454d-133">id</span></span>|<span data-ttu-id="0454d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0454d-134">String</span></span>|<span data-ttu-id="0454d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0454d-135">Key of the entity.</span></span>|
|<span data-ttu-id="0454d-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="0454d-136">pendingCount</span></span>|<span data-ttu-id="0454d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0454d-137">Int32</span></span>|<span data-ttu-id="0454d-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="0454d-138">Number of pending devices</span></span>|
|<span data-ttu-id="0454d-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0454d-139">notApplicableCount</span></span>|<span data-ttu-id="0454d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0454d-140">Int32</span></span>|<span data-ttu-id="0454d-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="0454d-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="0454d-142">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="0454d-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="0454d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0454d-143">Int32</span></span>|<span data-ttu-id="0454d-144">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="0454d-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="0454d-145">successCount</span><span class="sxs-lookup"><span data-stu-id="0454d-145">successCount</span></span>|<span data-ttu-id="0454d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0454d-146">Int32</span></span>|<span data-ttu-id="0454d-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="0454d-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="0454d-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="0454d-148">errorCount</span></span>|<span data-ttu-id="0454d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0454d-149">Int32</span></span>|<span data-ttu-id="0454d-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="0454d-150">Number of error devices</span></span>|
|<span data-ttu-id="0454d-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="0454d-151">failedCount</span></span>|<span data-ttu-id="0454d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0454d-152">Int32</span></span>|<span data-ttu-id="0454d-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="0454d-153">Number of failed devices</span></span>|
|<span data-ttu-id="0454d-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="0454d-154">conflictCount</span></span>|<span data-ttu-id="0454d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="0454d-155">Int32</span></span>|<span data-ttu-id="0454d-156">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="0454d-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="0454d-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0454d-157">lastUpdateDateTime</span></span>|<span data-ttu-id="0454d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0454d-158">DateTimeOffset</span></span>|<span data-ttu-id="0454d-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="0454d-159">Last update time</span></span>|
|<span data-ttu-id="0454d-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="0454d-160">configurationVersion</span></span>|<span data-ttu-id="0454d-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0454d-161">Int32</span></span>|<span data-ttu-id="0454d-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="0454d-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="0454d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="0454d-163">Response</span></span>
<span data-ttu-id="0454d-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0454d-164">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0454d-165">Пример</span><span class="sxs-lookup"><span data-stu-id="0454d-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="0454d-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="0454d-166">Request</span></span>
<span data-ttu-id="0454d-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0454d-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0454d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="0454d-168">Response</span></span>
<span data-ttu-id="0454d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0454d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





