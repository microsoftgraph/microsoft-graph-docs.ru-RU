---
title: Обновление объекта settingStateDeviceSummary
description: Обновление свойств объекта settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 951b76545e7c11f2a17ad9f787d898e77b3023d9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792648"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="a9f80-103">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a9f80-103">Update settingStateDeviceSummary</span></span>

<span data-ttu-id="a9f80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9f80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9f80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9f80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f80-107">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a9f80-107">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9f80-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a9f80-108">Prerequisites</span></span>
<span data-ttu-id="a9f80-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a9f80-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a9f80-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9f80-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9f80-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9f80-111">Permission type</span></span>|<span data-ttu-id="a9f80-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9f80-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9f80-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9f80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9f80-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f80-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9f80-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9f80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9f80-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f80-116">Not supported.</span></span>|
|<span data-ttu-id="a9f80-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9f80-117">Application</span></span>|<span data-ttu-id="a9f80-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f80-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9f80-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9f80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a9f80-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9f80-120">Request headers</span></span>
|<span data-ttu-id="a9f80-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9f80-121">Header</span></span>|<span data-ttu-id="a9f80-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9f80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9f80-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9f80-123">Authorization</span></span>|<span data-ttu-id="a9f80-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9f80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9f80-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9f80-125">Accept</span></span>|<span data-ttu-id="a9f80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9f80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9f80-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9f80-127">Request body</span></span>
<span data-ttu-id="a9f80-128">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9f80-128">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="a9f80-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a9f80-129">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="a9f80-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9f80-130">Property</span></span>|<span data-ttu-id="a9f80-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9f80-131">Type</span></span>|<span data-ttu-id="a9f80-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9f80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f80-133">id</span><span class="sxs-lookup"><span data-stu-id="a9f80-133">id</span></span>|<span data-ttu-id="a9f80-134">String</span><span class="sxs-lookup"><span data-stu-id="a9f80-134">String</span></span>|<span data-ttu-id="a9f80-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9f80-135">Key of the entity.</span></span>|
|<span data-ttu-id="a9f80-136">settingName</span><span class="sxs-lookup"><span data-stu-id="a9f80-136">settingName</span></span>|<span data-ttu-id="a9f80-137">String</span><span class="sxs-lookup"><span data-stu-id="a9f80-137">String</span></span>|<span data-ttu-id="a9f80-138">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="a9f80-138">Name of the setting</span></span>|
|<span data-ttu-id="a9f80-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="a9f80-139">instancePath</span></span>|<span data-ttu-id="a9f80-140">String</span><span class="sxs-lookup"><span data-stu-id="a9f80-140">String</span></span>|<span data-ttu-id="a9f80-141">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="a9f80-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="a9f80-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9f80-142">unknownDeviceCount</span></span>|<span data-ttu-id="a9f80-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f80-143">Int32</span></span>|<span data-ttu-id="a9f80-144">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="a9f80-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="a9f80-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9f80-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="a9f80-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f80-146">Int32</span></span>|<span data-ttu-id="a9f80-147">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="a9f80-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="a9f80-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9f80-148">compliantDeviceCount</span></span>|<span data-ttu-id="a9f80-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f80-149">Int32</span></span>|<span data-ttu-id="a9f80-150">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="a9f80-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="a9f80-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9f80-151">remediatedDeviceCount</span></span>|<span data-ttu-id="a9f80-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f80-152">Int32</span></span>|<span data-ttu-id="a9f80-153">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="a9f80-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="a9f80-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9f80-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a9f80-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f80-155">Int32</span></span>|<span data-ttu-id="a9f80-156">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="a9f80-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="a9f80-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9f80-157">errorDeviceCount</span></span>|<span data-ttu-id="a9f80-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f80-158">Int32</span></span>|<span data-ttu-id="a9f80-159">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="a9f80-159">Device error count for the setting</span></span>|
|<span data-ttu-id="a9f80-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9f80-160">conflictDeviceCount</span></span>|<span data-ttu-id="a9f80-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f80-161">Int32</span></span>|<span data-ttu-id="a9f80-162">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="a9f80-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="a9f80-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9f80-163">Response</span></span>
<span data-ttu-id="a9f80-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a9f80-164">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9f80-165">Пример</span><span class="sxs-lookup"><span data-stu-id="a9f80-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9f80-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9f80-166">Request</span></span>
<span data-ttu-id="a9f80-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9f80-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="a9f80-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9f80-168">Response</span></span>
<span data-ttu-id="a9f80-169">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a9f80-169">Here is an example of the response.</span></span> <span data-ttu-id="a9f80-170">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a9f80-170">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a9f80-171">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a9f80-171">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



