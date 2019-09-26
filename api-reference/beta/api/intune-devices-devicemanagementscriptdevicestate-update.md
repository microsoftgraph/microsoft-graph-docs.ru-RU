---
title: Обновление Девицеманажементскриптдевицестате
description: Обновление свойств объекта Девицеманажементскриптдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6bfb1dc79bd1162b2b05ddff35c3ea712db3ea97
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188558"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="44efc-103">Обновление Девицеманажементскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="44efc-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="44efc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44efc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44efc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44efc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44efc-106">Обновление свойств объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="44efc-106">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44efc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44efc-107">Prerequisites</span></span>
<span data-ttu-id="44efc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44efc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44efc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44efc-110">Permission type</span></span>|<span data-ttu-id="44efc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44efc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44efc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44efc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44efc-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44efc-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="44efc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44efc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44efc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44efc-115">Not supported.</span></span>|
|<span data-ttu-id="44efc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44efc-116">Application</span></span>|<span data-ttu-id="44efc-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44efc-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44efc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44efc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="44efc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44efc-119">Request headers</span></span>
|<span data-ttu-id="44efc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44efc-120">Header</span></span>|<span data-ttu-id="44efc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="44efc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44efc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44efc-122">Authorization</span></span>|<span data-ttu-id="44efc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44efc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44efc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="44efc-124">Accept</span></span>|<span data-ttu-id="44efc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44efc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44efc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44efc-126">Request body</span></span>
<span data-ttu-id="44efc-127">В тексте запроса добавьте представление объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44efc-127">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="44efc-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="44efc-128">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="44efc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="44efc-129">Property</span></span>|<span data-ttu-id="44efc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="44efc-130">Type</span></span>|<span data-ttu-id="44efc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="44efc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44efc-132">id</span><span class="sxs-lookup"><span data-stu-id="44efc-132">id</span></span>|<span data-ttu-id="44efc-133">String</span><span class="sxs-lookup"><span data-stu-id="44efc-133">String</span></span>|<span data-ttu-id="44efc-134">Ключ объекта состояния устройства сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="44efc-134">Key of the device management script device state entity.</span></span> <span data-ttu-id="44efc-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44efc-135">This property is read-only.</span></span>|
|<span data-ttu-id="44efc-136">рунстате</span><span class="sxs-lookup"><span data-stu-id="44efc-136">runState</span></span>|[<span data-ttu-id="44efc-137">рунстате</span><span class="sxs-lookup"><span data-stu-id="44efc-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="44efc-138">Состояние последнего запуска скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="44efc-138">State of latest run of the device management script.</span></span> <span data-ttu-id="44efc-139">Возможные значения: `unknown`, `success`, `fail`, `error`, `pending`.</span><span class="sxs-lookup"><span data-stu-id="44efc-139">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="44efc-140">ресултмессаже</span><span class="sxs-lookup"><span data-stu-id="44efc-140">resultMessage</span></span>|<span data-ttu-id="44efc-141">String.</span><span class="sxs-lookup"><span data-stu-id="44efc-141">String</span></span>|<span data-ttu-id="44efc-142">Сведения о выходных данных выполнения.</span><span class="sxs-lookup"><span data-stu-id="44efc-142">Details of execution output.</span></span>|
|<span data-ttu-id="44efc-143">ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="44efc-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="44efc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44efc-144">DateTimeOffset</span></span>|<span data-ttu-id="44efc-145">Последнее время выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="44efc-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="44efc-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="44efc-146">errorCode</span></span>|<span data-ttu-id="44efc-147">Int32</span><span class="sxs-lookup"><span data-stu-id="44efc-147">Int32</span></span>|<span data-ttu-id="44efc-148">Код ошибки, соответствующий ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="44efc-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="44efc-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="44efc-149">errorDescription</span></span>|<span data-ttu-id="44efc-150">String</span><span class="sxs-lookup"><span data-stu-id="44efc-150">String</span></span>|<span data-ttu-id="44efc-151">Описание ошибки, соответствующее ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="44efc-151">Error description corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="44efc-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="44efc-152">lastSyncDateTime</span></span>|<span data-ttu-id="44efc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44efc-153">DateTimeOffset</span></span>|<span data-ttu-id="44efc-154">Последнее время, когда расширение управления Intune будет синхронизироваться с Intune.</span><span class="sxs-lookup"><span data-stu-id="44efc-154">The latest time that Intune Managment Extension syncs to Intune.</span></span>|
|<span data-ttu-id="44efc-155">преремедиатиондетектионскриптаутпут</span><span class="sxs-lookup"><span data-stu-id="44efc-155">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="44efc-156">String.</span><span class="sxs-lookup"><span data-stu-id="44efc-156">String</span></span>|<span data-ttu-id="44efc-157">Выходные данные сценария обнаружения перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="44efc-157">Output of the detection script before remediation.</span></span>|
|<span data-ttu-id="44efc-158">ремедиатионскриптеррор</span><span class="sxs-lookup"><span data-stu-id="44efc-158">remediationScriptError</span></span>|<span data-ttu-id="44efc-159">String.</span><span class="sxs-lookup"><span data-stu-id="44efc-159">String</span></span>|<span data-ttu-id="44efc-160">Вывод ошибок сценария исправления.</span><span class="sxs-lookup"><span data-stu-id="44efc-160">Error output of the remediation script.</span></span>|
|<span data-ttu-id="44efc-161">постремедиатиондетектионскриптаутпут</span><span class="sxs-lookup"><span data-stu-id="44efc-161">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="44efc-162">String.</span><span class="sxs-lookup"><span data-stu-id="44efc-162">String</span></span>|<span data-ttu-id="44efc-163">Выходные данные сценария обнаружения после исправления.</span><span class="sxs-lookup"><span data-stu-id="44efc-163">Detection script output after remediation.</span></span>|



## <a name="response"></a><span data-ttu-id="44efc-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="44efc-164">Response</span></span>
<span data-ttu-id="44efc-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44efc-165">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44efc-166">Пример</span><span class="sxs-lookup"><span data-stu-id="44efc-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="44efc-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="44efc-167">Request</span></span>
<span data-ttu-id="44efc-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44efc-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value"
}
```

### <a name="response"></a><span data-ttu-id="44efc-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="44efc-169">Response</span></span>
<span data-ttu-id="44efc-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44efc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value"
}
```




