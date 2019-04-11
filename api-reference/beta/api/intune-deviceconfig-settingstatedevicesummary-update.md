---
title: Обновление объекта settingStateDeviceSummary
description: Обновление свойств объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae2edd382d6f9930163fc5d31b32e4a7a18389c7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776992"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="85705-103">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="85705-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="85705-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85705-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85705-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85705-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85705-106">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="85705-106">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85705-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="85705-107">Prerequisites</span></span>
<span data-ttu-id="85705-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85705-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85705-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85705-110">Permission type</span></span>|<span data-ttu-id="85705-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85705-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85705-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85705-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85705-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85705-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85705-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85705-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85705-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85705-115">Not supported.</span></span>|
|<span data-ttu-id="85705-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85705-116">Application</span></span>|<span data-ttu-id="85705-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85705-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85705-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85705-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="85705-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85705-119">Request headers</span></span>
|<span data-ttu-id="85705-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85705-120">Header</span></span>|<span data-ttu-id="85705-121">Значение</span><span class="sxs-lookup"><span data-stu-id="85705-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85705-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85705-122">Authorization</span></span>|<span data-ttu-id="85705-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85705-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85705-124">Accept</span><span class="sxs-lookup"><span data-stu-id="85705-124">Accept</span></span>|<span data-ttu-id="85705-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85705-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85705-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85705-126">Request body</span></span>
<span data-ttu-id="85705-127">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85705-127">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="85705-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="85705-128">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="85705-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="85705-129">Property</span></span>|<span data-ttu-id="85705-130">Тип</span><span class="sxs-lookup"><span data-stu-id="85705-130">Type</span></span>|<span data-ttu-id="85705-131">Описание</span><span class="sxs-lookup"><span data-stu-id="85705-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85705-132">id</span><span class="sxs-lookup"><span data-stu-id="85705-132">id</span></span>|<span data-ttu-id="85705-133">String</span><span class="sxs-lookup"><span data-stu-id="85705-133">String</span></span>|<span data-ttu-id="85705-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="85705-134">Key of the entity.</span></span>|
|<span data-ttu-id="85705-135">settingName</span><span class="sxs-lookup"><span data-stu-id="85705-135">settingName</span></span>|<span data-ttu-id="85705-136">String</span><span class="sxs-lookup"><span data-stu-id="85705-136">String</span></span>|<span data-ttu-id="85705-137">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="85705-137">Name of the setting</span></span>|
|<span data-ttu-id="85705-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="85705-138">instancePath</span></span>|<span data-ttu-id="85705-139">String</span><span class="sxs-lookup"><span data-stu-id="85705-139">String</span></span>|<span data-ttu-id="85705-140">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="85705-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="85705-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85705-141">unknownDeviceCount</span></span>|<span data-ttu-id="85705-142">Int32</span><span class="sxs-lookup"><span data-stu-id="85705-142">Int32</span></span>|<span data-ttu-id="85705-143">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="85705-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="85705-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85705-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="85705-145">Int32</span><span class="sxs-lookup"><span data-stu-id="85705-145">Int32</span></span>|<span data-ttu-id="85705-146">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="85705-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="85705-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85705-147">compliantDeviceCount</span></span>|<span data-ttu-id="85705-148">Int32</span><span class="sxs-lookup"><span data-stu-id="85705-148">Int32</span></span>|<span data-ttu-id="85705-149">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="85705-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="85705-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85705-150">remediatedDeviceCount</span></span>|<span data-ttu-id="85705-151">Int32</span><span class="sxs-lookup"><span data-stu-id="85705-151">Int32</span></span>|<span data-ttu-id="85705-152">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="85705-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="85705-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85705-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="85705-154">Int32</span><span class="sxs-lookup"><span data-stu-id="85705-154">Int32</span></span>|<span data-ttu-id="85705-155">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="85705-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="85705-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85705-156">errorDeviceCount</span></span>|<span data-ttu-id="85705-157">Int32</span><span class="sxs-lookup"><span data-stu-id="85705-157">Int32</span></span>|<span data-ttu-id="85705-158">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="85705-158">Device error count for the setting</span></span>|
|<span data-ttu-id="85705-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85705-159">conflictDeviceCount</span></span>|<span data-ttu-id="85705-160">Int32</span><span class="sxs-lookup"><span data-stu-id="85705-160">Int32</span></span>|<span data-ttu-id="85705-161">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="85705-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="85705-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="85705-162">Response</span></span>
<span data-ttu-id="85705-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85705-163">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85705-164">Пример</span><span class="sxs-lookup"><span data-stu-id="85705-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="85705-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="85705-165">Request</span></span>
<span data-ttu-id="85705-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85705-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85705-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="85705-167">Response</span></span>
<span data-ttu-id="85705-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85705-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





