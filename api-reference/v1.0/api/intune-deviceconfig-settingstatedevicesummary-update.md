---
title: Обновление объекта settingStateDeviceSummary
description: Обновление свойств объекта settingStateDeviceSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5dd5d497d73e1ada42512acf520ec5c03cf30192
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365798"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="8377f-103">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8377f-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="8377f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8377f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8377f-105">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8377f-105">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8377f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8377f-106">Prerequisites</span></span>
<span data-ttu-id="8377f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8377f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8377f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8377f-109">Permission type</span></span>|<span data-ttu-id="8377f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8377f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8377f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8377f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8377f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8377f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8377f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8377f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8377f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8377f-114">Not supported.</span></span>|
|<span data-ttu-id="8377f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8377f-115">Application</span></span>|<span data-ttu-id="8377f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8377f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8377f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8377f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="8377f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8377f-118">Request headers</span></span>
|<span data-ttu-id="8377f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8377f-119">Header</span></span>|<span data-ttu-id="8377f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8377f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8377f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8377f-121">Authorization</span></span>|<span data-ttu-id="8377f-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8377f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8377f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8377f-123">Accept</span></span>|<span data-ttu-id="8377f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8377f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8377f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8377f-125">Request body</span></span>
<span data-ttu-id="8377f-126">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8377f-126">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="8377f-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8377f-127">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="8377f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8377f-128">Property</span></span>|<span data-ttu-id="8377f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8377f-129">Type</span></span>|<span data-ttu-id="8377f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8377f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8377f-131">id</span><span class="sxs-lookup"><span data-stu-id="8377f-131">id</span></span>|<span data-ttu-id="8377f-132">String</span><span class="sxs-lookup"><span data-stu-id="8377f-132">String</span></span>|<span data-ttu-id="8377f-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8377f-133">Key of the entity.</span></span>|
|<span data-ttu-id="8377f-134">settingName</span><span class="sxs-lookup"><span data-stu-id="8377f-134">settingName</span></span>|<span data-ttu-id="8377f-135">String</span><span class="sxs-lookup"><span data-stu-id="8377f-135">String</span></span>|<span data-ttu-id="8377f-136">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="8377f-136">Name of the setting</span></span>|
|<span data-ttu-id="8377f-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="8377f-137">instancePath</span></span>|<span data-ttu-id="8377f-138">String</span><span class="sxs-lookup"><span data-stu-id="8377f-138">String</span></span>|<span data-ttu-id="8377f-139">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="8377f-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="8377f-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8377f-140">unknownDeviceCount</span></span>|<span data-ttu-id="8377f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="8377f-141">Int32</span></span>|<span data-ttu-id="8377f-142">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="8377f-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="8377f-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8377f-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="8377f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8377f-144">Int32</span></span>|<span data-ttu-id="8377f-145">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="8377f-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="8377f-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8377f-146">compliantDeviceCount</span></span>|<span data-ttu-id="8377f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8377f-147">Int32</span></span>|<span data-ttu-id="8377f-148">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="8377f-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="8377f-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8377f-149">remediatedDeviceCount</span></span>|<span data-ttu-id="8377f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8377f-150">Int32</span></span>|<span data-ttu-id="8377f-151">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="8377f-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="8377f-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8377f-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8377f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8377f-153">Int32</span></span>|<span data-ttu-id="8377f-154">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="8377f-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="8377f-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8377f-155">errorDeviceCount</span></span>|<span data-ttu-id="8377f-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8377f-156">Int32</span></span>|<span data-ttu-id="8377f-157">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="8377f-157">Device error count for the setting</span></span>|
|<span data-ttu-id="8377f-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8377f-158">conflictDeviceCount</span></span>|<span data-ttu-id="8377f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8377f-159">Int32</span></span>|<span data-ttu-id="8377f-160">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="8377f-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="8377f-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8377f-161">Response</span></span>
<span data-ttu-id="8377f-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8377f-162">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8377f-163">Пример</span><span class="sxs-lookup"><span data-stu-id="8377f-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="8377f-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="8377f-164">Request</span></span>
<span data-ttu-id="8377f-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8377f-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8377f-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="8377f-166">Response</span></span>
<span data-ttu-id="8377f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8377f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




