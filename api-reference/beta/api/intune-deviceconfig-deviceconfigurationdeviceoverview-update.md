---
title: Обновление объекта deviceConfigurationDeviceOverview
description: Обновление свойств объекта deviceConfigurationDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2394d047f3b262f63ecb28d202872b6219129a5a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131675"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="c5c3e-103">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c5c3e-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="c5c3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5c3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5c3e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5c3e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5c3e-107">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="c5c3e-107">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5c3e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c5c3e-108">Prerequisites</span></span>
<span data-ttu-id="c5c3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5c3e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5c3e-111">Permission type</span></span>|<span data-ttu-id="c5c3e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5c3e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5c3e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5c3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5c3e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5c3e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5c3e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5c3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5c3e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-116">Not supported.</span></span>|
|<span data-ttu-id="c5c3e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c5c3e-117">Application</span></span>|<span data-ttu-id="c5c3e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5c3e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5c3e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5c3e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c5c3e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5c3e-120">Request headers</span></span>
|<span data-ttu-id="c5c3e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5c3e-121">Header</span></span>|<span data-ttu-id="c5c3e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5c3e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5c3e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5c3e-123">Authorization</span></span>|<span data-ttu-id="c5c3e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5c3e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5c3e-125">Accept</span></span>|<span data-ttu-id="c5c3e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5c3e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5c3e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5c3e-127">Request body</span></span>
<span data-ttu-id="c5c3e-128">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="c5c3e-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="c5c3e-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="c5c3e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5c3e-130">Property</span></span>|<span data-ttu-id="c5c3e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5c3e-131">Type</span></span>|<span data-ttu-id="c5c3e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5c3e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5c3e-133">id</span><span class="sxs-lookup"><span data-stu-id="c5c3e-133">id</span></span>|<span data-ttu-id="c5c3e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c5c3e-134">String</span></span>|<span data-ttu-id="c5c3e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-135">Key of the entity.</span></span>|
|<span data-ttu-id="c5c3e-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="c5c3e-136">pendingCount</span></span>|<span data-ttu-id="c5c3e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c5c3e-137">Int32</span></span>|<span data-ttu-id="c5c3e-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-138">Number of pending devices</span></span>|
|<span data-ttu-id="c5c3e-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c5c3e-139">notApplicableCount</span></span>|<span data-ttu-id="c5c3e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c5c3e-140">Int32</span></span>|<span data-ttu-id="c5c3e-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="c5c3e-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="c5c3e-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="c5c3e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c5c3e-143">Int32</span></span>|<span data-ttu-id="c5c3e-144">Количество не применимых устройств из-за несоответствия платформы и политики</span><span class="sxs-lookup"><span data-stu-id="c5c3e-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="c5c3e-145">successCount</span><span class="sxs-lookup"><span data-stu-id="c5c3e-145">successCount</span></span>|<span data-ttu-id="c5c3e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c5c3e-146">Int32</span></span>|<span data-ttu-id="c5c3e-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="c5c3e-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="c5c3e-148">errorCount</span></span>|<span data-ttu-id="c5c3e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c5c3e-149">Int32</span></span>|<span data-ttu-id="c5c3e-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-150">Number of error devices</span></span>|
|<span data-ttu-id="c5c3e-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="c5c3e-151">failedCount</span></span>|<span data-ttu-id="c5c3e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c5c3e-152">Int32</span></span>|<span data-ttu-id="c5c3e-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-153">Number of failed devices</span></span>|
|<span data-ttu-id="c5c3e-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="c5c3e-154">conflictCount</span></span>|<span data-ttu-id="c5c3e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="c5c3e-155">Int32</span></span>|<span data-ttu-id="c5c3e-156">Количество устройств в конфликте</span><span class="sxs-lookup"><span data-stu-id="c5c3e-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="c5c3e-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="c5c3e-157">lastUpdateDateTime</span></span>|<span data-ttu-id="c5c3e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5c3e-158">DateTimeOffset</span></span>|<span data-ttu-id="c5c3e-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-159">Last update time</span></span>|
|<span data-ttu-id="c5c3e-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="c5c3e-160">configurationVersion</span></span>|<span data-ttu-id="c5c3e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c5c3e-161">Int32</span></span>|<span data-ttu-id="c5c3e-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="c5c3e-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5c3e-163">Response</span></span>
<span data-ttu-id="c5c3e-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-164">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5c3e-165">Пример</span><span class="sxs-lookup"><span data-stu-id="c5c3e-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5c3e-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5c3e-166">Request</span></span>
<span data-ttu-id="c5c3e-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5c3e-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5c3e-168">Response</span></span>
<span data-ttu-id="c5c3e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5c3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




