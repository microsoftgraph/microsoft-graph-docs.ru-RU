---
title: Создание deviceComplianceScriptDeviceState
description: Создание нового объекта deviceComplianceScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0dcb977cc83eedeab5c0a8f8ac1cb3ccc96d8f32
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611855"
---
# <a name="create-devicecompliancescriptdevicestate"></a><span data-ttu-id="03695-103">Создание deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="03695-103">Create deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="03695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03695-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03695-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03695-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03695-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03695-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03695-107">Создание нового [объекта deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="03695-107">Create a new [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03695-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03695-108">Prerequisites</span></span>
<span data-ttu-id="03695-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03695-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03695-111">Permission type</span></span>|<span data-ttu-id="03695-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03695-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03695-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03695-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03695-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03695-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03695-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03695-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03695-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03695-116">Not supported.</span></span>|
|<span data-ttu-id="03695-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="03695-117">Application</span></span>|<span data-ttu-id="03695-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03695-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03695-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03695-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="03695-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03695-120">Request headers</span></span>
|<span data-ttu-id="03695-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03695-121">Header</span></span>|<span data-ttu-id="03695-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03695-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03695-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03695-123">Authorization</span></span>|<span data-ttu-id="03695-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03695-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03695-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03695-125">Accept</span></span>|<span data-ttu-id="03695-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03695-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03695-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03695-127">Request body</span></span>
<span data-ttu-id="03695-128">В корпусе запроса поставляем представление JSON для объекта deviceComplianceScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="03695-128">In the request body, supply a JSON representation for the deviceComplianceScriptDeviceState object.</span></span>

<span data-ttu-id="03695-129">В следующей таблице показаны свойства, необходимые при создании устройстваComplianceScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="03695-129">The following table shows the properties that are required when you create the deviceComplianceScriptDeviceState.</span></span>

|<span data-ttu-id="03695-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="03695-130">Property</span></span>|<span data-ttu-id="03695-131">Тип</span><span class="sxs-lookup"><span data-stu-id="03695-131">Type</span></span>|<span data-ttu-id="03695-132">Описание</span><span class="sxs-lookup"><span data-stu-id="03695-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03695-133">id</span><span class="sxs-lookup"><span data-stu-id="03695-133">id</span></span>|<span data-ttu-id="03695-134">String</span><span class="sxs-lookup"><span data-stu-id="03695-134">String</span></span>|<span data-ttu-id="03695-135">Ключ состояния состояния скрипта устройства устройства.</span><span class="sxs-lookup"><span data-stu-id="03695-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="03695-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03695-136">This property is read-only.</span></span>|
|<span data-ttu-id="03695-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="03695-137">detectionState</span></span>|[<span data-ttu-id="03695-138">runState</span><span class="sxs-lookup"><span data-stu-id="03695-138">runState</span></span>](../resources/intune-devices-runstate.md)|<span data-ttu-id="03695-139">Состояние обнаружения из последнего выполнения скрипта соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="03695-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="03695-140">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="03695-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="03695-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="03695-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="03695-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03695-142">DateTimeOffset</span></span>|<span data-ttu-id="03695-143">Последний период выполнения сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="03695-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="03695-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="03695-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="03695-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03695-145">DateTimeOffset</span></span>|<span data-ttu-id="03695-146">Следующий период выполнения сценария соответствия требованиям к устройству</span><span class="sxs-lookup"><span data-stu-id="03695-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="03695-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="03695-147">lastSyncDateTime</span></span>|<span data-ttu-id="03695-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03695-148">DateTimeOffset</span></span>|<span data-ttu-id="03695-149">Последний раз, когда расширение управления Intune синхронизировали с Intune</span><span class="sxs-lookup"><span data-stu-id="03695-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="03695-150">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="03695-150">scriptOutput</span></span>|<span data-ttu-id="03695-151">String</span><span class="sxs-lookup"><span data-stu-id="03695-151">String</span></span>|<span data-ttu-id="03695-152">Выход сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="03695-152">Output of the detection script</span></span>|
|<span data-ttu-id="03695-153">scriptError</span><span class="sxs-lookup"><span data-stu-id="03695-153">scriptError</span></span>|<span data-ttu-id="03695-154">String</span><span class="sxs-lookup"><span data-stu-id="03695-154">String</span></span>|<span data-ttu-id="03695-155">Ошибка из сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="03695-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="03695-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="03695-156">Response</span></span>
<span data-ttu-id="03695-157">В случае успешного использования этот метод возвращает код отклика и `201 Created` [объект deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="03695-157">If successful, this method returns a `201 Created` response code and a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03695-158">Пример</span><span class="sxs-lookup"><span data-stu-id="03695-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="03695-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="03695-159">Request</span></span>
<span data-ttu-id="03695-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03695-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="03695-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="03695-161">Response</span></span>
<span data-ttu-id="03695-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03695-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




