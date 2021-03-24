---
title: Обновление deviceComplianceScriptDeviceState
description: Обновление свойств объекта deviceComplianceScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d4f61c14eda8d1187acaab07d92975e07710ba5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130779"
---
# <a name="update-devicecompliancescriptdevicestate"></a><span data-ttu-id="f4661-103">Обновление deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="f4661-103">Update deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="f4661-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4661-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4661-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4661-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4661-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4661-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4661-107">Обновление свойств объекта [deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="f4661-107">Update the properties of a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4661-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4661-108">Prerequisites</span></span>
<span data-ttu-id="f4661-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4661-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4661-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4661-111">Permission type</span></span>|<span data-ttu-id="f4661-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4661-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4661-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4661-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4661-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4661-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f4661-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4661-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4661-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4661-116">Not supported.</span></span>|
|<span data-ttu-id="f4661-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f4661-117">Application</span></span>|<span data-ttu-id="f4661-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4661-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4661-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4661-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f4661-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f4661-120">Request headers</span></span>
|<span data-ttu-id="f4661-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4661-121">Header</span></span>|<span data-ttu-id="f4661-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4661-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4661-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4661-123">Authorization</span></span>|<span data-ttu-id="f4661-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4661-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4661-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4661-125">Accept</span></span>|<span data-ttu-id="f4661-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4661-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4661-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4661-127">Request body</span></span>
<span data-ttu-id="f4661-128">В корпусе запроса поставляем представление JSON для [объекта deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="f4661-128">In the request body, supply a JSON representation for the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

<span data-ttu-id="f4661-129">В следующей таблице показаны свойства, необходимые при создании [устройстваComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="f4661-129">The following table shows the properties that are required when you create the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span></span>

|<span data-ttu-id="f4661-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4661-130">Property</span></span>|<span data-ttu-id="f4661-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f4661-131">Type</span></span>|<span data-ttu-id="f4661-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f4661-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4661-133">id</span><span class="sxs-lookup"><span data-stu-id="f4661-133">id</span></span>|<span data-ttu-id="f4661-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f4661-134">String</span></span>|<span data-ttu-id="f4661-135">Ключ состояния состояния скрипта устройства устройства.</span><span class="sxs-lookup"><span data-stu-id="f4661-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="f4661-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4661-136">This property is read-only.</span></span>|
|<span data-ttu-id="f4661-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="f4661-137">detectionState</span></span>|[<span data-ttu-id="f4661-138">runState</span><span class="sxs-lookup"><span data-stu-id="f4661-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="f4661-139">Состояние обнаружения из последнего выполнения скрипта соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="f4661-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="f4661-140">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f4661-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="f4661-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f4661-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="f4661-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4661-142">DateTimeOffset</span></span>|<span data-ttu-id="f4661-143">Последний период выполнения сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="f4661-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="f4661-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f4661-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="f4661-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4661-145">DateTimeOffset</span></span>|<span data-ttu-id="f4661-146">Следующий период выполнения сценария соответствия требованиям к устройству</span><span class="sxs-lookup"><span data-stu-id="f4661-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="f4661-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f4661-147">lastSyncDateTime</span></span>|<span data-ttu-id="f4661-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4661-148">DateTimeOffset</span></span>|<span data-ttu-id="f4661-149">Последний раз, когда расширение управления Intune синхронизировали с Intune</span><span class="sxs-lookup"><span data-stu-id="f4661-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="f4661-150">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="f4661-150">scriptOutput</span></span>|<span data-ttu-id="f4661-151">Строка</span><span class="sxs-lookup"><span data-stu-id="f4661-151">String</span></span>|<span data-ttu-id="f4661-152">Выход сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="f4661-152">Output of the detection script</span></span>|
|<span data-ttu-id="f4661-153">scriptError</span><span class="sxs-lookup"><span data-stu-id="f4661-153">scriptError</span></span>|<span data-ttu-id="f4661-154">Строка</span><span class="sxs-lookup"><span data-stu-id="f4661-154">String</span></span>|<span data-ttu-id="f4661-155">Ошибка из сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="f4661-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="f4661-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4661-156">Response</span></span>
<span data-ttu-id="f4661-157">В случае успешного использования этот метод возвращает код отклика и обновленный объект `200 OK` [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f4661-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4661-158">Пример</span><span class="sxs-lookup"><span data-stu-id="f4661-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4661-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4661-159">Request</span></span>
<span data-ttu-id="f4661-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4661-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4661-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4661-161">Response</span></span>
<span data-ttu-id="f4661-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4661-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




