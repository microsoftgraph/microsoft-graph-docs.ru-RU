---
title: Обновление Девицехеалсскриптрунсуммари
description: Обновление свойств объекта Девицехеалсскриптрунсуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f6852123f88c76e8eac25f9689b7e14dbf182ee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077046"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="9dbe3-103">Обновление Девицехеалсскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="9dbe3-103">Update deviceHealthScriptRunSummary</span></span>

<span data-ttu-id="9dbe3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dbe3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9dbe3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9dbe3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dbe3-107">Обновление свойств объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9dbe3-107">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dbe3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9dbe3-108">Prerequisites</span></span>
<span data-ttu-id="9dbe3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dbe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dbe3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dbe3-111">Permission type</span></span>|<span data-ttu-id="9dbe3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dbe3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dbe3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dbe3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9dbe3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9dbe3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9dbe3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dbe3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dbe3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-116">Not supported.</span></span>|
|<span data-ttu-id="9dbe3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dbe3-117">Application</span></span>|<span data-ttu-id="9dbe3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9dbe3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dbe3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dbe3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="9dbe3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9dbe3-120">Request headers</span></span>
|<span data-ttu-id="9dbe3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dbe3-121">Header</span></span>|<span data-ttu-id="9dbe3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9dbe3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dbe3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dbe3-123">Authorization</span></span>|<span data-ttu-id="9dbe3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dbe3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9dbe3-125">Accept</span></span>|<span data-ttu-id="9dbe3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9dbe3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dbe3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dbe3-127">Request body</span></span>
<span data-ttu-id="9dbe3-128">В тексте запроса добавьте представление объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-128">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="9dbe3-129">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="9dbe3-129">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="9dbe3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dbe3-130">Property</span></span>|<span data-ttu-id="9dbe3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9dbe3-131">Type</span></span>|<span data-ttu-id="9dbe3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9dbe3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dbe3-133">id</span><span class="sxs-lookup"><span data-stu-id="9dbe3-133">id</span></span>|<span data-ttu-id="9dbe3-134">String</span><span class="sxs-lookup"><span data-stu-id="9dbe3-134">String</span></span>|<span data-ttu-id="9dbe3-135">Ключевой объект сводки запуска сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-135">Key of the device health script run summary entity.</span></span> <span data-ttu-id="9dbe3-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-136">This property is read-only.</span></span>|
|<span data-ttu-id="9dbe3-137">ноиссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9dbe3-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="9dbe3-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbe3-138">Int32</span></span>|<span data-ttu-id="9dbe3-139">Количество устройств, для которых сценарий обнаружения не обнаружил проблему, и устройство находится в работоспособном состоянии.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-139">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="9dbe3-140">иссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9dbe3-140">issueDetectedDeviceCount</span></span>|<span data-ttu-id="9dbe3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbe3-141">Int32</span></span>|<span data-ttu-id="9dbe3-142">Количество устройств, для которых обнаружена ошибка сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="9dbe3-142">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="9dbe3-143">детектионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9dbe3-143">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="9dbe3-144">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbe3-144">Int32</span></span>|<span data-ttu-id="9dbe3-145">Количество устройств, на которых возникла ошибка при выполнении сценария обнаружения и который не был выполнен</span><span class="sxs-lookup"><span data-stu-id="9dbe3-145">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="9dbe3-146">детектионскриптпендингдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9dbe3-146">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="9dbe3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbe3-147">Int32</span></span>|<span data-ttu-id="9dbe3-148">Количество устройств, на которых еще не выполнялась последняя версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="9dbe3-148">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="9dbe3-149">иссуеремедиатеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9dbe3-149">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="9dbe3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbe3-150">Int32</span></span>|<span data-ttu-id="9dbe3-151">Количество устройств, для которых сценарий исправления мог разрешить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="9dbe3-151">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="9dbe3-152">ремедиатионскиппеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9dbe3-152">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="9dbe3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbe3-153">Int32</span></span>|<span data-ttu-id="9dbe3-154">Количество устройств, для которых было пропущено исправление</span><span class="sxs-lookup"><span data-stu-id="9dbe3-154">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="9dbe3-155">иссуереоккурреддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9dbe3-155">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="9dbe3-156">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbe3-156">Int32</span></span>|<span data-ttu-id="9dbe3-157">Количество устройств, для которых сценарий исправления успешно выполнен, но не удалось разрешить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="9dbe3-157">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="9dbe3-158">ремедиатионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9dbe3-158">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="9dbe3-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbe3-159">Int32</span></span>|<span data-ttu-id="9dbe3-160">Количество устройств, для которых при выполнении сценария исправления возникла ошибка и оно не было завершено</span><span class="sxs-lookup"><span data-stu-id="9dbe3-160">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="9dbe3-161">ластскриптрундатетиме</span><span class="sxs-lookup"><span data-stu-id="9dbe3-161">lastScriptRunDateTime</span></span>|<span data-ttu-id="9dbe3-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dbe3-162">DateTimeOffset</span></span>|<span data-ttu-id="9dbe3-163">Время последнего запуска сценария на всех устройствах</span><span class="sxs-lookup"><span data-stu-id="9dbe3-163">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="9dbe3-164">иссуеремедиатедкумулативедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9dbe3-164">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="9dbe3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbe3-165">Int32</span></span>|<span data-ttu-id="9dbe3-166">Количество устройств, которые были исправлены за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="9dbe3-166">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="9dbe3-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dbe3-167">Response</span></span>
<span data-ttu-id="9dbe3-168">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-168">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dbe3-169">Пример</span><span class="sxs-lookup"><span data-stu-id="9dbe3-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dbe3-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dbe3-170">Request</span></span>
<span data-ttu-id="9dbe3-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9dbe3-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dbe3-172">Response</span></span>
<span data-ttu-id="9dbe3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9dbe3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






