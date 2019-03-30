---
title: Обновление объекта settingStateDeviceSummary
description: Обновление свойств объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fa47448fffacf3e48e7b9f63a34cf93b4392044
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986861"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="75ee6-103">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="75ee6-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="75ee6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75ee6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75ee6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75ee6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75ee6-106">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="75ee6-106">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75ee6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75ee6-107">Prerequisites</span></span>
<span data-ttu-id="75ee6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75ee6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75ee6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75ee6-110">Permission type</span></span>|<span data-ttu-id="75ee6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75ee6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75ee6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75ee6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75ee6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75ee6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75ee6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75ee6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75ee6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75ee6-115">Not supported.</span></span>|
|<span data-ttu-id="75ee6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75ee6-116">Application</span></span>|<span data-ttu-id="75ee6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75ee6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75ee6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75ee6-118">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="75ee6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75ee6-119">Request headers</span></span>
|<span data-ttu-id="75ee6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75ee6-120">Header</span></span>|<span data-ttu-id="75ee6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="75ee6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75ee6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75ee6-122">Authorization</span></span>|<span data-ttu-id="75ee6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75ee6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75ee6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="75ee6-124">Accept</span></span>|<span data-ttu-id="75ee6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75ee6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75ee6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75ee6-126">Request body</span></span>
<span data-ttu-id="75ee6-127">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75ee6-127">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="75ee6-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="75ee6-128">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="75ee6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="75ee6-129">Property</span></span>|<span data-ttu-id="75ee6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="75ee6-130">Type</span></span>|<span data-ttu-id="75ee6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="75ee6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75ee6-132">id</span><span class="sxs-lookup"><span data-stu-id="75ee6-132">id</span></span>|<span data-ttu-id="75ee6-133">String</span><span class="sxs-lookup"><span data-stu-id="75ee6-133">String</span></span>|<span data-ttu-id="75ee6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="75ee6-134">Key of the entity.</span></span>|
|<span data-ttu-id="75ee6-135">settingName</span><span class="sxs-lookup"><span data-stu-id="75ee6-135">settingName</span></span>|<span data-ttu-id="75ee6-136">String</span><span class="sxs-lookup"><span data-stu-id="75ee6-136">String</span></span>|<span data-ttu-id="75ee6-137">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="75ee6-137">Name of the setting</span></span>|
|<span data-ttu-id="75ee6-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="75ee6-138">instancePath</span></span>|<span data-ttu-id="75ee6-139">String</span><span class="sxs-lookup"><span data-stu-id="75ee6-139">String</span></span>|<span data-ttu-id="75ee6-140">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="75ee6-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="75ee6-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75ee6-141">unknownDeviceCount</span></span>|<span data-ttu-id="75ee6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="75ee6-142">Int32</span></span>|<span data-ttu-id="75ee6-143">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="75ee6-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="75ee6-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75ee6-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="75ee6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="75ee6-145">Int32</span></span>|<span data-ttu-id="75ee6-146">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="75ee6-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="75ee6-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75ee6-147">compliantDeviceCount</span></span>|<span data-ttu-id="75ee6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="75ee6-148">Int32</span></span>|<span data-ttu-id="75ee6-149">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="75ee6-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="75ee6-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75ee6-150">remediatedDeviceCount</span></span>|<span data-ttu-id="75ee6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="75ee6-151">Int32</span></span>|<span data-ttu-id="75ee6-152">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="75ee6-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="75ee6-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75ee6-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="75ee6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="75ee6-154">Int32</span></span>|<span data-ttu-id="75ee6-155">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="75ee6-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="75ee6-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75ee6-156">errorDeviceCount</span></span>|<span data-ttu-id="75ee6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="75ee6-157">Int32</span></span>|<span data-ttu-id="75ee6-158">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="75ee6-158">Device error count for the setting</span></span>|
|<span data-ttu-id="75ee6-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75ee6-159">conflictDeviceCount</span></span>|<span data-ttu-id="75ee6-160">Int32</span><span class="sxs-lookup"><span data-stu-id="75ee6-160">Int32</span></span>|<span data-ttu-id="75ee6-161">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="75ee6-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="75ee6-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="75ee6-162">Response</span></span>
<span data-ttu-id="75ee6-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="75ee6-163">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75ee6-164">Пример</span><span class="sxs-lookup"><span data-stu-id="75ee6-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="75ee6-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="75ee6-165">Request</span></span>
<span data-ttu-id="75ee6-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75ee6-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75ee6-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="75ee6-167">Response</span></span>
<span data-ttu-id="75ee6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75ee6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




