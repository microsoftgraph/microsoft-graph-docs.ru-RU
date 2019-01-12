---
title: Обновление объекта settingStateDeviceSummary
description: Обновление свойств объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ab0a3ec4609ce3f5015d9bb1ae6f1b815f5d6b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920599"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="e1859-103">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e1859-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="e1859-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1859-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1859-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1859-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1859-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e1859-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1859-107">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e1859-107">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1859-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e1859-108">Prerequisites</span></span>
<span data-ttu-id="e1859-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1859-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1859-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1859-111">Permission type</span></span>|<span data-ttu-id="e1859-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1859-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1859-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1859-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1859-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1859-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1859-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1859-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1859-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1859-116">Not supported.</span></span>|
|<span data-ttu-id="e1859-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1859-117">Application</span></span>|<span data-ttu-id="e1859-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1859-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1859-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1859-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e1859-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1859-120">Request headers</span></span>
|<span data-ttu-id="e1859-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1859-121">Header</span></span>|<span data-ttu-id="e1859-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1859-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1859-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1859-123">Authorization</span></span>|<span data-ttu-id="e1859-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e1859-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1859-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1859-125">Accept</span></span>|<span data-ttu-id="e1859-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1859-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1859-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1859-127">Request body</span></span>
<span data-ttu-id="e1859-128">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1859-128">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="e1859-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e1859-129">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="e1859-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1859-130">Property</span></span>|<span data-ttu-id="e1859-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e1859-131">Type</span></span>|<span data-ttu-id="e1859-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e1859-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1859-133">id</span><span class="sxs-lookup"><span data-stu-id="e1859-133">id</span></span>|<span data-ttu-id="e1859-134">String</span><span class="sxs-lookup"><span data-stu-id="e1859-134">String</span></span>|<span data-ttu-id="e1859-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e1859-135">Key of the entity.</span></span>|
|<span data-ttu-id="e1859-136">settingName</span><span class="sxs-lookup"><span data-stu-id="e1859-136">settingName</span></span>|<span data-ttu-id="e1859-137">String</span><span class="sxs-lookup"><span data-stu-id="e1859-137">String</span></span>|<span data-ttu-id="e1859-138">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="e1859-138">Name of the setting</span></span>|
|<span data-ttu-id="e1859-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="e1859-139">instancePath</span></span>|<span data-ttu-id="e1859-140">String</span><span class="sxs-lookup"><span data-stu-id="e1859-140">String</span></span>|<span data-ttu-id="e1859-141">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="e1859-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="e1859-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1859-142">unknownDeviceCount</span></span>|<span data-ttu-id="e1859-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e1859-143">Int32</span></span>|<span data-ttu-id="e1859-144">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="e1859-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="e1859-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1859-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="e1859-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e1859-146">Int32</span></span>|<span data-ttu-id="e1859-147">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="e1859-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="e1859-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1859-148">compliantDeviceCount</span></span>|<span data-ttu-id="e1859-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e1859-149">Int32</span></span>|<span data-ttu-id="e1859-150">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="e1859-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="e1859-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1859-151">remediatedDeviceCount</span></span>|<span data-ttu-id="e1859-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e1859-152">Int32</span></span>|<span data-ttu-id="e1859-153">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="e1859-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="e1859-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1859-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e1859-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e1859-155">Int32</span></span>|<span data-ttu-id="e1859-156">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="e1859-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="e1859-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1859-157">errorDeviceCount</span></span>|<span data-ttu-id="e1859-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e1859-158">Int32</span></span>|<span data-ttu-id="e1859-159">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="e1859-159">Device error count for the setting</span></span>|
|<span data-ttu-id="e1859-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1859-160">conflictDeviceCount</span></span>|<span data-ttu-id="e1859-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e1859-161">Int32</span></span>|<span data-ttu-id="e1859-162">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="e1859-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="e1859-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1859-163">Response</span></span>
<span data-ttu-id="e1859-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1859-164">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1859-165">Пример</span><span class="sxs-lookup"><span data-stu-id="e1859-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1859-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1859-166">Request</span></span>
<span data-ttu-id="e1859-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1859-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 296

{
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

### <a name="response"></a><span data-ttu-id="e1859-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1859-168">Response</span></span>
<span data-ttu-id="e1859-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e1859-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





