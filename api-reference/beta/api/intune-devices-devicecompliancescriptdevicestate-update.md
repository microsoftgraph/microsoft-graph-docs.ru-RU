---
title: Обновление Девицекомплианцескриптдевицестате
description: Обновление свойств объекта Девицекомплианцескриптдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c961a524f77f0a72c97c6f4b9967089ef5ea8806
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49310883"
---
# <a name="update-devicecompliancescriptdevicestate"></a><span data-ttu-id="8f383-103">Обновление Девицекомплианцескриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="8f383-103">Update deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="8f383-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f383-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f383-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f383-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f383-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f383-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f383-107">Обновление свойств объекта [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="8f383-107">Update the properties of a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f383-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8f383-108">Prerequisites</span></span>
<span data-ttu-id="8f383-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f383-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f383-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f383-111">Permission type</span></span>|<span data-ttu-id="8f383-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f383-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f383-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f383-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f383-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f383-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8f383-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f383-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f383-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f383-116">Not supported.</span></span>|
|<span data-ttu-id="8f383-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f383-117">Application</span></span>|<span data-ttu-id="8f383-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f383-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f383-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f383-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="8f383-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8f383-120">Request headers</span></span>
|<span data-ttu-id="8f383-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f383-121">Header</span></span>|<span data-ttu-id="8f383-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8f383-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f383-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f383-123">Authorization</span></span>|<span data-ttu-id="8f383-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f383-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f383-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f383-125">Accept</span></span>|<span data-ttu-id="8f383-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f383-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f383-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f383-127">Request body</span></span>
<span data-ttu-id="8f383-128">В тексте запроса добавьте представление объекта [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f383-128">In the request body, supply a JSON representation for the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

<span data-ttu-id="8f383-129">В следующей таблице приведены свойства, необходимые при создании [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="8f383-129">The following table shows the properties that are required when you create the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span></span>

|<span data-ttu-id="8f383-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f383-130">Property</span></span>|<span data-ttu-id="8f383-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f383-131">Type</span></span>|<span data-ttu-id="8f383-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f383-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f383-133">id</span><span class="sxs-lookup"><span data-stu-id="8f383-133">id</span></span>|<span data-ttu-id="8f383-134">String</span><span class="sxs-lookup"><span data-stu-id="8f383-134">String</span></span>|<span data-ttu-id="8f383-135">Ключ объекта состояния "сценарий соответствия требованиям устройства".</span><span class="sxs-lookup"><span data-stu-id="8f383-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="8f383-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f383-136">This property is read-only.</span></span>|
|<span data-ttu-id="8f383-137">детектионстате</span><span class="sxs-lookup"><span data-stu-id="8f383-137">detectionState</span></span>|[<span data-ttu-id="8f383-138">рунстате</span><span class="sxs-lookup"><span data-stu-id="8f383-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="8f383-139">Состояние обнаружения с последнего выполнения скрипта соответствия устройств требованиям.</span><span class="sxs-lookup"><span data-stu-id="8f383-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="8f383-140">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="8f383-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="8f383-141">ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="8f383-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="8f383-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f383-142">DateTimeOffset</span></span>|<span data-ttu-id="8f383-143">Последняя метка времени выполнения сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="8f383-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="8f383-144">експектедстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="8f383-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="8f383-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f383-145">DateTimeOffset</span></span>|<span data-ttu-id="8f383-146">Следующий штамп времени, когда ожидается выполнение сценария соответствия устройства</span><span class="sxs-lookup"><span data-stu-id="8f383-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="8f383-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8f383-147">lastSyncDateTime</span></span>|<span data-ttu-id="8f383-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f383-148">DateTimeOffset</span></span>|<span data-ttu-id="8f383-149">Время последнего синхронизации расширения управления Intune с Intune</span><span class="sxs-lookup"><span data-stu-id="8f383-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="8f383-150">скриптаутпут</span><span class="sxs-lookup"><span data-stu-id="8f383-150">scriptOutput</span></span>|<span data-ttu-id="8f383-151">String</span><span class="sxs-lookup"><span data-stu-id="8f383-151">String</span></span>|<span data-ttu-id="8f383-152">Выходные данные сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="8f383-152">Output of the detection script</span></span>|
|<span data-ttu-id="8f383-153">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="8f383-153">scriptError</span></span>|<span data-ttu-id="8f383-154">String</span><span class="sxs-lookup"><span data-stu-id="8f383-154">String</span></span>|<span data-ttu-id="8f383-155">Ошибка сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="8f383-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="8f383-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f383-156">Response</span></span>
<span data-ttu-id="8f383-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f383-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f383-158">Пример</span><span class="sxs-lookup"><span data-stu-id="8f383-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f383-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f383-159">Request</span></span>
<span data-ttu-id="8f383-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f383-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8f383-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f383-161">Response</span></span>
<span data-ttu-id="8f383-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f383-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




