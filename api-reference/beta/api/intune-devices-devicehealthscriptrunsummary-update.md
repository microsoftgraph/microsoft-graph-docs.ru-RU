---
title: Обновление устройстваHealthScriptRunSummary
description: Обновление свойств объекта deviceHealthScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72dd3594aee3bc9a19c7195e67201c7f54270b9b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127083"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="b1552-103">Обновление устройстваHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="b1552-103">Update deviceHealthScriptRunSummary</span></span>

<span data-ttu-id="b1552-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1552-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1552-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1552-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1552-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1552-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1552-107">Обновление свойств объекта [deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="b1552-107">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1552-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1552-108">Prerequisites</span></span>
<span data-ttu-id="b1552-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1552-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1552-111">Permission type</span></span>|<span data-ttu-id="b1552-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1552-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1552-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1552-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1552-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1552-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1552-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1552-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1552-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1552-116">Not supported.</span></span>|
|<span data-ttu-id="b1552-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b1552-117">Application</span></span>|<span data-ttu-id="b1552-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1552-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1552-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1552-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="b1552-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1552-120">Request headers</span></span>
|<span data-ttu-id="b1552-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1552-121">Header</span></span>|<span data-ttu-id="b1552-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b1552-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1552-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1552-123">Authorization</span></span>|<span data-ttu-id="b1552-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1552-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1552-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1552-125">Accept</span></span>|<span data-ttu-id="b1552-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1552-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1552-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1552-127">Request body</span></span>
<span data-ttu-id="b1552-128">В теле запроса поставляем представление JSON для [объекта deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="b1552-128">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="b1552-129">В следующей таблице показаны свойства, необходимые при создании [устройстваHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="b1552-129">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="b1552-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1552-130">Property</span></span>|<span data-ttu-id="b1552-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b1552-131">Type</span></span>|<span data-ttu-id="b1552-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b1552-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1552-133">id</span><span class="sxs-lookup"><span data-stu-id="b1552-133">id</span></span>|<span data-ttu-id="b1552-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b1552-134">String</span></span>|<span data-ttu-id="b1552-135">Ключ скрипта для службы службы устройств запустите объект сводки.</span><span class="sxs-lookup"><span data-stu-id="b1552-135">Key of the device health script run summary entity.</span></span> <span data-ttu-id="b1552-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1552-136">This property is read-only.</span></span>|
|<span data-ttu-id="b1552-137">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1552-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="b1552-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b1552-138">Int32</span></span>|<span data-ttu-id="b1552-139">Количество устройств, для которых сценарий обнаружения не нашел проблемы и устройство является здоровым</span><span class="sxs-lookup"><span data-stu-id="b1552-139">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="b1552-140">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1552-140">issueDetectedDeviceCount</span></span>|<span data-ttu-id="b1552-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b1552-141">Int32</span></span>|<span data-ttu-id="b1552-142">Количество устройств, для которых скрипт обнаружения обнаружил проблему</span><span class="sxs-lookup"><span data-stu-id="b1552-142">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="b1552-143">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1552-143">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="b1552-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b1552-144">Int32</span></span>|<span data-ttu-id="b1552-145">Количество устройств, на которых при выполнении скрипта обнаружения произошла ошибка и не была завершена</span><span class="sxs-lookup"><span data-stu-id="b1552-145">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="b1552-146">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1552-146">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="b1552-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b1552-147">Int32</span></span>|<span data-ttu-id="b1552-148">Количество устройств, которые еще не запускают последнюю версию скрипта здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="b1552-148">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="b1552-149">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1552-149">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="b1552-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b1552-150">Int32</span></span>|<span data-ttu-id="b1552-151">Количество устройств, для которых сценарий восстановления смог устранить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="b1552-151">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="b1552-152">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1552-152">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="b1552-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b1552-153">Int32</span></span>|<span data-ttu-id="b1552-154">Количество устройств, для которых было пропущено исправление</span><span class="sxs-lookup"><span data-stu-id="b1552-154">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="b1552-155">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1552-155">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="b1552-156">Int32</span><span class="sxs-lookup"><span data-stu-id="b1552-156">Int32</span></span>|<span data-ttu-id="b1552-157">Количество устройств, для которых успешно выполнен сценарий восстановления, но не удалось устранить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="b1552-157">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="b1552-158">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1552-158">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="b1552-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b1552-159">Int32</span></span>|<span data-ttu-id="b1552-160">Количество устройств, для которых при выполнении сценария восстановления произошла ошибка и не была завершена</span><span class="sxs-lookup"><span data-stu-id="b1552-160">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="b1552-161">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="b1552-161">lastScriptRunDateTime</span></span>|<span data-ttu-id="b1552-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1552-162">DateTimeOffset</span></span>|<span data-ttu-id="b1552-163">Время последнего запуска сценария на всех устройствах</span><span class="sxs-lookup"><span data-stu-id="b1552-163">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="b1552-164">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1552-164">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="b1552-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b1552-165">Int32</span></span>|<span data-ttu-id="b1552-166">Количество устройств, которые были исправлены за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="b1552-166">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="b1552-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1552-167">Response</span></span>
<span data-ttu-id="b1552-168">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b1552-168">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1552-169">Пример</span><span class="sxs-lookup"><span data-stu-id="b1552-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1552-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1552-170">Request</span></span>
<span data-ttu-id="b1552-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1552-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1552-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1552-172">Response</span></span>
<span data-ttu-id="b1552-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1552-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




