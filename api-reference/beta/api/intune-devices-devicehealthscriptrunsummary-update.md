---
title: Обновление Девицехеалсскриптрунсуммари
description: Обновление свойств объекта Девицехеалсскриптрунсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a102b6624a2bedf70708ac4fedb03c523c34511
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945041"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="b9ba1-103">Обновление Девицехеалсскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="b9ba1-103">Update deviceHealthScriptRunSummary</span></span>

> <span data-ttu-id="b9ba1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9ba1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9ba1-106">Обновление свойств объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b9ba1-106">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9ba1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b9ba1-107">Prerequisites</span></span>
<span data-ttu-id="b9ba1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9ba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9ba1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9ba1-110">Permission type</span></span>|<span data-ttu-id="b9ba1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9ba1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9ba1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9ba1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9ba1-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9ba1-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b9ba1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9ba1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9ba1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-115">Not supported.</span></span>|
|<span data-ttu-id="b9ba1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9ba1-116">Application</span></span>|<span data-ttu-id="b9ba1-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9ba1-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9ba1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9ba1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="b9ba1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b9ba1-119">Request headers</span></span>
|<span data-ttu-id="b9ba1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9ba1-120">Header</span></span>|<span data-ttu-id="b9ba1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b9ba1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9ba1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9ba1-122">Authorization</span></span>|<span data-ttu-id="b9ba1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9ba1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b9ba1-124">Accept</span></span>|<span data-ttu-id="b9ba1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9ba1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9ba1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9ba1-126">Request body</span></span>
<span data-ttu-id="b9ba1-127">В тексте запроса добавьте представление объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-127">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="b9ba1-128">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b9ba1-128">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="b9ba1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9ba1-129">Property</span></span>|<span data-ttu-id="b9ba1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b9ba1-130">Type</span></span>|<span data-ttu-id="b9ba1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b9ba1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9ba1-132">id</span><span class="sxs-lookup"><span data-stu-id="b9ba1-132">id</span></span>|<span data-ttu-id="b9ba1-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b9ba1-133">String</span></span>|<span data-ttu-id="b9ba1-134">Ключевой объект сводки запуска сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-134">Key of the device health script run summary entity.</span></span> <span data-ttu-id="b9ba1-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-135">This property is read-only.</span></span>|
|<span data-ttu-id="b9ba1-136">ноиссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="b9ba1-136">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="b9ba1-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b9ba1-137">Int32</span></span>|<span data-ttu-id="b9ba1-138">Количество устройств, для которых сценарий обнаружения не обнаружил проблему, и устройство находится в работоспособном состоянии.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-138">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="b9ba1-139">иссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="b9ba1-139">issueDetectedDeviceCount</span></span>|<span data-ttu-id="b9ba1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b9ba1-140">Int32</span></span>|<span data-ttu-id="b9ba1-141">Количество устройств, для которых обнаружена ошибка сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="b9ba1-141">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="b9ba1-142">детектионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="b9ba1-142">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="b9ba1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b9ba1-143">Int32</span></span>|<span data-ttu-id="b9ba1-144">Количество устройств, на которых возникла ошибка при выполнении сценария обнаружения и который не был выполнен</span><span class="sxs-lookup"><span data-stu-id="b9ba1-144">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="b9ba1-145">детектионскриптпендингдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="b9ba1-145">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="b9ba1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b9ba1-146">Int32</span></span>|<span data-ttu-id="b9ba1-147">Количество устройств, на которых еще не выполнялась последняя версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="b9ba1-147">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="b9ba1-148">иссуеремедиатеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="b9ba1-148">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="b9ba1-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b9ba1-149">Int32</span></span>|<span data-ttu-id="b9ba1-150">Количество устройств, для которых сценарий исправления мог разрешить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="b9ba1-150">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="b9ba1-151">ремедиатионскиппеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="b9ba1-151">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="b9ba1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b9ba1-152">Int32</span></span>|<span data-ttu-id="b9ba1-153">Количество устройств, для которых было пропущено исправление</span><span class="sxs-lookup"><span data-stu-id="b9ba1-153">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="b9ba1-154">иссуереоккурреддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="b9ba1-154">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="b9ba1-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b9ba1-155">Int32</span></span>|<span data-ttu-id="b9ba1-156">Количество устройств, для которых сценарий исправления успешно выполнен, но не удалось разрешить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="b9ba1-156">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="b9ba1-157">ремедиатионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="b9ba1-157">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="b9ba1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b9ba1-158">Int32</span></span>|<span data-ttu-id="b9ba1-159">Количество устройств, для которых при выполнении сценария исправления возникла ошибка и оно не было завершено</span><span class="sxs-lookup"><span data-stu-id="b9ba1-159">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="b9ba1-160">ластскриптрундатетиме</span><span class="sxs-lookup"><span data-stu-id="b9ba1-160">lastScriptRunDateTime</span></span>|<span data-ttu-id="b9ba1-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9ba1-161">DateTimeOffset</span></span>|<span data-ttu-id="b9ba1-162">Время последнего запуска сценария на всех устройствах</span><span class="sxs-lookup"><span data-stu-id="b9ba1-162">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="b9ba1-163">иссуеремедиатедкумулативедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="b9ba1-163">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="b9ba1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b9ba1-164">Int32</span></span>|<span data-ttu-id="b9ba1-165">Количество устройств, которые были исправлены за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="b9ba1-165">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="b9ba1-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9ba1-166">Response</span></span>
<span data-ttu-id="b9ba1-167">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-167">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9ba1-168">Пример</span><span class="sxs-lookup"><span data-stu-id="b9ba1-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9ba1-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9ba1-169">Request</span></span>
<span data-ttu-id="b9ba1-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```

### <a name="response"></a><span data-ttu-id="b9ba1-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9ba1-171">Response</span></span>
<span data-ttu-id="b9ba1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9ba1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "8221b043-b043-8221-43b0-218243b02182",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```





