---
title: Создание Девицеманажементскриптдевицестате
description: Создание нового объекта Девицеманажементскриптдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 35417b26989f5343784c26e21cea09d21b4623a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088099"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="e45d4-103">Создание Девицеманажементскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="e45d4-103">Create deviceManagementScriptDeviceState</span></span>

<span data-ttu-id="e45d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e45d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e45d4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e45d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e45d4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e45d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e45d4-107">Создание нового объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="e45d4-107">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e45d4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e45d4-108">Prerequisites</span></span>
<span data-ttu-id="e45d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e45d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e45d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e45d4-111">Permission type</span></span>|<span data-ttu-id="e45d4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e45d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e45d4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e45d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e45d4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45d4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e45d4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e45d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e45d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e45d4-116">Not supported.</span></span>|
|<span data-ttu-id="e45d4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e45d4-117">Application</span></span>|<span data-ttu-id="e45d4-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45d4-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e45d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e45d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="e45d4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e45d4-120">Request headers</span></span>
|<span data-ttu-id="e45d4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e45d4-121">Header</span></span>|<span data-ttu-id="e45d4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e45d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e45d4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e45d4-123">Authorization</span></span>|<span data-ttu-id="e45d4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e45d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e45d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e45d4-125">Accept</span></span>|<span data-ttu-id="e45d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e45d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e45d4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e45d4-127">Request body</span></span>
<span data-ttu-id="e45d4-128">В тексте запроса добавьте представление объекта Девицеманажементскриптдевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e45d4-128">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="e45d4-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементскриптдевицестате.</span><span class="sxs-lookup"><span data-stu-id="e45d4-129">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="e45d4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e45d4-130">Property</span></span>|<span data-ttu-id="e45d4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e45d4-131">Type</span></span>|<span data-ttu-id="e45d4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e45d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45d4-133">id</span><span class="sxs-lookup"><span data-stu-id="e45d4-133">id</span></span>|<span data-ttu-id="e45d4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e45d4-134">String</span></span>|<span data-ttu-id="e45d4-135">Ключ объекта состояния устройства сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e45d4-135">Key of the device management script device state entity.</span></span> <span data-ttu-id="e45d4-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e45d4-136">This property is read-only.</span></span>|
|<span data-ttu-id="e45d4-137">рунстате</span><span class="sxs-lookup"><span data-stu-id="e45d4-137">runState</span></span>|[<span data-ttu-id="e45d4-138">рунстате</span><span class="sxs-lookup"><span data-stu-id="e45d4-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="e45d4-139">Состояние последнего запуска скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e45d4-139">State of latest run of the device management script.</span></span> <span data-ttu-id="e45d4-140">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e45d4-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="e45d4-141">ресултмессаже</span><span class="sxs-lookup"><span data-stu-id="e45d4-141">resultMessage</span></span>|<span data-ttu-id="e45d4-142">Строка</span><span class="sxs-lookup"><span data-stu-id="e45d4-142">String</span></span>|<span data-ttu-id="e45d4-143">Сведения о выходных данных выполнения.</span><span class="sxs-lookup"><span data-stu-id="e45d4-143">Details of execution output.</span></span>|
|<span data-ttu-id="e45d4-144">ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="e45d4-144">lastStateUpdateDateTime</span></span>|<span data-ttu-id="e45d4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e45d4-145">DateTimeOffset</span></span>|<span data-ttu-id="e45d4-146">Последнее время выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e45d4-146">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="e45d4-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="e45d4-147">errorCode</span></span>|<span data-ttu-id="e45d4-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e45d4-148">Int32</span></span>|<span data-ttu-id="e45d4-149">Код ошибки, соответствующий ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e45d4-149">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="e45d4-150">errorDescription</span><span class="sxs-lookup"><span data-stu-id="e45d4-150">errorDescription</span></span>|<span data-ttu-id="e45d4-151">String</span><span class="sxs-lookup"><span data-stu-id="e45d4-151">String</span></span>|<span data-ttu-id="e45d4-152">Описание ошибки, соответствующее ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e45d4-152">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="e45d4-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e45d4-153">Response</span></span>
<span data-ttu-id="e45d4-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e45d4-154">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e45d4-155">Пример</span><span class="sxs-lookup"><span data-stu-id="e45d4-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="e45d4-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="e45d4-156">Request</span></span>
<span data-ttu-id="e45d4-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e45d4-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="e45d4-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="e45d4-158">Response</span></span>
<span data-ttu-id="e45d4-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e45d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






