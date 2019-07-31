---
title: Обновление Девицеманажементскриптдевицестате
description: Обновление свойств объекта Девицеманажементскриптдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db46807d376decdcbe81484ce097514af849efa7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986017"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="1af1b-103">Обновление Девицеманажементскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="1af1b-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="1af1b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1af1b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1af1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1af1b-106">Обновление свойств объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1af1b-106">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1af1b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1af1b-107">Prerequisites</span></span>
<span data-ttu-id="1af1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1af1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1af1b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1af1b-110">Permission type</span></span>|<span data-ttu-id="1af1b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1af1b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1af1b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1af1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1af1b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1af1b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1af1b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1af1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1af1b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af1b-115">Not supported.</span></span>|
|<span data-ttu-id="1af1b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1af1b-116">Application</span></span>|<span data-ttu-id="1af1b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af1b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1af1b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1af1b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="1af1b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1af1b-119">Request headers</span></span>
|<span data-ttu-id="1af1b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1af1b-120">Header</span></span>|<span data-ttu-id="1af1b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1af1b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1af1b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1af1b-122">Authorization</span></span>|<span data-ttu-id="1af1b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1af1b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1af1b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1af1b-124">Accept</span></span>|<span data-ttu-id="1af1b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1af1b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1af1b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1af1b-126">Request body</span></span>
<span data-ttu-id="1af1b-127">В тексте запроса добавьте представление объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1af1b-127">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="1af1b-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="1af1b-128">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="1af1b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1af1b-129">Property</span></span>|<span data-ttu-id="1af1b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1af1b-130">Type</span></span>|<span data-ttu-id="1af1b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1af1b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1af1b-132">id</span><span class="sxs-lookup"><span data-stu-id="1af1b-132">id</span></span>|<span data-ttu-id="1af1b-133">String</span><span class="sxs-lookup"><span data-stu-id="1af1b-133">String</span></span>|<span data-ttu-id="1af1b-134">Ключ объекта состояния устройства сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="1af1b-134">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="1af1b-135">Рунстате</span><span class="sxs-lookup"><span data-stu-id="1af1b-135">runState</span></span>|[<span data-ttu-id="1af1b-136">Рунстате</span><span class="sxs-lookup"><span data-stu-id="1af1b-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="1af1b-137">Состояние последнего запуска скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="1af1b-137">State of latest run of the device management script.</span></span> <span data-ttu-id="1af1b-138">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="1af1b-138">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="1af1b-139">Ресултмессаже</span><span class="sxs-lookup"><span data-stu-id="1af1b-139">resultMessage</span></span>|<span data-ttu-id="1af1b-140">String</span><span class="sxs-lookup"><span data-stu-id="1af1b-140">String</span></span>|<span data-ttu-id="1af1b-141">Сведения о выходных данных выполнения.</span><span class="sxs-lookup"><span data-stu-id="1af1b-141">Details of execution output.</span></span>|
|<span data-ttu-id="1af1b-142">Ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="1af1b-142">lastStateUpdateDateTime</span></span>|<span data-ttu-id="1af1b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1af1b-143">DateTimeOffset</span></span>|<span data-ttu-id="1af1b-144">Последнее время выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="1af1b-144">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="1af1b-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="1af1b-145">errorCode</span></span>|<span data-ttu-id="1af1b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1af1b-146">Int32</span></span>|<span data-ttu-id="1af1b-147">Код ошибки, соответствующий ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="1af1b-147">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="1af1b-148">errorDescription</span><span class="sxs-lookup"><span data-stu-id="1af1b-148">errorDescription</span></span>|<span data-ttu-id="1af1b-149">String</span><span class="sxs-lookup"><span data-stu-id="1af1b-149">String</span></span>|<span data-ttu-id="1af1b-150">Описание ошибки, соответствующее ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="1af1b-150">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="1af1b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="1af1b-151">Response</span></span>
<span data-ttu-id="1af1b-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1af1b-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1af1b-153">Пример</span><span class="sxs-lookup"><span data-stu-id="1af1b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1af1b-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="1af1b-154">Request</span></span>
<span data-ttu-id="1af1b-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1af1b-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="1af1b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="1af1b-156">Response</span></span>
<span data-ttu-id="1af1b-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1af1b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





