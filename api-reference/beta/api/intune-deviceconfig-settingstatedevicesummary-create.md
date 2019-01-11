---
title: Create settingStateDeviceSummary
description: Создание объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 06c9851a534f59be935791e1c1f435d2180bf9d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852110"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="6e39a-103">Create settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6e39a-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="6e39a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e39a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e39a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e39a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e39a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6e39a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e39a-107">Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6e39a-107">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6e39a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6e39a-108">Prerequisites</span></span>
<span data-ttu-id="6e39a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e39a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e39a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e39a-111">Permission type</span></span>|<span data-ttu-id="6e39a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e39a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e39a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e39a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e39a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e39a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e39a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e39a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e39a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e39a-116">Not supported.</span></span>|
|<span data-ttu-id="6e39a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e39a-117">Application</span></span>|<span data-ttu-id="6e39a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e39a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e39a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e39a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6e39a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e39a-120">Request headers</span></span>
|<span data-ttu-id="6e39a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e39a-121">Header</span></span>|<span data-ttu-id="6e39a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6e39a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e39a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e39a-123">Authorization</span></span>|<span data-ttu-id="6e39a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6e39a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e39a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e39a-125">Accept</span></span>|<span data-ttu-id="6e39a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e39a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e39a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6e39a-127">Request body</span></span>
<span data-ttu-id="6e39a-128">В теле запроса добавьте представление объекта settingStateDeviceSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e39a-128">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="6e39a-129">Ниже показаны свойства, которые необходимо указывать при создании объекта settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="6e39a-129">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="6e39a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e39a-130">Property</span></span>|<span data-ttu-id="6e39a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6e39a-131">Type</span></span>|<span data-ttu-id="6e39a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6e39a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e39a-133">id</span><span class="sxs-lookup"><span data-stu-id="6e39a-133">id</span></span>|<span data-ttu-id="6e39a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6e39a-134">String</span></span>|<span data-ttu-id="6e39a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6e39a-135">Key of the entity.</span></span>|
|<span data-ttu-id="6e39a-136">settingName</span><span class="sxs-lookup"><span data-stu-id="6e39a-136">settingName</span></span>|<span data-ttu-id="6e39a-137">String</span><span class="sxs-lookup"><span data-stu-id="6e39a-137">String</span></span>|<span data-ttu-id="6e39a-138">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="6e39a-138">Name of the setting</span></span>|
|<span data-ttu-id="6e39a-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="6e39a-139">instancePath</span></span>|<span data-ttu-id="6e39a-140">String</span><span class="sxs-lookup"><span data-stu-id="6e39a-140">String</span></span>|<span data-ttu-id="6e39a-141">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="6e39a-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="6e39a-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e39a-142">unknownDeviceCount</span></span>|<span data-ttu-id="6e39a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6e39a-143">Int32</span></span>|<span data-ttu-id="6e39a-144">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6e39a-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="6e39a-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e39a-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="6e39a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6e39a-146">Int32</span></span>|<span data-ttu-id="6e39a-147">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6e39a-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="6e39a-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e39a-148">compliantDeviceCount</span></span>|<span data-ttu-id="6e39a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6e39a-149">Int32</span></span>|<span data-ttu-id="6e39a-150">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6e39a-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6e39a-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e39a-151">remediatedDeviceCount</span></span>|<span data-ttu-id="6e39a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6e39a-152">Int32</span></span>|<span data-ttu-id="6e39a-153">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6e39a-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6e39a-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e39a-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6e39a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6e39a-155">Int32</span></span>|<span data-ttu-id="6e39a-156">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6e39a-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="6e39a-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e39a-157">errorDeviceCount</span></span>|<span data-ttu-id="6e39a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6e39a-158">Int32</span></span>|<span data-ttu-id="6e39a-159">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6e39a-159">Device error count for the setting</span></span>|
|<span data-ttu-id="6e39a-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6e39a-160">conflictDeviceCount</span></span>|<span data-ttu-id="6e39a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="6e39a-161">Int32</span></span>|<span data-ttu-id="6e39a-162">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6e39a-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="6e39a-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e39a-163">Response</span></span>
<span data-ttu-id="6e39a-164">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6e39a-164">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e39a-165">Пример</span><span class="sxs-lookup"><span data-stu-id="6e39a-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e39a-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e39a-166">Request</span></span>
<span data-ttu-id="6e39a-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e39a-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e39a-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e39a-168">Response</span></span>
<span data-ttu-id="6e39a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6e39a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





