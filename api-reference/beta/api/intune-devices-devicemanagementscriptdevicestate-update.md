---
title: Обновление Девицеманажементскриптдевицестате
description: Обновление свойств объекта Девицеманажементскриптдевицестате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc964a5ee2f0ac5ba72ae2dad910a9c7e0c02d77
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762929"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="399e4-103">Обновление Девицеманажементскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="399e4-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="399e4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="399e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="399e4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="399e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="399e4-106">Обновление свойств объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="399e4-106">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="399e4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="399e4-107">Prerequisites</span></span>
<span data-ttu-id="399e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="399e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="399e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="399e4-110">Permission type</span></span>|<span data-ttu-id="399e4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="399e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="399e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="399e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="399e4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="399e4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="399e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="399e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="399e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="399e4-115">Not supported.</span></span>|
|<span data-ttu-id="399e4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="399e4-116">Application</span></span>|<span data-ttu-id="399e4-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="399e4-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="399e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="399e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="399e4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="399e4-119">Request headers</span></span>
|<span data-ttu-id="399e4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="399e4-120">Header</span></span>|<span data-ttu-id="399e4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="399e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="399e4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="399e4-122">Authorization</span></span>|<span data-ttu-id="399e4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="399e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="399e4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="399e4-124">Accept</span></span>|<span data-ttu-id="399e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="399e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="399e4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="399e4-126">Request body</span></span>
<span data-ttu-id="399e4-127">В тексте запроса добавьте представление объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="399e4-127">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="399e4-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="399e4-128">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="399e4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="399e4-129">Property</span></span>|<span data-ttu-id="399e4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="399e4-130">Type</span></span>|<span data-ttu-id="399e4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="399e4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="399e4-132">id</span><span class="sxs-lookup"><span data-stu-id="399e4-132">id</span></span>|<span data-ttu-id="399e4-133">String</span><span class="sxs-lookup"><span data-stu-id="399e4-133">String</span></span>|<span data-ttu-id="399e4-134">Ключ объекта состояния устройства сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="399e4-134">Key of the device management script device state entity.</span></span> <span data-ttu-id="399e4-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="399e4-135">This property is read-only.</span></span>|
|<span data-ttu-id="399e4-136">рунстате</span><span class="sxs-lookup"><span data-stu-id="399e4-136">runState</span></span>|[<span data-ttu-id="399e4-137">рунстате</span><span class="sxs-lookup"><span data-stu-id="399e4-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="399e4-138">Состояние последнего запуска скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="399e4-138">State of latest run of the device management script.</span></span> <span data-ttu-id="399e4-139">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="399e4-139">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="399e4-140">ресултмессаже</span><span class="sxs-lookup"><span data-stu-id="399e4-140">resultMessage</span></span>|<span data-ttu-id="399e4-141">String</span><span class="sxs-lookup"><span data-stu-id="399e4-141">String</span></span>|<span data-ttu-id="399e4-142">Сведения о выходных данных выполнения.</span><span class="sxs-lookup"><span data-stu-id="399e4-142">Details of execution output.</span></span>|
|<span data-ttu-id="399e4-143">ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="399e4-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="399e4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="399e4-144">DateTimeOffset</span></span>|<span data-ttu-id="399e4-145">Последнее время выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="399e4-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="399e4-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="399e4-146">errorCode</span></span>|<span data-ttu-id="399e4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="399e4-147">Int32</span></span>|<span data-ttu-id="399e4-148">Код ошибки, соответствующий ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="399e4-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="399e4-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="399e4-149">errorDescription</span></span>|<span data-ttu-id="399e4-150">String</span><span class="sxs-lookup"><span data-stu-id="399e4-150">String</span></span>|<span data-ttu-id="399e4-151">Описание ошибки, соответствующее ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="399e4-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="399e4-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="399e4-152">Response</span></span>
<span data-ttu-id="399e4-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="399e4-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="399e4-154">Пример</span><span class="sxs-lookup"><span data-stu-id="399e4-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="399e4-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="399e4-155">Request</span></span>
<span data-ttu-id="399e4-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="399e4-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```

### <a name="response"></a><span data-ttu-id="399e4-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="399e4-157">Response</span></span>
<span data-ttu-id="399e4-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="399e4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```




