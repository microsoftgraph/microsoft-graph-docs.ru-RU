---
title: Обновление Девицекомплианцескриптдевицестате
description: Обновление свойств объекта Девицекомплианцескриптдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2506199946b3b80c983c84486cb3b6de4a209494
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792445"
---
# <a name="update-devicecompliancescriptdevicestate"></a><span data-ttu-id="cdad9-103">Обновление Девицекомплианцескриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="cdad9-103">Update deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="cdad9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdad9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdad9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdad9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdad9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdad9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdad9-107">Обновление свойств объекта [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="cdad9-107">Update the properties of a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdad9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cdad9-108">Prerequisites</span></span>
<span data-ttu-id="cdad9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="cdad9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cdad9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdad9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdad9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdad9-111">Permission type</span></span>|<span data-ttu-id="cdad9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdad9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdad9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdad9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdad9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdad9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cdad9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdad9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdad9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdad9-116">Not supported.</span></span>|
|<span data-ttu-id="cdad9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdad9-117">Application</span></span>|<span data-ttu-id="cdad9-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdad9-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdad9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdad9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="cdad9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cdad9-120">Request headers</span></span>
|<span data-ttu-id="cdad9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdad9-121">Header</span></span>|<span data-ttu-id="cdad9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cdad9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdad9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdad9-123">Authorization</span></span>|<span data-ttu-id="cdad9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdad9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdad9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cdad9-125">Accept</span></span>|<span data-ttu-id="cdad9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdad9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdad9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cdad9-127">Request body</span></span>
<span data-ttu-id="cdad9-128">В тексте запроса добавьте представление объекта [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdad9-128">In the request body, supply a JSON representation for the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

<span data-ttu-id="cdad9-129">В следующей таблице приведены свойства, необходимые при создании [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="cdad9-129">The following table shows the properties that are required when you create the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span></span>

|<span data-ttu-id="cdad9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdad9-130">Property</span></span>|<span data-ttu-id="cdad9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cdad9-131">Type</span></span>|<span data-ttu-id="cdad9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cdad9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdad9-133">id</span><span class="sxs-lookup"><span data-stu-id="cdad9-133">id</span></span>|<span data-ttu-id="cdad9-134">String</span><span class="sxs-lookup"><span data-stu-id="cdad9-134">String</span></span>|<span data-ttu-id="cdad9-135">Ключ объекта состояния "сценарий соответствия требованиям устройства".</span><span class="sxs-lookup"><span data-stu-id="cdad9-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="cdad9-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdad9-136">This property is read-only.</span></span>|
|<span data-ttu-id="cdad9-137">детектионстате</span><span class="sxs-lookup"><span data-stu-id="cdad9-137">detectionState</span></span>|[<span data-ttu-id="cdad9-138">рунстате</span><span class="sxs-lookup"><span data-stu-id="cdad9-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="cdad9-139">Состояние обнаружения с последнего выполнения скрипта соответствия устройств требованиям.</span><span class="sxs-lookup"><span data-stu-id="cdad9-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="cdad9-140">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="cdad9-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="cdad9-141">ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="cdad9-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="cdad9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdad9-142">DateTimeOffset</span></span>|<span data-ttu-id="cdad9-143">Последняя метка времени выполнения сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="cdad9-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="cdad9-144">експектедстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="cdad9-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="cdad9-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdad9-145">DateTimeOffset</span></span>|<span data-ttu-id="cdad9-146">Следующий штамп времени, когда ожидается выполнение сценария соответствия устройства</span><span class="sxs-lookup"><span data-stu-id="cdad9-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="cdad9-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cdad9-147">lastSyncDateTime</span></span>|<span data-ttu-id="cdad9-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdad9-148">DateTimeOffset</span></span>|<span data-ttu-id="cdad9-149">Время последнего синхронизации расширения управления Intune с Intune</span><span class="sxs-lookup"><span data-stu-id="cdad9-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="cdad9-150">скриптаутпут</span><span class="sxs-lookup"><span data-stu-id="cdad9-150">scriptOutput</span></span>|<span data-ttu-id="cdad9-151">String</span><span class="sxs-lookup"><span data-stu-id="cdad9-151">String</span></span>|<span data-ttu-id="cdad9-152">Выходные данные сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="cdad9-152">Output of the detection script</span></span>|
|<span data-ttu-id="cdad9-153">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="cdad9-153">scriptError</span></span>|<span data-ttu-id="cdad9-154">String</span><span class="sxs-lookup"><span data-stu-id="cdad9-154">String</span></span>|<span data-ttu-id="cdad9-155">Ошибка сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="cdad9-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="cdad9-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdad9-156">Response</span></span>
<span data-ttu-id="cdad9-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdad9-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdad9-158">Пример</span><span class="sxs-lookup"><span data-stu-id="cdad9-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdad9-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdad9-159">Request</span></span>
<span data-ttu-id="cdad9-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdad9-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
Content-type: application/json
Content-length: 387

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "scriptOutput": "Script Output value",
  "scriptError": "Script Error value"
}
```

### <a name="response"></a><span data-ttu-id="cdad9-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdad9-161">Response</span></span>
<span data-ttu-id="cdad9-162">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="cdad9-162">Here is an example of the response.</span></span> <span data-ttu-id="cdad9-163">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="cdad9-163">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cdad9-164">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="cdad9-164">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 436

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "id": "7bd39c86-9c86-7bd3-869c-d37b869cd37b",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "scriptOutput": "Script Output value",
  "scriptError": "Script Error value"
}
```



