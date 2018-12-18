---
title: Обновление объекта settingStateDeviceSummary
description: Обновление свойств объекта settingStateDeviceSummary.
author: tfitzmac
ms.openlocfilehash: 531b8f80aff08e2b8e4faa1444ecc0b264d39a4d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323592"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="dd784-103">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="dd784-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="dd784-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dd784-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd784-105">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="dd784-105">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd784-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dd784-106">Prerequisites</span></span>
<span data-ttu-id="dd784-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd784-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd784-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd784-109">Permission type</span></span>|<span data-ttu-id="dd784-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd784-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd784-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd784-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd784-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd784-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd784-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd784-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd784-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd784-114">Not supported.</span></span>|
|<span data-ttu-id="dd784-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd784-115">Application</span></span>|<span data-ttu-id="dd784-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd784-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd784-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd784-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="dd784-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd784-118">Request headers</span></span>
|<span data-ttu-id="dd784-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd784-119">Header</span></span>|<span data-ttu-id="dd784-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dd784-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd784-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd784-121">Authorization</span></span>|<span data-ttu-id="dd784-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dd784-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd784-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dd784-123">Accept</span></span>|<span data-ttu-id="dd784-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dd784-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd784-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd784-125">Request body</span></span>
<span data-ttu-id="dd784-126">В теле запроса добавьте представление объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd784-126">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="dd784-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="dd784-127">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="dd784-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd784-128">Property</span></span>|<span data-ttu-id="dd784-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dd784-129">Type</span></span>|<span data-ttu-id="dd784-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dd784-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd784-131">id</span><span class="sxs-lookup"><span data-stu-id="dd784-131">id</span></span>|<span data-ttu-id="dd784-132">Строка</span><span class="sxs-lookup"><span data-stu-id="dd784-132">String</span></span>|<span data-ttu-id="dd784-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd784-133">Key of the entity.</span></span>|
|<span data-ttu-id="dd784-134">settingName</span><span class="sxs-lookup"><span data-stu-id="dd784-134">settingName</span></span>|<span data-ttu-id="dd784-135">String</span><span class="sxs-lookup"><span data-stu-id="dd784-135">String</span></span>|<span data-ttu-id="dd784-136">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="dd784-136">Name of the setting</span></span>|
|<span data-ttu-id="dd784-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="dd784-137">instancePath</span></span>|<span data-ttu-id="dd784-138">String</span><span class="sxs-lookup"><span data-stu-id="dd784-138">String</span></span>|<span data-ttu-id="dd784-139">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="dd784-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="dd784-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd784-140">unknownDeviceCount</span></span>|<span data-ttu-id="dd784-141">Int32</span><span class="sxs-lookup"><span data-stu-id="dd784-141">Int32</span></span>|<span data-ttu-id="dd784-142">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="dd784-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="dd784-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd784-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="dd784-144">Int32</span><span class="sxs-lookup"><span data-stu-id="dd784-144">Int32</span></span>|<span data-ttu-id="dd784-145">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="dd784-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="dd784-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd784-146">compliantDeviceCount</span></span>|<span data-ttu-id="dd784-147">Int32</span><span class="sxs-lookup"><span data-stu-id="dd784-147">Int32</span></span>|<span data-ttu-id="dd784-148">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="dd784-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="dd784-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd784-149">remediatedDeviceCount</span></span>|<span data-ttu-id="dd784-150">Int32</span><span class="sxs-lookup"><span data-stu-id="dd784-150">Int32</span></span>|<span data-ttu-id="dd784-151">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="dd784-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="dd784-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd784-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="dd784-153">Int32</span><span class="sxs-lookup"><span data-stu-id="dd784-153">Int32</span></span>|<span data-ttu-id="dd784-154">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="dd784-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="dd784-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd784-155">errorDeviceCount</span></span>|<span data-ttu-id="dd784-156">Int32</span><span class="sxs-lookup"><span data-stu-id="dd784-156">Int32</span></span>|<span data-ttu-id="dd784-157">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="dd784-157">Device error count for the setting</span></span>|
|<span data-ttu-id="dd784-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd784-158">conflictDeviceCount</span></span>|<span data-ttu-id="dd784-159">Int32</span><span class="sxs-lookup"><span data-stu-id="dd784-159">Int32</span></span>|<span data-ttu-id="dd784-160">Количество конфликтов устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="dd784-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="dd784-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd784-161">Response</span></span>
<span data-ttu-id="dd784-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dd784-162">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd784-163">Пример</span><span class="sxs-lookup"><span data-stu-id="dd784-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd784-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd784-164">Request</span></span>
<span data-ttu-id="dd784-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd784-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dd784-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd784-166">Response</span></span>
<span data-ttu-id="dd784-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dd784-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



