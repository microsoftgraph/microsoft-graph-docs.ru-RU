---
title: Create settingStateDeviceSummary
description: Создание объекта settingStateDeviceSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 723ad2be57443411eacbc762f6b97c12576e09ed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514293"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="86c17-103">Create settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="86c17-103">Create settingStateDeviceSummary</span></span>

<span data-ttu-id="86c17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86c17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86c17-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86c17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86c17-106">Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="86c17-106">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86c17-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="86c17-107">Prerequisites</span></span>
<span data-ttu-id="86c17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86c17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86c17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86c17-110">Permission type</span></span>|<span data-ttu-id="86c17-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86c17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86c17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86c17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86c17-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c17-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86c17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86c17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86c17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86c17-115">Not supported.</span></span>|
|<span data-ttu-id="86c17-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86c17-116">Application</span></span>|<span data-ttu-id="86c17-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86c17-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86c17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86c17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="86c17-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86c17-119">Request headers</span></span>
|<span data-ttu-id="86c17-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86c17-120">Header</span></span>|<span data-ttu-id="86c17-121">Значение</span><span class="sxs-lookup"><span data-stu-id="86c17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86c17-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86c17-122">Authorization</span></span>|<span data-ttu-id="86c17-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86c17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86c17-124">Accept</span><span class="sxs-lookup"><span data-stu-id="86c17-124">Accept</span></span>|<span data-ttu-id="86c17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86c17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86c17-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86c17-126">Request body</span></span>
<span data-ttu-id="86c17-127">В теле запроса добавьте представление объекта settingStateDeviceSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86c17-127">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="86c17-128">Ниже показаны свойства, которые необходимо указывать при создании объекта settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="86c17-128">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="86c17-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="86c17-129">Property</span></span>|<span data-ttu-id="86c17-130">Тип</span><span class="sxs-lookup"><span data-stu-id="86c17-130">Type</span></span>|<span data-ttu-id="86c17-131">Описание</span><span class="sxs-lookup"><span data-stu-id="86c17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86c17-132">id</span><span class="sxs-lookup"><span data-stu-id="86c17-132">id</span></span>|<span data-ttu-id="86c17-133">Строка</span><span class="sxs-lookup"><span data-stu-id="86c17-133">String</span></span>|<span data-ttu-id="86c17-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="86c17-134">Key of the entity.</span></span>|
|<span data-ttu-id="86c17-135">settingName</span><span class="sxs-lookup"><span data-stu-id="86c17-135">settingName</span></span>|<span data-ttu-id="86c17-136">Строка</span><span class="sxs-lookup"><span data-stu-id="86c17-136">String</span></span>|<span data-ttu-id="86c17-137">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="86c17-137">Name of the setting</span></span>|
|<span data-ttu-id="86c17-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="86c17-138">instancePath</span></span>|<span data-ttu-id="86c17-139">String</span><span class="sxs-lookup"><span data-stu-id="86c17-139">String</span></span>|<span data-ttu-id="86c17-140">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="86c17-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="86c17-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86c17-141">unknownDeviceCount</span></span>|<span data-ttu-id="86c17-142">Int32</span><span class="sxs-lookup"><span data-stu-id="86c17-142">Int32</span></span>|<span data-ttu-id="86c17-143">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="86c17-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="86c17-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86c17-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="86c17-145">Int32</span><span class="sxs-lookup"><span data-stu-id="86c17-145">Int32</span></span>|<span data-ttu-id="86c17-146">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="86c17-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="86c17-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86c17-147">compliantDeviceCount</span></span>|<span data-ttu-id="86c17-148">Int32</span><span class="sxs-lookup"><span data-stu-id="86c17-148">Int32</span></span>|<span data-ttu-id="86c17-149">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="86c17-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="86c17-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86c17-150">remediatedDeviceCount</span></span>|<span data-ttu-id="86c17-151">Int32</span><span class="sxs-lookup"><span data-stu-id="86c17-151">Int32</span></span>|<span data-ttu-id="86c17-152">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="86c17-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="86c17-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86c17-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="86c17-154">Int32</span><span class="sxs-lookup"><span data-stu-id="86c17-154">Int32</span></span>|<span data-ttu-id="86c17-155">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="86c17-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="86c17-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86c17-156">errorDeviceCount</span></span>|<span data-ttu-id="86c17-157">Int32</span><span class="sxs-lookup"><span data-stu-id="86c17-157">Int32</span></span>|<span data-ttu-id="86c17-158">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="86c17-158">Device error count for the setting</span></span>|
|<span data-ttu-id="86c17-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86c17-159">conflictDeviceCount</span></span>|<span data-ttu-id="86c17-160">Int32</span><span class="sxs-lookup"><span data-stu-id="86c17-160">Int32</span></span>|<span data-ttu-id="86c17-161">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="86c17-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="86c17-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="86c17-162">Response</span></span>
<span data-ttu-id="86c17-163">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="86c17-163">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c17-164">Пример</span><span class="sxs-lookup"><span data-stu-id="86c17-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="86c17-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="86c17-165">Request</span></span>
<span data-ttu-id="86c17-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86c17-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="86c17-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="86c17-167">Response</span></span>
<span data-ttu-id="86c17-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86c17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




