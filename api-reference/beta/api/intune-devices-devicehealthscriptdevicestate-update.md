---
title: Обновление Девицехеалсскриптдевицестате
description: Обновление свойств объекта Девицехеалсскриптдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ec3c9cb2825afb4c94ea0be9ddb947e370b16661
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37531086"
---
# <a name="update-devicehealthscriptdevicestate"></a><span data-ttu-id="94525-103">Обновление Девицехеалсскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="94525-103">Update deviceHealthScriptDeviceState</span></span>

> <span data-ttu-id="94525-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94525-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94525-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94525-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94525-106">Обновление свойств объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="94525-106">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94525-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="94525-107">Prerequisites</span></span>
<span data-ttu-id="94525-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94525-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94525-110">Permission type</span></span>|<span data-ttu-id="94525-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="94525-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94525-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94525-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94525-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94525-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="94525-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94525-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94525-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94525-115">Not supported.</span></span>|
|<span data-ttu-id="94525-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="94525-116">Application</span></span>|<span data-ttu-id="94525-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94525-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94525-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94525-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="94525-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94525-119">Request headers</span></span>
|<span data-ttu-id="94525-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94525-120">Header</span></span>|<span data-ttu-id="94525-121">Значение</span><span class="sxs-lookup"><span data-stu-id="94525-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94525-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94525-122">Authorization</span></span>|<span data-ttu-id="94525-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94525-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94525-124">Accept</span><span class="sxs-lookup"><span data-stu-id="94525-124">Accept</span></span>|<span data-ttu-id="94525-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94525-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94525-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94525-126">Request body</span></span>
<span data-ttu-id="94525-127">В тексте запроса добавьте представление объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94525-127">In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

<span data-ttu-id="94525-128">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="94525-128">The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>

|<span data-ttu-id="94525-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="94525-129">Property</span></span>|<span data-ttu-id="94525-130">Тип</span><span class="sxs-lookup"><span data-stu-id="94525-130">Type</span></span>|<span data-ttu-id="94525-131">Описание</span><span class="sxs-lookup"><span data-stu-id="94525-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94525-132">id</span><span class="sxs-lookup"><span data-stu-id="94525-132">id</span></span>|<span data-ttu-id="94525-133">String</span><span class="sxs-lookup"><span data-stu-id="94525-133">String</span></span>|<span data-ttu-id="94525-134">Ключ объекта состояния устройства сценария работоспособности.</span><span class="sxs-lookup"><span data-stu-id="94525-134">Key of the device health script device state entity.</span></span> <span data-ttu-id="94525-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94525-135">This property is read-only.</span></span>|
|<span data-ttu-id="94525-136">детектионстате</span><span class="sxs-lookup"><span data-stu-id="94525-136">detectionState</span></span>|[<span data-ttu-id="94525-137">рунстате</span><span class="sxs-lookup"><span data-stu-id="94525-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="94525-138">Состояние обнаружения с последнего выполнения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="94525-138">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="94525-139">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="94525-139">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="94525-140">ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="94525-140">lastStateUpdateDateTime</span></span>|<span data-ttu-id="94525-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94525-141">DateTimeOffset</span></span>|<span data-ttu-id="94525-142">Последняя метка времени выполнения сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="94525-142">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="94525-143">експектедстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="94525-143">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="94525-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94525-144">DateTimeOffset</span></span>|<span data-ttu-id="94525-145">Следующий штамп времени, когда ожидается выполнение сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="94525-145">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="94525-146">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="94525-146">lastSyncDateTime</span></span>|<span data-ttu-id="94525-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94525-147">DateTimeOffset</span></span>|<span data-ttu-id="94525-148">Время последнего синхронизации расширения управления Intune с Intune</span><span class="sxs-lookup"><span data-stu-id="94525-148">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="94525-149">преремедиатиондетектионскриптаутпут</span><span class="sxs-lookup"><span data-stu-id="94525-149">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="94525-150">String</span><span class="sxs-lookup"><span data-stu-id="94525-150">String</span></span>|<span data-ttu-id="94525-151">Выходные данные сценария обнаружения перед исправлением</span><span class="sxs-lookup"><span data-stu-id="94525-151">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="94525-152">преремедиатиондетектионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="94525-152">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="94525-153">String</span><span class="sxs-lookup"><span data-stu-id="94525-153">String</span></span>|<span data-ttu-id="94525-154">Ошибка сценария обнаружения перед исправлением</span><span class="sxs-lookup"><span data-stu-id="94525-154">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="94525-155">ремедиатионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="94525-155">remediationScriptError</span></span>|<span data-ttu-id="94525-156">String</span><span class="sxs-lookup"><span data-stu-id="94525-156">String</span></span>|<span data-ttu-id="94525-157">Вывод ошибок сценария исправления</span><span class="sxs-lookup"><span data-stu-id="94525-157">Error output of the remediation script</span></span>|
|<span data-ttu-id="94525-158">постремедиатиондетектионскриптаутпут</span><span class="sxs-lookup"><span data-stu-id="94525-158">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="94525-159">String</span><span class="sxs-lookup"><span data-stu-id="94525-159">String</span></span>|<span data-ttu-id="94525-160">Выходные данные сценария обнаружения после исправления</span><span class="sxs-lookup"><span data-stu-id="94525-160">Detection script output after remediation</span></span>|
|<span data-ttu-id="94525-161">постремедиатиондетектионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="94525-161">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="94525-162">String</span><span class="sxs-lookup"><span data-stu-id="94525-162">String</span></span>|<span data-ttu-id="94525-163">Ошибка сценария обнаружения после исправления</span><span class="sxs-lookup"><span data-stu-id="94525-163">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="94525-164">ремедиатионстате</span><span class="sxs-lookup"><span data-stu-id="94525-164">remediationState</span></span>|[<span data-ttu-id="94525-165">ремедиатионстате</span><span class="sxs-lookup"><span data-stu-id="94525-165">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="94525-166">Состояние исправления с последнего выполнения скрипта работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="94525-166">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="94525-167">Возможные значения: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span><span class="sxs-lookup"><span data-stu-id="94525-167">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="94525-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="94525-168">Response</span></span>
<span data-ttu-id="94525-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94525-169">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94525-170">Пример</span><span class="sxs-lookup"><span data-stu-id="94525-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="94525-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="94525-171">Request</span></span>
<span data-ttu-id="94525-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94525-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
Content-type: application/json
Content-length: 762

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped"
}
```

### <a name="response"></a><span data-ttu-id="94525-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="94525-173">Response</span></span>
<span data-ttu-id="94525-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94525-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 811

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "fd2e4505-4505-fd2e-0545-2efd05452efd",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped"
}
```






