---
title: Create settingStateDeviceSummary
description: Создание объекта settingStateDeviceSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5393bc76fe9d4a6b546ff182191993e43d1a3d63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398851"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="f04fe-103">Create settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f04fe-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="f04fe-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f04fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f04fe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f04fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f04fe-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f04fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f04fe-107">Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f04fe-107">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f04fe-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f04fe-108">Prerequisites</span></span>
<span data-ttu-id="f04fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f04fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f04fe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f04fe-111">Permission type</span></span>|<span data-ttu-id="f04fe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f04fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f04fe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f04fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f04fe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f04fe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f04fe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f04fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f04fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f04fe-116">Not supported.</span></span>|
|<span data-ttu-id="f04fe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f04fe-117">Application</span></span>|<span data-ttu-id="f04fe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f04fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f04fe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f04fe-119">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f04fe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f04fe-120">Request headers</span></span>
|<span data-ttu-id="f04fe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f04fe-121">Header</span></span>|<span data-ttu-id="f04fe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f04fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f04fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f04fe-123">Authorization</span></span>|<span data-ttu-id="f04fe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f04fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f04fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f04fe-125">Accept</span></span>|<span data-ttu-id="f04fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f04fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f04fe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f04fe-127">Request body</span></span>
<span data-ttu-id="f04fe-128">В теле запроса добавьте представление объекта settingStateDeviceSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f04fe-128">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="f04fe-129">Ниже показаны свойства, которые необходимо указывать при создании объекта settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="f04fe-129">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="f04fe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f04fe-130">Property</span></span>|<span data-ttu-id="f04fe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f04fe-131">Type</span></span>|<span data-ttu-id="f04fe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f04fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f04fe-133">id</span><span class="sxs-lookup"><span data-stu-id="f04fe-133">id</span></span>|<span data-ttu-id="f04fe-134">String</span><span class="sxs-lookup"><span data-stu-id="f04fe-134">String</span></span>|<span data-ttu-id="f04fe-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f04fe-135">Key of the entity.</span></span>|
|<span data-ttu-id="f04fe-136">settingName</span><span class="sxs-lookup"><span data-stu-id="f04fe-136">settingName</span></span>|<span data-ttu-id="f04fe-137">String</span><span class="sxs-lookup"><span data-stu-id="f04fe-137">String</span></span>|<span data-ttu-id="f04fe-138">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="f04fe-138">Name of the setting</span></span>|
|<span data-ttu-id="f04fe-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="f04fe-139">instancePath</span></span>|<span data-ttu-id="f04fe-140">String</span><span class="sxs-lookup"><span data-stu-id="f04fe-140">String</span></span>|<span data-ttu-id="f04fe-141">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="f04fe-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="f04fe-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f04fe-142">unknownDeviceCount</span></span>|<span data-ttu-id="f04fe-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fe-143">Int32</span></span>|<span data-ttu-id="f04fe-144">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="f04fe-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="f04fe-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f04fe-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="f04fe-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fe-146">Int32</span></span>|<span data-ttu-id="f04fe-147">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="f04fe-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="f04fe-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f04fe-148">compliantDeviceCount</span></span>|<span data-ttu-id="f04fe-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fe-149">Int32</span></span>|<span data-ttu-id="f04fe-150">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="f04fe-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="f04fe-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f04fe-151">remediatedDeviceCount</span></span>|<span data-ttu-id="f04fe-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fe-152">Int32</span></span>|<span data-ttu-id="f04fe-153">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="f04fe-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="f04fe-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f04fe-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f04fe-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fe-155">Int32</span></span>|<span data-ttu-id="f04fe-156">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="f04fe-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="f04fe-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f04fe-157">errorDeviceCount</span></span>|<span data-ttu-id="f04fe-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fe-158">Int32</span></span>|<span data-ttu-id="f04fe-159">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="f04fe-159">Device error count for the setting</span></span>|
|<span data-ttu-id="f04fe-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f04fe-160">conflictDeviceCount</span></span>|<span data-ttu-id="f04fe-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fe-161">Int32</span></span>|<span data-ttu-id="f04fe-162">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="f04fe-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="f04fe-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="f04fe-163">Response</span></span>
<span data-ttu-id="f04fe-164">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f04fe-164">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f04fe-165">Пример</span><span class="sxs-lookup"><span data-stu-id="f04fe-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="f04fe-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="f04fe-166">Request</span></span>
<span data-ttu-id="f04fe-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f04fe-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f04fe-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="f04fe-168">Response</span></span>
<span data-ttu-id="f04fe-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f04fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




