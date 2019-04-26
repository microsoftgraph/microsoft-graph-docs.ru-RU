---
title: Create settingStateDeviceSummary
description: Создание объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b91ab722e2918309d3b944b56f5c32ad6d463a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561154"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="68eba-103">Create settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="68eba-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="68eba-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68eba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68eba-105">Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="68eba-105">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68eba-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="68eba-106">Prerequisites</span></span>
<span data-ttu-id="68eba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68eba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68eba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68eba-109">Permission type</span></span>|<span data-ttu-id="68eba-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68eba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68eba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68eba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68eba-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68eba-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68eba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68eba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68eba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68eba-114">Not supported.</span></span>|
|<span data-ttu-id="68eba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68eba-115">Application</span></span>|<span data-ttu-id="68eba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68eba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68eba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68eba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="68eba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68eba-118">Request headers</span></span>
|<span data-ttu-id="68eba-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68eba-119">Header</span></span>|<span data-ttu-id="68eba-120">Значение</span><span class="sxs-lookup"><span data-stu-id="68eba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68eba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68eba-121">Authorization</span></span>|<span data-ttu-id="68eba-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68eba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68eba-123">Accept</span><span class="sxs-lookup"><span data-stu-id="68eba-123">Accept</span></span>|<span data-ttu-id="68eba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="68eba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68eba-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68eba-125">Request body</span></span>
<span data-ttu-id="68eba-126">В теле запроса добавьте представление объекта settingStateDeviceSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68eba-126">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="68eba-127">Ниже показаны свойства, которые необходимо указывать при создании объекта settingStateDeviceSummary.</span><span class="sxs-lookup"><span data-stu-id="68eba-127">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="68eba-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="68eba-128">Property</span></span>|<span data-ttu-id="68eba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="68eba-129">Type</span></span>|<span data-ttu-id="68eba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="68eba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68eba-131">id</span><span class="sxs-lookup"><span data-stu-id="68eba-131">id</span></span>|<span data-ttu-id="68eba-132">String</span><span class="sxs-lookup"><span data-stu-id="68eba-132">String</span></span>|<span data-ttu-id="68eba-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="68eba-133">Key of the entity.</span></span>|
|<span data-ttu-id="68eba-134">settingName</span><span class="sxs-lookup"><span data-stu-id="68eba-134">settingName</span></span>|<span data-ttu-id="68eba-135">String</span><span class="sxs-lookup"><span data-stu-id="68eba-135">String</span></span>|<span data-ttu-id="68eba-136">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="68eba-136">Name of the setting</span></span>|
|<span data-ttu-id="68eba-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="68eba-137">instancePath</span></span>|<span data-ttu-id="68eba-138">String</span><span class="sxs-lookup"><span data-stu-id="68eba-138">String</span></span>|<span data-ttu-id="68eba-139">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="68eba-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="68eba-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="68eba-140">unknownDeviceCount</span></span>|<span data-ttu-id="68eba-141">Int32</span><span class="sxs-lookup"><span data-stu-id="68eba-141">Int32</span></span>|<span data-ttu-id="68eba-142">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="68eba-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="68eba-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="68eba-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="68eba-144">Int32</span><span class="sxs-lookup"><span data-stu-id="68eba-144">Int32</span></span>|<span data-ttu-id="68eba-145">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="68eba-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="68eba-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="68eba-146">compliantDeviceCount</span></span>|<span data-ttu-id="68eba-147">Int32</span><span class="sxs-lookup"><span data-stu-id="68eba-147">Int32</span></span>|<span data-ttu-id="68eba-148">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="68eba-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="68eba-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="68eba-149">remediatedDeviceCount</span></span>|<span data-ttu-id="68eba-150">Int32</span><span class="sxs-lookup"><span data-stu-id="68eba-150">Int32</span></span>|<span data-ttu-id="68eba-151">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="68eba-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="68eba-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="68eba-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="68eba-153">Int32</span><span class="sxs-lookup"><span data-stu-id="68eba-153">Int32</span></span>|<span data-ttu-id="68eba-154">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="68eba-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="68eba-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="68eba-155">errorDeviceCount</span></span>|<span data-ttu-id="68eba-156">Int32</span><span class="sxs-lookup"><span data-stu-id="68eba-156">Int32</span></span>|<span data-ttu-id="68eba-157">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="68eba-157">Device error count for the setting</span></span>|
|<span data-ttu-id="68eba-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="68eba-158">conflictDeviceCount</span></span>|<span data-ttu-id="68eba-159">Int32</span><span class="sxs-lookup"><span data-stu-id="68eba-159">Int32</span></span>|<span data-ttu-id="68eba-160">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="68eba-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="68eba-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="68eba-161">Response</span></span>
<span data-ttu-id="68eba-162">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="68eba-162">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68eba-163">Пример</span><span class="sxs-lookup"><span data-stu-id="68eba-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="68eba-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="68eba-164">Request</span></span>
<span data-ttu-id="68eba-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68eba-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68eba-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="68eba-166">Response</span></span>
<span data-ttu-id="68eba-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68eba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



