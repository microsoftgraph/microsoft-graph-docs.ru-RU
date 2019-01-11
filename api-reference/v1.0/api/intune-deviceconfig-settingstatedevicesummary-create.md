---
title: Create settingStateDeviceSummary
description: Создание объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2c6025a1ee8ff513b18d66d5b71f8c857bba9913
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867986"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="3a289-103">Create settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="3a289-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="3a289-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3a289-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a289-105">Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3a289-105">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a289-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3a289-106">Prerequisites</span></span>
<span data-ttu-id="3a289-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a289-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a289-109">Permission type</span></span>|<span data-ttu-id="3a289-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a289-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a289-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a289-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a289-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a289-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a289-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a289-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a289-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a289-114">Not supported.</span></span>|
|<span data-ttu-id="3a289-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a289-115">Application</span></span>|<span data-ttu-id="3a289-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a289-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a289-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a289-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="3a289-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a289-118">Request headers</span></span>
|<span data-ttu-id="3a289-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a289-119">Header</span></span>|<span data-ttu-id="3a289-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3a289-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a289-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a289-121">Authorization</span></span>|<span data-ttu-id="3a289-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3a289-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a289-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3a289-123">Accept</span></span>|<span data-ttu-id="3a289-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3a289-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a289-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a289-125">Request body</span></span>
<span data-ttu-id="3a289-126">В теле запроса добавьте представление объекта settingStateDeviceSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a289-126">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="3a289-127">Ниже показаны свойства, которые необходимо указывать при создании объекта settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="3a289-127">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="3a289-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a289-128">Property</span></span>|<span data-ttu-id="3a289-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3a289-129">Type</span></span>|<span data-ttu-id="3a289-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3a289-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a289-131">id</span><span class="sxs-lookup"><span data-stu-id="3a289-131">id</span></span>|<span data-ttu-id="3a289-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3a289-132">String</span></span>|<span data-ttu-id="3a289-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a289-133">Key of the entity.</span></span>|
|<span data-ttu-id="3a289-134">settingName</span><span class="sxs-lookup"><span data-stu-id="3a289-134">settingName</span></span>|<span data-ttu-id="3a289-135">String</span><span class="sxs-lookup"><span data-stu-id="3a289-135">String</span></span>|<span data-ttu-id="3a289-136">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="3a289-136">Name of the setting</span></span>|
|<span data-ttu-id="3a289-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="3a289-137">instancePath</span></span>|<span data-ttu-id="3a289-138">String</span><span class="sxs-lookup"><span data-stu-id="3a289-138">String</span></span>|<span data-ttu-id="3a289-139">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="3a289-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="3a289-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3a289-140">unknownDeviceCount</span></span>|<span data-ttu-id="3a289-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3a289-141">Int32</span></span>|<span data-ttu-id="3a289-142">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="3a289-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="3a289-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3a289-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="3a289-144">Int32</span><span class="sxs-lookup"><span data-stu-id="3a289-144">Int32</span></span>|<span data-ttu-id="3a289-145">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="3a289-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="3a289-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3a289-146">compliantDeviceCount</span></span>|<span data-ttu-id="3a289-147">Int32</span><span class="sxs-lookup"><span data-stu-id="3a289-147">Int32</span></span>|<span data-ttu-id="3a289-148">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="3a289-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="3a289-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3a289-149">remediatedDeviceCount</span></span>|<span data-ttu-id="3a289-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3a289-150">Int32</span></span>|<span data-ttu-id="3a289-151">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="3a289-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="3a289-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3a289-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3a289-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3a289-153">Int32</span></span>|<span data-ttu-id="3a289-154">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="3a289-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="3a289-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3a289-155">errorDeviceCount</span></span>|<span data-ttu-id="3a289-156">Int32</span><span class="sxs-lookup"><span data-stu-id="3a289-156">Int32</span></span>|<span data-ttu-id="3a289-157">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="3a289-157">Device error count for the setting</span></span>|
|<span data-ttu-id="3a289-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3a289-158">conflictDeviceCount</span></span>|<span data-ttu-id="3a289-159">Int32</span><span class="sxs-lookup"><span data-stu-id="3a289-159">Int32</span></span>|<span data-ttu-id="3a289-160">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="3a289-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="3a289-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a289-161">Response</span></span>
<span data-ttu-id="3a289-162">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a289-162">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a289-163">Пример</span><span class="sxs-lookup"><span data-stu-id="3a289-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a289-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a289-164">Request</span></span>
<span data-ttu-id="3a289-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a289-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a289-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a289-166">Response</span></span>
<span data-ttu-id="3a289-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a289-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



