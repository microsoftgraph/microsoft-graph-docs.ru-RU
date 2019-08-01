---
title: Create settingStateDeviceSummary
description: Создание объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f8cdf18006611634e019d7275dafbeea8d302ca3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017086"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="69ed9-103">Create settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="69ed9-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="69ed9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69ed9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69ed9-105">Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="69ed9-105">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69ed9-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="69ed9-106">Prerequisites</span></span>
<span data-ttu-id="69ed9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69ed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ed9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69ed9-109">Permission type</span></span>|<span data-ttu-id="69ed9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69ed9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69ed9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69ed9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69ed9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ed9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69ed9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69ed9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69ed9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69ed9-114">Not supported.</span></span>|
|<span data-ttu-id="69ed9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69ed9-115">Application</span></span>|<span data-ttu-id="69ed9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69ed9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69ed9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69ed9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="69ed9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69ed9-118">Request headers</span></span>
|<span data-ttu-id="69ed9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69ed9-119">Header</span></span>|<span data-ttu-id="69ed9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="69ed9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69ed9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69ed9-121">Authorization</span></span>|<span data-ttu-id="69ed9-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69ed9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69ed9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="69ed9-123">Accept</span></span>|<span data-ttu-id="69ed9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="69ed9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ed9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69ed9-125">Request body</span></span>
<span data-ttu-id="69ed9-126">В теле запроса добавьте представление объекта settingStateDeviceSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69ed9-126">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="69ed9-127">Ниже показаны свойства, которые необходимо указывать при создании объекта settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="69ed9-127">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="69ed9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="69ed9-128">Property</span></span>|<span data-ttu-id="69ed9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="69ed9-129">Type</span></span>|<span data-ttu-id="69ed9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="69ed9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69ed9-131">id</span><span class="sxs-lookup"><span data-stu-id="69ed9-131">id</span></span>|<span data-ttu-id="69ed9-132">String</span><span class="sxs-lookup"><span data-stu-id="69ed9-132">String</span></span>|<span data-ttu-id="69ed9-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="69ed9-133">Key of the entity.</span></span>|
|<span data-ttu-id="69ed9-134">settingName</span><span class="sxs-lookup"><span data-stu-id="69ed9-134">settingName</span></span>|<span data-ttu-id="69ed9-135">String</span><span class="sxs-lookup"><span data-stu-id="69ed9-135">String</span></span>|<span data-ttu-id="69ed9-136">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="69ed9-136">Name of the setting</span></span>|
|<span data-ttu-id="69ed9-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="69ed9-137">instancePath</span></span>|<span data-ttu-id="69ed9-138">String</span><span class="sxs-lookup"><span data-stu-id="69ed9-138">String</span></span>|<span data-ttu-id="69ed9-139">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="69ed9-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="69ed9-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69ed9-140">unknownDeviceCount</span></span>|<span data-ttu-id="69ed9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="69ed9-141">Int32</span></span>|<span data-ttu-id="69ed9-142">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="69ed9-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="69ed9-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69ed9-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="69ed9-144">Int32</span><span class="sxs-lookup"><span data-stu-id="69ed9-144">Int32</span></span>|<span data-ttu-id="69ed9-145">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="69ed9-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="69ed9-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69ed9-146">compliantDeviceCount</span></span>|<span data-ttu-id="69ed9-147">Int32</span><span class="sxs-lookup"><span data-stu-id="69ed9-147">Int32</span></span>|<span data-ttu-id="69ed9-148">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="69ed9-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="69ed9-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69ed9-149">remediatedDeviceCount</span></span>|<span data-ttu-id="69ed9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="69ed9-150">Int32</span></span>|<span data-ttu-id="69ed9-151">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="69ed9-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="69ed9-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69ed9-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="69ed9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="69ed9-153">Int32</span></span>|<span data-ttu-id="69ed9-154">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="69ed9-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="69ed9-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69ed9-155">errorDeviceCount</span></span>|<span data-ttu-id="69ed9-156">Int32</span><span class="sxs-lookup"><span data-stu-id="69ed9-156">Int32</span></span>|<span data-ttu-id="69ed9-157">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="69ed9-157">Device error count for the setting</span></span>|
|<span data-ttu-id="69ed9-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69ed9-158">conflictDeviceCount</span></span>|<span data-ttu-id="69ed9-159">Int32</span><span class="sxs-lookup"><span data-stu-id="69ed9-159">Int32</span></span>|<span data-ttu-id="69ed9-160">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="69ed9-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="69ed9-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="69ed9-161">Response</span></span>
<span data-ttu-id="69ed9-162">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="69ed9-162">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69ed9-163">Пример</span><span class="sxs-lookup"><span data-stu-id="69ed9-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="69ed9-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="69ed9-164">Request</span></span>
<span data-ttu-id="69ed9-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69ed9-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69ed9-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="69ed9-166">Response</span></span>
<span data-ttu-id="69ed9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69ed9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



