---
title: Create settingStateDeviceSummary
description: Создание объекта settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cc4570a3aa4a98ba1ac4b4605295b7f0bdd3923
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695693"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="d4101-103">Create settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="d4101-103">Create settingStateDeviceSummary</span></span>

<span data-ttu-id="d4101-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4101-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4101-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4101-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4101-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4101-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4101-107">Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d4101-107">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4101-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d4101-108">Prerequisites</span></span>
<span data-ttu-id="d4101-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4101-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4101-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4101-111">Permission type</span></span>|<span data-ttu-id="d4101-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4101-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4101-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4101-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4101-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4101-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4101-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4101-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4101-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4101-116">Not supported.</span></span>|
|<span data-ttu-id="d4101-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4101-117">Application</span></span>|<span data-ttu-id="d4101-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4101-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4101-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4101-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d4101-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4101-120">Request headers</span></span>
|<span data-ttu-id="d4101-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4101-121">Header</span></span>|<span data-ttu-id="d4101-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4101-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4101-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4101-123">Authorization</span></span>|<span data-ttu-id="d4101-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4101-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4101-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4101-125">Accept</span></span>|<span data-ttu-id="d4101-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4101-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4101-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4101-127">Request body</span></span>
<span data-ttu-id="d4101-128">В теле запроса добавьте представление объекта settingStateDeviceSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4101-128">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="d4101-129">Ниже показаны свойства, которые необходимо указывать при создании объекта settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="d4101-129">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="d4101-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4101-130">Property</span></span>|<span data-ttu-id="d4101-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d4101-131">Type</span></span>|<span data-ttu-id="d4101-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d4101-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4101-133">id</span><span class="sxs-lookup"><span data-stu-id="d4101-133">id</span></span>|<span data-ttu-id="d4101-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d4101-134">String</span></span>|<span data-ttu-id="d4101-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d4101-135">Key of the entity.</span></span>|
|<span data-ttu-id="d4101-136">settingName</span><span class="sxs-lookup"><span data-stu-id="d4101-136">settingName</span></span>|<span data-ttu-id="d4101-137">String</span><span class="sxs-lookup"><span data-stu-id="d4101-137">String</span></span>|<span data-ttu-id="d4101-138">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="d4101-138">Name of the setting</span></span>|
|<span data-ttu-id="d4101-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="d4101-139">instancePath</span></span>|<span data-ttu-id="d4101-140">String</span><span class="sxs-lookup"><span data-stu-id="d4101-140">String</span></span>|<span data-ttu-id="d4101-141">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="d4101-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="d4101-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4101-142">unknownDeviceCount</span></span>|<span data-ttu-id="d4101-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d4101-143">Int32</span></span>|<span data-ttu-id="d4101-144">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="d4101-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="d4101-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4101-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="d4101-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d4101-146">Int32</span></span>|<span data-ttu-id="d4101-147">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="d4101-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="d4101-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4101-148">compliantDeviceCount</span></span>|<span data-ttu-id="d4101-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d4101-149">Int32</span></span>|<span data-ttu-id="d4101-150">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="d4101-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="d4101-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4101-151">remediatedDeviceCount</span></span>|<span data-ttu-id="d4101-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d4101-152">Int32</span></span>|<span data-ttu-id="d4101-153">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="d4101-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="d4101-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4101-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d4101-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d4101-155">Int32</span></span>|<span data-ttu-id="d4101-156">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="d4101-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="d4101-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4101-157">errorDeviceCount</span></span>|<span data-ttu-id="d4101-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d4101-158">Int32</span></span>|<span data-ttu-id="d4101-159">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="d4101-159">Device error count for the setting</span></span>|
|<span data-ttu-id="d4101-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4101-160">conflictDeviceCount</span></span>|<span data-ttu-id="d4101-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d4101-161">Int32</span></span>|<span data-ttu-id="d4101-162">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="d4101-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="d4101-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4101-163">Response</span></span>
<span data-ttu-id="d4101-164">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d4101-164">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4101-165">Пример</span><span class="sxs-lookup"><span data-stu-id="d4101-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4101-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4101-166">Request</span></span>
<span data-ttu-id="d4101-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4101-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="d4101-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4101-168">Response</span></span>
<span data-ttu-id="d4101-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4101-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





