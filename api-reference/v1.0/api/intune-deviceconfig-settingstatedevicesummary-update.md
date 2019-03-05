---
title: Обновление объекта settingStateDeviceSummary
description: Обновление свойств объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2419f6e743448c91ea3927d1bc9f7ca71ebc686d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258683"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="7e2e1-103">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="7e2e1-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="7e2e1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e2e1-105">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7e2e1-105">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e2e1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7e2e1-106">Prerequisites</span></span>
<span data-ttu-id="7e2e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e2e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7e2e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e2e1-109">Permission type</span></span>|<span data-ttu-id="7e2e1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e2e1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e2e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e2e1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7e2e1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2e1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7e2e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e2e1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e2e1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-114">Not supported.</span></span>|
|<span data-ttu-id="7e2e1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e2e1-115">Application</span></span>|<span data-ttu-id="7e2e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e2e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e2e1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7e2e1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e2e1-118">Request headers</span></span>
|<span data-ttu-id="7e2e1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e2e1-119">Header</span></span>|<span data-ttu-id="7e2e1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7e2e1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e2e1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e2e1-121">Authorization</span></span>|<span data-ttu-id="7e2e1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7e2e1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e2e1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7e2e1-123">Accept</span></span>|<span data-ttu-id="7e2e1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7e2e1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e2e1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e2e1-125">Request body</span></span>
<span data-ttu-id="7e2e1-126">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-126">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="7e2e1-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7e2e1-127">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="7e2e1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e2e1-128">Property</span></span>|<span data-ttu-id="7e2e1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7e2e1-129">Type</span></span>|<span data-ttu-id="7e2e1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7e2e1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e2e1-131">id</span><span class="sxs-lookup"><span data-stu-id="7e2e1-131">id</span></span>|<span data-ttu-id="7e2e1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="7e2e1-132">String</span></span>|<span data-ttu-id="7e2e1-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-133">Key of the entity.</span></span>|
|<span data-ttu-id="7e2e1-134">settingName</span><span class="sxs-lookup"><span data-stu-id="7e2e1-134">settingName</span></span>|<span data-ttu-id="7e2e1-135">String</span><span class="sxs-lookup"><span data-stu-id="7e2e1-135">String</span></span>|<span data-ttu-id="7e2e1-136">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-136">Name of the setting</span></span>|
|<span data-ttu-id="7e2e1-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="7e2e1-137">instancePath</span></span>|<span data-ttu-id="7e2e1-138">String</span><span class="sxs-lookup"><span data-stu-id="7e2e1-138">String</span></span>|<span data-ttu-id="7e2e1-139">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="7e2e1-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2e1-140">unknownDeviceCount</span></span>|<span data-ttu-id="7e2e1-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2e1-141">Int32</span></span>|<span data-ttu-id="7e2e1-142">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="7e2e1-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2e1-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="7e2e1-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2e1-144">Int32</span></span>|<span data-ttu-id="7e2e1-145">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="7e2e1-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2e1-146">compliantDeviceCount</span></span>|<span data-ttu-id="7e2e1-147">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2e1-147">Int32</span></span>|<span data-ttu-id="7e2e1-148">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="7e2e1-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2e1-149">remediatedDeviceCount</span></span>|<span data-ttu-id="7e2e1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2e1-150">Int32</span></span>|<span data-ttu-id="7e2e1-151">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="7e2e1-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2e1-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7e2e1-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2e1-153">Int32</span></span>|<span data-ttu-id="7e2e1-154">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="7e2e1-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2e1-155">errorDeviceCount</span></span>|<span data-ttu-id="7e2e1-156">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2e1-156">Int32</span></span>|<span data-ttu-id="7e2e1-157">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-157">Device error count for the setting</span></span>|
|<span data-ttu-id="7e2e1-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2e1-158">conflictDeviceCount</span></span>|<span data-ttu-id="7e2e1-159">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2e1-159">Int32</span></span>|<span data-ttu-id="7e2e1-160">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="7e2e1-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e2e1-161">Response</span></span>
<span data-ttu-id="7e2e1-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-162">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e2e1-163">Пример</span><span class="sxs-lookup"><span data-stu-id="7e2e1-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e2e1-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e2e1-164">Request</span></span>
<span data-ttu-id="7e2e1-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7e2e1-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e2e1-166">Response</span></span>
<span data-ttu-id="7e2e1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e2e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



