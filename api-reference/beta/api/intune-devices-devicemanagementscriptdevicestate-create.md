---
title: Создание Девицеманажементскриптдевицестате
description: Создание нового объекта Девицеманажементскриптдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dfd0b21906cd7692e32b93475efdb8b861ed44b3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37530617"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="cf36d-103">Создание Девицеманажементскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="cf36d-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="cf36d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf36d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf36d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf36d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf36d-106">Создание нового объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="cf36d-106">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf36d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf36d-107">Prerequisites</span></span>
<span data-ttu-id="cf36d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf36d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf36d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf36d-110">Permission type</span></span>|<span data-ttu-id="cf36d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf36d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf36d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf36d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf36d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf36d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cf36d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf36d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf36d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf36d-115">Not supported.</span></span>|
|<span data-ttu-id="cf36d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cf36d-116">Application</span></span>|<span data-ttu-id="cf36d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf36d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf36d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf36d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="cf36d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf36d-119">Request headers</span></span>
|<span data-ttu-id="cf36d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf36d-120">Header</span></span>|<span data-ttu-id="cf36d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cf36d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf36d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf36d-122">Authorization</span></span>|<span data-ttu-id="cf36d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf36d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf36d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cf36d-124">Accept</span></span>|<span data-ttu-id="cf36d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf36d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf36d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf36d-126">Request body</span></span>
<span data-ttu-id="cf36d-127">В тексте запроса добавьте представление объекта Девицеманажементскриптдевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf36d-127">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="cf36d-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементскриптдевицестате.</span><span class="sxs-lookup"><span data-stu-id="cf36d-128">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="cf36d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf36d-129">Property</span></span>|<span data-ttu-id="cf36d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cf36d-130">Type</span></span>|<span data-ttu-id="cf36d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cf36d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf36d-132">id</span><span class="sxs-lookup"><span data-stu-id="cf36d-132">id</span></span>|<span data-ttu-id="cf36d-133">String</span><span class="sxs-lookup"><span data-stu-id="cf36d-133">String</span></span>|<span data-ttu-id="cf36d-134">Ключ объекта состояния устройства сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cf36d-134">Key of the device management script device state entity.</span></span> <span data-ttu-id="cf36d-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf36d-135">This property is read-only.</span></span>|
|<span data-ttu-id="cf36d-136">рунстате</span><span class="sxs-lookup"><span data-stu-id="cf36d-136">runState</span></span>|[<span data-ttu-id="cf36d-137">рунстате</span><span class="sxs-lookup"><span data-stu-id="cf36d-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="cf36d-138">Состояние последнего запуска скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cf36d-138">State of latest run of the device management script.</span></span> <span data-ttu-id="cf36d-139">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="cf36d-139">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="cf36d-140">ресултмессаже</span><span class="sxs-lookup"><span data-stu-id="cf36d-140">resultMessage</span></span>|<span data-ttu-id="cf36d-141">String</span><span class="sxs-lookup"><span data-stu-id="cf36d-141">String</span></span>|<span data-ttu-id="cf36d-142">Сведения о выходных данных выполнения.</span><span class="sxs-lookup"><span data-stu-id="cf36d-142">Details of execution output.</span></span>|
|<span data-ttu-id="cf36d-143">ластстатеупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="cf36d-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="cf36d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf36d-144">DateTimeOffset</span></span>|<span data-ttu-id="cf36d-145">Последнее время выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cf36d-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="cf36d-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="cf36d-146">errorCode</span></span>|<span data-ttu-id="cf36d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="cf36d-147">Int32</span></span>|<span data-ttu-id="cf36d-148">Код ошибки, соответствующий ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cf36d-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="cf36d-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="cf36d-149">errorDescription</span></span>|<span data-ttu-id="cf36d-150">String</span><span class="sxs-lookup"><span data-stu-id="cf36d-150">String</span></span>|<span data-ttu-id="cf36d-151">Описание ошибки, соответствующее ошибочному выполнению сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cf36d-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="cf36d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf36d-152">Response</span></span>
<span data-ttu-id="cf36d-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf36d-153">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf36d-154">Пример</span><span class="sxs-lookup"><span data-stu-id="cf36d-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf36d-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf36d-155">Request</span></span>
<span data-ttu-id="cf36d-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf36d-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="cf36d-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf36d-157">Response</span></span>
<span data-ttu-id="cf36d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf36d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






