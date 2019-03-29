---
title: Обновление объекта settingStateDeviceSummary
description: Обновление свойств объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7adbba330453a0bcd308fe5aa5804c8a63dfc2ac
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961632"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="c1f5d-103">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="c1f5d-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="c1f5d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1f5d-105">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c1f5d-105">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1f5d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1f5d-106">Prerequisites</span></span>
<span data-ttu-id="c1f5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1f5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1f5d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1f5d-109">Permission type</span></span>|<span data-ttu-id="c1f5d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1f5d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1f5d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1f5d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1f5d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1f5d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1f5d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1f5d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1f5d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-114">Not supported.</span></span>|
|<span data-ttu-id="c1f5d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1f5d-115">Application</span></span>|<span data-ttu-id="c1f5d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1f5d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1f5d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="c1f5d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1f5d-118">Request headers</span></span>
|<span data-ttu-id="c1f5d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1f5d-119">Header</span></span>|<span data-ttu-id="c1f5d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c1f5d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1f5d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1f5d-121">Authorization</span></span>|<span data-ttu-id="c1f5d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1f5d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c1f5d-123">Accept</span></span>|<span data-ttu-id="c1f5d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c1f5d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1f5d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1f5d-125">Request body</span></span>
<span data-ttu-id="c1f5d-126">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-126">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="c1f5d-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c1f5d-127">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="c1f5d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1f5d-128">Property</span></span>|<span data-ttu-id="c1f5d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c1f5d-129">Type</span></span>|<span data-ttu-id="c1f5d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c1f5d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1f5d-131">id</span><span class="sxs-lookup"><span data-stu-id="c1f5d-131">id</span></span>|<span data-ttu-id="c1f5d-132">String</span><span class="sxs-lookup"><span data-stu-id="c1f5d-132">String</span></span>|<span data-ttu-id="c1f5d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-133">Key of the entity.</span></span>|
|<span data-ttu-id="c1f5d-134">settingName</span><span class="sxs-lookup"><span data-stu-id="c1f5d-134">settingName</span></span>|<span data-ttu-id="c1f5d-135">String</span><span class="sxs-lookup"><span data-stu-id="c1f5d-135">String</span></span>|<span data-ttu-id="c1f5d-136">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-136">Name of the setting</span></span>|
|<span data-ttu-id="c1f5d-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="c1f5d-137">instancePath</span></span>|<span data-ttu-id="c1f5d-138">String</span><span class="sxs-lookup"><span data-stu-id="c1f5d-138">String</span></span>|<span data-ttu-id="c1f5d-139">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="c1f5d-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1f5d-140">unknownDeviceCount</span></span>|<span data-ttu-id="c1f5d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c1f5d-141">Int32</span></span>|<span data-ttu-id="c1f5d-142">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="c1f5d-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1f5d-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="c1f5d-144">Int32</span><span class="sxs-lookup"><span data-stu-id="c1f5d-144">Int32</span></span>|<span data-ttu-id="c1f5d-145">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="c1f5d-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1f5d-146">compliantDeviceCount</span></span>|<span data-ttu-id="c1f5d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="c1f5d-147">Int32</span></span>|<span data-ttu-id="c1f5d-148">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="c1f5d-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1f5d-149">remediatedDeviceCount</span></span>|<span data-ttu-id="c1f5d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c1f5d-150">Int32</span></span>|<span data-ttu-id="c1f5d-151">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="c1f5d-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1f5d-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c1f5d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c1f5d-153">Int32</span></span>|<span data-ttu-id="c1f5d-154">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="c1f5d-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1f5d-155">errorDeviceCount</span></span>|<span data-ttu-id="c1f5d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c1f5d-156">Int32</span></span>|<span data-ttu-id="c1f5d-157">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-157">Device error count for the setting</span></span>|
|<span data-ttu-id="c1f5d-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1f5d-158">conflictDeviceCount</span></span>|<span data-ttu-id="c1f5d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="c1f5d-159">Int32</span></span>|<span data-ttu-id="c1f5d-160">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="c1f5d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1f5d-161">Response</span></span>
<span data-ttu-id="c1f5d-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-162">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1f5d-163">Пример</span><span class="sxs-lookup"><span data-stu-id="c1f5d-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1f5d-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1f5d-164">Request</span></span>
<span data-ttu-id="c1f5d-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1f5d-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1f5d-166">Response</span></span>
<span data-ttu-id="c1f5d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1f5d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



