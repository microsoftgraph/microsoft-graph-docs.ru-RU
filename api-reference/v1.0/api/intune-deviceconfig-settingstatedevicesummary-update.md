---
title: Обновление объекта settingStateDeviceSummary
description: Обновление свойств объекта settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81331f767403b40ebe07ad0676a568f82a844384
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089163"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="cf206-103">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cf206-103">Update settingStateDeviceSummary</span></span>

<span data-ttu-id="cf206-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf206-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf206-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf206-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf206-106">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="cf206-106">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf206-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cf206-107">Prerequisites</span></span>
<span data-ttu-id="cf206-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf206-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf206-110">Permission type</span></span>|<span data-ttu-id="cf206-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf206-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf206-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf206-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf206-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf206-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf206-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf206-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf206-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf206-115">Not supported.</span></span>|
|<span data-ttu-id="cf206-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf206-116">Application</span></span>|<span data-ttu-id="cf206-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf206-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf206-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf206-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="cf206-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf206-119">Request headers</span></span>
|<span data-ttu-id="cf206-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf206-120">Header</span></span>|<span data-ttu-id="cf206-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cf206-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf206-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf206-122">Authorization</span></span>|<span data-ttu-id="cf206-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf206-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf206-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cf206-124">Accept</span></span>|<span data-ttu-id="cf206-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf206-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf206-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf206-126">Request body</span></span>
<span data-ttu-id="cf206-127">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf206-127">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="cf206-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="cf206-128">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="cf206-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf206-129">Property</span></span>|<span data-ttu-id="cf206-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cf206-130">Type</span></span>|<span data-ttu-id="cf206-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cf206-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf206-132">id</span><span class="sxs-lookup"><span data-stu-id="cf206-132">id</span></span>|<span data-ttu-id="cf206-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cf206-133">String</span></span>|<span data-ttu-id="cf206-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cf206-134">Key of the entity.</span></span>|
|<span data-ttu-id="cf206-135">settingName</span><span class="sxs-lookup"><span data-stu-id="cf206-135">settingName</span></span>|<span data-ttu-id="cf206-136">String</span><span class="sxs-lookup"><span data-stu-id="cf206-136">String</span></span>|<span data-ttu-id="cf206-137">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="cf206-137">Name of the setting</span></span>|
|<span data-ttu-id="cf206-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="cf206-138">instancePath</span></span>|<span data-ttu-id="cf206-139">String</span><span class="sxs-lookup"><span data-stu-id="cf206-139">String</span></span>|<span data-ttu-id="cf206-140">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="cf206-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="cf206-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf206-141">unknownDeviceCount</span></span>|<span data-ttu-id="cf206-142">Int32</span><span class="sxs-lookup"><span data-stu-id="cf206-142">Int32</span></span>|<span data-ttu-id="cf206-143">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="cf206-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="cf206-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf206-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="cf206-145">Int32</span><span class="sxs-lookup"><span data-stu-id="cf206-145">Int32</span></span>|<span data-ttu-id="cf206-146">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="cf206-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="cf206-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf206-147">compliantDeviceCount</span></span>|<span data-ttu-id="cf206-148">Int32</span><span class="sxs-lookup"><span data-stu-id="cf206-148">Int32</span></span>|<span data-ttu-id="cf206-149">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="cf206-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="cf206-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf206-150">remediatedDeviceCount</span></span>|<span data-ttu-id="cf206-151">Int32</span><span class="sxs-lookup"><span data-stu-id="cf206-151">Int32</span></span>|<span data-ttu-id="cf206-152">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="cf206-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="cf206-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf206-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="cf206-154">Int32</span><span class="sxs-lookup"><span data-stu-id="cf206-154">Int32</span></span>|<span data-ttu-id="cf206-155">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="cf206-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="cf206-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf206-156">errorDeviceCount</span></span>|<span data-ttu-id="cf206-157">Int32</span><span class="sxs-lookup"><span data-stu-id="cf206-157">Int32</span></span>|<span data-ttu-id="cf206-158">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="cf206-158">Device error count for the setting</span></span>|
|<span data-ttu-id="cf206-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf206-159">conflictDeviceCount</span></span>|<span data-ttu-id="cf206-160">Int32</span><span class="sxs-lookup"><span data-stu-id="cf206-160">Int32</span></span>|<span data-ttu-id="cf206-161">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="cf206-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="cf206-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf206-162">Response</span></span>
<span data-ttu-id="cf206-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cf206-163">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf206-164">Пример</span><span class="sxs-lookup"><span data-stu-id="cf206-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf206-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf206-165">Request</span></span>
<span data-ttu-id="cf206-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf206-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
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

### <a name="response"></a><span data-ttu-id="cf206-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf206-167">Response</span></span>
<span data-ttu-id="cf206-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf206-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









