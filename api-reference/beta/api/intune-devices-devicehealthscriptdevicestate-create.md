---
title: Создание Девицехеалсскриптдевицестате
description: Создание нового объекта Девицехеалсскриптдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69500d91eb5a22c5c3742256265d435ea0b31d0b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724278"
---
# <a name="create-devicehealthscriptdevicestate"></a><span data-ttu-id="7fad8-103">Создание Девицехеалсскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="7fad8-103">Create deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="7fad8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fad8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7fad8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fad8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fad8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7fad8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fad8-107">Создание нового объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="7fad8-107">Create a new [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fad8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7fad8-108">Prerequisites</span></span>
<span data-ttu-id="7fad8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fad8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fad8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fad8-111">Permission type</span></span>|<span data-ttu-id="7fad8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fad8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fad8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fad8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7fad8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fad8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7fad8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fad8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fad8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fad8-116">Not supported.</span></span>|
|<span data-ttu-id="7fad8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fad8-117">Application</span></span>|<span data-ttu-id="7fad8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fad8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fad8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fad8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="7fad8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7fad8-120">Request headers</span></span>
|<span data-ttu-id="7fad8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fad8-121">Header</span></span>|<span data-ttu-id="7fad8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7fad8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fad8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fad8-123">Authorization</span></span>|<span data-ttu-id="7fad8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fad8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fad8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7fad8-125">Accept</span></span>|<span data-ttu-id="7fad8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fad8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fad8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7fad8-127">Request body</span></span>
<span data-ttu-id="7fad8-128">В тексте запроса добавьте представление объекта Девицехеалсскриптдевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fad8-128">In the request body, supply a JSON representation for the deviceHealthScriptDeviceState object.</span></span>

<span data-ttu-id="7fad8-129">В следующей таблице приведены свойства, необходимые при создании Девицехеалсскриптдевицестате.</span><span class="sxs-lookup"><span data-stu-id="7fad8-129">The following table shows the properties that are required when you create the deviceHealthScriptDeviceState.</span></span>

|<span data-ttu-id="7fad8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fad8-130">Property</span></span>|<span data-ttu-id="7fad8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7fad8-131">Type</span></span>|<span data-ttu-id="7fad8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7fad8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fad8-133">id</span><span class="sxs-lookup"><span data-stu-id="7fad8-133">id</span></span>|<span data-ttu-id="7fad8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7fad8-134">String</span></span>|<span data-ttu-id="7fad8-135">Ключ объекта состояния устройства сценария работоспособности.</span><span class="sxs-lookup"><span data-stu-id="7fad8-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="7fad8-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fad8-136">This property is read-only.</span></span>|
|<span data-ttu-id="7fad8-137">детектионстате</span><span class="sxs-lookup"><span data-stu-id="7fad8-137">detectionState</span></span>|[<span data-ttu-id="7fad8-138">рунстате</span><span class="sxs-lookup"><span data-stu-id="7fad8-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="7fad8-139">Состояние обнаружения с последнего выполнения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="7fad8-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="7fad8-140">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="7fad8-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="7fad8-141">ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="7fad8-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="7fad8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fad8-142">DateTimeOffset</span></span>|<span data-ttu-id="7fad8-143">Последняя метка времени выполнения сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="7fad8-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="7fad8-144">експектедстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="7fad8-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="7fad8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fad8-145">DateTimeOffset</span></span>|<span data-ttu-id="7fad8-146">Следующий штамп времени, когда ожидается выполнение сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="7fad8-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="7fad8-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7fad8-147">lastSyncDateTime</span></span>|<span data-ttu-id="7fad8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fad8-148">DateTimeOffset</span></span>|<span data-ttu-id="7fad8-149">Время последнего синхронизации расширения управления Intune с Intune</span><span class="sxs-lookup"><span data-stu-id="7fad8-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="7fad8-150">преремедиатиондетектионскриптаутпут</span><span class="sxs-lookup"><span data-stu-id="7fad8-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="7fad8-151">Строка</span><span class="sxs-lookup"><span data-stu-id="7fad8-151">String</span></span>|<span data-ttu-id="7fad8-152">Выходные данные сценария обнаружения перед исправлением</span><span class="sxs-lookup"><span data-stu-id="7fad8-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="7fad8-153">преремедиатиондетектионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="7fad8-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="7fad8-154">Строка</span><span class="sxs-lookup"><span data-stu-id="7fad8-154">String</span></span>|<span data-ttu-id="7fad8-155">Ошибка сценария обнаружения перед исправлением</span><span class="sxs-lookup"><span data-stu-id="7fad8-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="7fad8-156">ремедиатионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="7fad8-156">remediationScriptError</span></span>|<span data-ttu-id="7fad8-157">Строка</span><span class="sxs-lookup"><span data-stu-id="7fad8-157">String</span></span>|<span data-ttu-id="7fad8-158">Вывод ошибок сценария исправления</span><span class="sxs-lookup"><span data-stu-id="7fad8-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="7fad8-159">постремедиатиондетектионскриптаутпут</span><span class="sxs-lookup"><span data-stu-id="7fad8-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="7fad8-160">Строка</span><span class="sxs-lookup"><span data-stu-id="7fad8-160">String</span></span>|<span data-ttu-id="7fad8-161">Выходные данные сценария обнаружения после исправления</span><span class="sxs-lookup"><span data-stu-id="7fad8-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="7fad8-162">постремедиатиондетектионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="7fad8-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="7fad8-163">Строка</span><span class="sxs-lookup"><span data-stu-id="7fad8-163">String</span></span>|<span data-ttu-id="7fad8-164">Ошибка сценария обнаружения после исправления</span><span class="sxs-lookup"><span data-stu-id="7fad8-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="7fad8-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="7fad8-165">remediationState</span></span>|[<span data-ttu-id="7fad8-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="7fad8-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="7fad8-167">Состояние исправления с последнего выполнения скрипта работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="7fad8-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="7fad8-168">Возможные значения: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span><span class="sxs-lookup"><span data-stu-id="7fad8-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="7fad8-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fad8-169">Response</span></span>
<span data-ttu-id="7fad8-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7fad8-170">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fad8-171">Пример</span><span class="sxs-lookup"><span data-stu-id="7fad8-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fad8-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fad8-172">Request</span></span>
<span data-ttu-id="7fad8-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fad8-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="7fad8-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fad8-174">Response</span></span>
<span data-ttu-id="7fad8-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7fad8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





