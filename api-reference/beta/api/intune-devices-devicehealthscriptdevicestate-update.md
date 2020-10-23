---
title: Обновление Девицехеалсскриптдевицестате
description: Обновление свойств объекта Девицехеалсскриптдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5537e1bfa95780545df9e7c53f19c688477f0b78
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736529"
---
# <a name="update-devicehealthscriptdevicestate"></a><span data-ttu-id="98b4e-103">Обновление Девицехеалсскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="98b4e-103">Update deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="98b4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98b4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98b4e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98b4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98b4e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98b4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98b4e-107">Обновление свойств объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="98b4e-107">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98b4e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="98b4e-108">Prerequisites</span></span>
<span data-ttu-id="98b4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98b4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98b4e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98b4e-111">Permission type</span></span>|<span data-ttu-id="98b4e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98b4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98b4e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98b4e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98b4e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="98b4e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="98b4e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98b4e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98b4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98b4e-116">Not supported.</span></span>|
|<span data-ttu-id="98b4e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98b4e-117">Application</span></span>|<span data-ttu-id="98b4e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="98b4e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98b4e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98b4e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="98b4e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98b4e-120">Request headers</span></span>
|<span data-ttu-id="98b4e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98b4e-121">Header</span></span>|<span data-ttu-id="98b4e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98b4e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98b4e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98b4e-123">Authorization</span></span>|<span data-ttu-id="98b4e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98b4e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98b4e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98b4e-125">Accept</span></span>|<span data-ttu-id="98b4e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98b4e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98b4e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98b4e-127">Request body</span></span>
<span data-ttu-id="98b4e-128">В тексте запроса добавьте представление объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98b4e-128">In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

<span data-ttu-id="98b4e-129">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="98b4e-129">The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>

|<span data-ttu-id="98b4e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="98b4e-130">Property</span></span>|<span data-ttu-id="98b4e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="98b4e-131">Type</span></span>|<span data-ttu-id="98b4e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="98b4e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b4e-133">id</span><span class="sxs-lookup"><span data-stu-id="98b4e-133">id</span></span>|<span data-ttu-id="98b4e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="98b4e-134">String</span></span>|<span data-ttu-id="98b4e-135">Ключ объекта состояния устройства сценария работоспособности.</span><span class="sxs-lookup"><span data-stu-id="98b4e-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="98b4e-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98b4e-136">This property is read-only.</span></span>|
|<span data-ttu-id="98b4e-137">детектионстате</span><span class="sxs-lookup"><span data-stu-id="98b4e-137">detectionState</span></span>|[<span data-ttu-id="98b4e-138">рунстате</span><span class="sxs-lookup"><span data-stu-id="98b4e-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="98b4e-139">Состояние обнаружения с последнего выполнения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="98b4e-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="98b4e-140">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="98b4e-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="98b4e-141">ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="98b4e-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="98b4e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98b4e-142">DateTimeOffset</span></span>|<span data-ttu-id="98b4e-143">Последняя метка времени выполнения сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="98b4e-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="98b4e-144">експектедстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="98b4e-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="98b4e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98b4e-145">DateTimeOffset</span></span>|<span data-ttu-id="98b4e-146">Следующий штамп времени, когда ожидается выполнение сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="98b4e-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="98b4e-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="98b4e-147">lastSyncDateTime</span></span>|<span data-ttu-id="98b4e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98b4e-148">DateTimeOffset</span></span>|<span data-ttu-id="98b4e-149">Время последнего синхронизации расширения управления Intune с Intune</span><span class="sxs-lookup"><span data-stu-id="98b4e-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="98b4e-150">преремедиатиондетектионскриптаутпут</span><span class="sxs-lookup"><span data-stu-id="98b4e-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="98b4e-151">Строка</span><span class="sxs-lookup"><span data-stu-id="98b4e-151">String</span></span>|<span data-ttu-id="98b4e-152">Выходные данные сценария обнаружения перед исправлением</span><span class="sxs-lookup"><span data-stu-id="98b4e-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="98b4e-153">преремедиатиондетектионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="98b4e-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="98b4e-154">Строка</span><span class="sxs-lookup"><span data-stu-id="98b4e-154">String</span></span>|<span data-ttu-id="98b4e-155">Ошибка сценария обнаружения перед исправлением</span><span class="sxs-lookup"><span data-stu-id="98b4e-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="98b4e-156">ремедиатионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="98b4e-156">remediationScriptError</span></span>|<span data-ttu-id="98b4e-157">Строка</span><span class="sxs-lookup"><span data-stu-id="98b4e-157">String</span></span>|<span data-ttu-id="98b4e-158">Вывод ошибок сценария исправления</span><span class="sxs-lookup"><span data-stu-id="98b4e-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="98b4e-159">постремедиатиондетектионскриптаутпут</span><span class="sxs-lookup"><span data-stu-id="98b4e-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="98b4e-160">Строка</span><span class="sxs-lookup"><span data-stu-id="98b4e-160">String</span></span>|<span data-ttu-id="98b4e-161">Выходные данные сценария обнаружения после исправления</span><span class="sxs-lookup"><span data-stu-id="98b4e-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="98b4e-162">постремедиатиондетектионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="98b4e-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="98b4e-163">Строка</span><span class="sxs-lookup"><span data-stu-id="98b4e-163">String</span></span>|<span data-ttu-id="98b4e-164">Ошибка сценария обнаружения после исправления</span><span class="sxs-lookup"><span data-stu-id="98b4e-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="98b4e-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="98b4e-165">remediationState</span></span>|[<span data-ttu-id="98b4e-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="98b4e-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="98b4e-167">Состояние исправления с последнего выполнения скрипта работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="98b4e-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="98b4e-168">Возможные значения: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span><span class="sxs-lookup"><span data-stu-id="98b4e-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="98b4e-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="98b4e-169">Response</span></span>
<span data-ttu-id="98b4e-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98b4e-170">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98b4e-171">Пример</span><span class="sxs-lookup"><span data-stu-id="98b4e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="98b4e-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="98b4e-172">Request</span></span>
<span data-ttu-id="98b4e-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98b4e-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="98b4e-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="98b4e-174">Response</span></span>
<span data-ttu-id="98b4e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98b4e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





