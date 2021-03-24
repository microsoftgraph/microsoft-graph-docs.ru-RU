---
title: Создание deviceHealthScriptDeviceState
description: Создание нового объекта deviceHealthScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a115878511d7d0317bc17bc38f88538de503b9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130737"
---
# <a name="create-devicehealthscriptdevicestate"></a><span data-ttu-id="dc46b-103">Создание deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="dc46b-103">Create deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="dc46b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc46b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc46b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc46b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc46b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc46b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc46b-107">Создание нового [объекта deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="dc46b-107">Create a new [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc46b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dc46b-108">Prerequisites</span></span>
<span data-ttu-id="dc46b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc46b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc46b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc46b-111">Permission type</span></span>|<span data-ttu-id="dc46b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc46b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc46b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc46b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc46b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc46b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc46b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc46b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc46b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc46b-116">Not supported.</span></span>|
|<span data-ttu-id="dc46b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dc46b-117">Application</span></span>|<span data-ttu-id="dc46b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc46b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc46b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc46b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="dc46b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dc46b-120">Request headers</span></span>
|<span data-ttu-id="dc46b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc46b-121">Header</span></span>|<span data-ttu-id="dc46b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dc46b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc46b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc46b-123">Authorization</span></span>|<span data-ttu-id="dc46b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc46b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc46b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc46b-125">Accept</span></span>|<span data-ttu-id="dc46b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc46b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc46b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc46b-127">Request body</span></span>
<span data-ttu-id="dc46b-128">В корпусе запроса поставляем представление JSON для объекта deviceHealthScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="dc46b-128">In the request body, supply a JSON representation for the deviceHealthScriptDeviceState object.</span></span>

<span data-ttu-id="dc46b-129">В следующей таблице показаны свойства, необходимые при создании устройстваHealthScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="dc46b-129">The following table shows the properties that are required when you create the deviceHealthScriptDeviceState.</span></span>

|<span data-ttu-id="dc46b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc46b-130">Property</span></span>|<span data-ttu-id="dc46b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dc46b-131">Type</span></span>|<span data-ttu-id="dc46b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dc46b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc46b-133">id</span><span class="sxs-lookup"><span data-stu-id="dc46b-133">id</span></span>|<span data-ttu-id="dc46b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dc46b-134">String</span></span>|<span data-ttu-id="dc46b-135">Ключ состояния состояния скрипта устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="dc46b-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="dc46b-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc46b-136">This property is read-only.</span></span>|
|<span data-ttu-id="dc46b-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="dc46b-137">detectionState</span></span>|[<span data-ttu-id="dc46b-138">runState</span><span class="sxs-lookup"><span data-stu-id="dc46b-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="dc46b-139">Состояние обнаружения из последнего выполнения скрипта для здоровья устройств.</span><span class="sxs-lookup"><span data-stu-id="dc46b-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="dc46b-140">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="dc46b-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="dc46b-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="dc46b-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="dc46b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc46b-142">DateTimeOffset</span></span>|<span data-ttu-id="dc46b-143">Последний период выполнения скрипта для здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="dc46b-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="dc46b-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="dc46b-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="dc46b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc46b-145">DateTimeOffset</span></span>|<span data-ttu-id="dc46b-146">Следующий период, когда ожидается выполнение сценария состояния устройства</span><span class="sxs-lookup"><span data-stu-id="dc46b-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="dc46b-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dc46b-147">lastSyncDateTime</span></span>|<span data-ttu-id="dc46b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc46b-148">DateTimeOffset</span></span>|<span data-ttu-id="dc46b-149">Последний раз, когда расширение управления Intune синхронизировали с Intune</span><span class="sxs-lookup"><span data-stu-id="dc46b-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="dc46b-150">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="dc46b-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="dc46b-151">Строка</span><span class="sxs-lookup"><span data-stu-id="dc46b-151">String</span></span>|<span data-ttu-id="dc46b-152">Выход сценария обнаружения перед исправлением</span><span class="sxs-lookup"><span data-stu-id="dc46b-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="dc46b-153">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="dc46b-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="dc46b-154">Строка</span><span class="sxs-lookup"><span data-stu-id="dc46b-154">String</span></span>|<span data-ttu-id="dc46b-155">Ошибка из сценария обнаружения перед исправлением</span><span class="sxs-lookup"><span data-stu-id="dc46b-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="dc46b-156">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="dc46b-156">remediationScriptError</span></span>|<span data-ttu-id="dc46b-157">Строка</span><span class="sxs-lookup"><span data-stu-id="dc46b-157">String</span></span>|<span data-ttu-id="dc46b-158">Выход ошибки сценария восстановления</span><span class="sxs-lookup"><span data-stu-id="dc46b-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="dc46b-159">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="dc46b-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="dc46b-160">Строка</span><span class="sxs-lookup"><span data-stu-id="dc46b-160">String</span></span>|<span data-ttu-id="dc46b-161">Вывод скрипта обнаружения после устранения</span><span class="sxs-lookup"><span data-stu-id="dc46b-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="dc46b-162">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="dc46b-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="dc46b-163">Строка</span><span class="sxs-lookup"><span data-stu-id="dc46b-163">String</span></span>|<span data-ttu-id="dc46b-164">Ошибка из сценария обнаружения после устранения</span><span class="sxs-lookup"><span data-stu-id="dc46b-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="dc46b-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="dc46b-165">remediationState</span></span>|[<span data-ttu-id="dc46b-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="dc46b-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="dc46b-167">Состояние исправлений из последнего выполнения скрипта для здоровья устройств.</span><span class="sxs-lookup"><span data-stu-id="dc46b-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="dc46b-168">Возможные значения: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span><span class="sxs-lookup"><span data-stu-id="dc46b-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="dc46b-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc46b-169">Response</span></span>
<span data-ttu-id="dc46b-170">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dc46b-170">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc46b-171">Пример</span><span class="sxs-lookup"><span data-stu-id="dc46b-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc46b-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc46b-172">Request</span></span>
<span data-ttu-id="dc46b-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc46b-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc46b-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc46b-174">Response</span></span>
<span data-ttu-id="dc46b-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc46b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




