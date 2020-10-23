---
title: Обновление Девицехеалсскриптрунсуммари
description: Обновление свойств объекта Девицехеалсскриптрунсуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2b1d00b523e989d927e834b54f8b748bb93d301
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729210"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="5ed46-103">Обновление Девицехеалсскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="5ed46-103">Update deviceHealthScriptRunSummary</span></span>

<span data-ttu-id="5ed46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ed46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ed46-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ed46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ed46-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ed46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ed46-107">Обновление свойств объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5ed46-107">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ed46-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ed46-108">Prerequisites</span></span>
<span data-ttu-id="5ed46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ed46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ed46-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ed46-111">Permission type</span></span>|<span data-ttu-id="5ed46-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ed46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ed46-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ed46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ed46-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ed46-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5ed46-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ed46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ed46-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ed46-116">Not supported.</span></span>|
|<span data-ttu-id="5ed46-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ed46-117">Application</span></span>|<span data-ttu-id="5ed46-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ed46-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ed46-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ed46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="5ed46-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5ed46-120">Request headers</span></span>
|<span data-ttu-id="5ed46-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ed46-121">Header</span></span>|<span data-ttu-id="5ed46-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5ed46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ed46-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ed46-123">Authorization</span></span>|<span data-ttu-id="5ed46-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ed46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ed46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5ed46-125">Accept</span></span>|<span data-ttu-id="5ed46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ed46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ed46-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ed46-127">Request body</span></span>
<span data-ttu-id="5ed46-128">В тексте запроса добавьте представление объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ed46-128">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="5ed46-129">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="5ed46-129">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="5ed46-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ed46-130">Property</span></span>|<span data-ttu-id="5ed46-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5ed46-131">Type</span></span>|<span data-ttu-id="5ed46-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5ed46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed46-133">id</span><span class="sxs-lookup"><span data-stu-id="5ed46-133">id</span></span>|<span data-ttu-id="5ed46-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5ed46-134">String</span></span>|<span data-ttu-id="5ed46-135">Ключевой объект сводки запуска сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="5ed46-135">Key of the device health script run summary entity.</span></span> <span data-ttu-id="5ed46-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ed46-136">This property is read-only.</span></span>|
|<span data-ttu-id="5ed46-137">ноиссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5ed46-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="5ed46-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed46-138">Int32</span></span>|<span data-ttu-id="5ed46-139">Количество устройств, для которых сценарий обнаружения не обнаружил проблему, и устройство находится в работоспособном состоянии.</span><span class="sxs-lookup"><span data-stu-id="5ed46-139">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="5ed46-140">иссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5ed46-140">issueDetectedDeviceCount</span></span>|<span data-ttu-id="5ed46-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed46-141">Int32</span></span>|<span data-ttu-id="5ed46-142">Количество устройств, для которых обнаружена ошибка сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="5ed46-142">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="5ed46-143">детектионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5ed46-143">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="5ed46-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed46-144">Int32</span></span>|<span data-ttu-id="5ed46-145">Количество устройств, на которых возникла ошибка при выполнении сценария обнаружения и который не был выполнен</span><span class="sxs-lookup"><span data-stu-id="5ed46-145">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="5ed46-146">детектионскриптпендингдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5ed46-146">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="5ed46-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed46-147">Int32</span></span>|<span data-ttu-id="5ed46-148">Количество устройств, на которых еще не выполнялась последняя версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="5ed46-148">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="5ed46-149">иссуеремедиатеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5ed46-149">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="5ed46-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed46-150">Int32</span></span>|<span data-ttu-id="5ed46-151">Количество устройств, для которых сценарий исправления мог разрешить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="5ed46-151">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="5ed46-152">ремедиатионскиппеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5ed46-152">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="5ed46-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed46-153">Int32</span></span>|<span data-ttu-id="5ed46-154">Количество устройств, для которых было пропущено исправление</span><span class="sxs-lookup"><span data-stu-id="5ed46-154">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="5ed46-155">иссуереоккурреддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5ed46-155">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="5ed46-156">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed46-156">Int32</span></span>|<span data-ttu-id="5ed46-157">Количество устройств, для которых сценарий исправления успешно выполнен, но не удалось разрешить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="5ed46-157">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="5ed46-158">ремедиатионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5ed46-158">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="5ed46-159">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed46-159">Int32</span></span>|<span data-ttu-id="5ed46-160">Количество устройств, для которых при выполнении сценария исправления возникла ошибка и оно не было завершено</span><span class="sxs-lookup"><span data-stu-id="5ed46-160">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="5ed46-161">ластскриптрундатетиме</span><span class="sxs-lookup"><span data-stu-id="5ed46-161">lastScriptRunDateTime</span></span>|<span data-ttu-id="5ed46-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed46-162">DateTimeOffset</span></span>|<span data-ttu-id="5ed46-163">Время последнего запуска сценария на всех устройствах</span><span class="sxs-lookup"><span data-stu-id="5ed46-163">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="5ed46-164">иссуеремедиатедкумулативедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5ed46-164">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="5ed46-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed46-165">Int32</span></span>|<span data-ttu-id="5ed46-166">Количество устройств, которые были исправлены за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="5ed46-166">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="5ed46-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ed46-167">Response</span></span>
<span data-ttu-id="5ed46-168">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ed46-168">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ed46-169">Пример</span><span class="sxs-lookup"><span data-stu-id="5ed46-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ed46-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ed46-170">Request</span></span>
<span data-ttu-id="5ed46-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ed46-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5ed46-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ed46-172">Response</span></span>
<span data-ttu-id="5ed46-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ed46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





