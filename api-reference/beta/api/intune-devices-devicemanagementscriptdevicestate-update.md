---
title: Обновление deviceManagementScriptDeviceState
description: Обновление свойства объекта deviceManagementScriptDeviceState.
ms.openlocfilehash: 790b13615d9f00d1e8441f444aeb0340454de098
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078294"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="48644-103">Обновление deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="48644-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="48644-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48644-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48644-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48644-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48644-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="48644-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48644-107">Обновление свойства объекта [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="48644-107">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48644-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="48644-108">Prerequisites</span></span>
<span data-ttu-id="48644-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48644-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48644-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48644-111">Permission type</span></span>|<span data-ttu-id="48644-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48644-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48644-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48644-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48644-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48644-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="48644-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48644-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48644-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48644-116">Not supported.</span></span>|
|<span data-ttu-id="48644-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48644-117">Application</span></span>|<span data-ttu-id="48644-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48644-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48644-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48644-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="48644-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48644-120">Request headers</span></span>
|<span data-ttu-id="48644-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48644-121">Header</span></span>|<span data-ttu-id="48644-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48644-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48644-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48644-123">Authorization</span></span>|<span data-ttu-id="48644-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="48644-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48644-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48644-125">Accept</span></span>|<span data-ttu-id="48644-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48644-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48644-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48644-127">Request body</span></span>
<span data-ttu-id="48644-128">В тексте запроса укажите представление JSON для объекта [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="48644-128">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="48644-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="48644-129">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="48644-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="48644-130">Property</span></span>|<span data-ttu-id="48644-131">Тип</span><span class="sxs-lookup"><span data-stu-id="48644-131">Type</span></span>|<span data-ttu-id="48644-132">Описание</span><span class="sxs-lookup"><span data-stu-id="48644-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48644-133">id</span><span class="sxs-lookup"><span data-stu-id="48644-133">id</span></span>|<span data-ttu-id="48644-134">String</span><span class="sxs-lookup"><span data-stu-id="48644-134">String</span></span>|<span data-ttu-id="48644-135">Ключ сущности состояния устройства устройства управления скрипта.</span><span class="sxs-lookup"><span data-stu-id="48644-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="48644-136">runState</span><span class="sxs-lookup"><span data-stu-id="48644-136">runState</span></span>|[<span data-ttu-id="48644-137">runState</span><span class="sxs-lookup"><span data-stu-id="48644-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="48644-138">Состояние последнего выполнения сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="48644-138">State of latest run of the device management script.</span></span> <span data-ttu-id="48644-139">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="48644-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="48644-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="48644-140">resultMessage</span></span>|<span data-ttu-id="48644-141">String</span><span class="sxs-lookup"><span data-stu-id="48644-141">String</span></span>|<span data-ttu-id="48644-142">Подробные сведения о результатов выполнения.</span><span class="sxs-lookup"><span data-stu-id="48644-142">Details of execution output.</span></span>|
|<span data-ttu-id="48644-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="48644-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="48644-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48644-144">DateTimeOffset</span></span>|<span data-ttu-id="48644-145">Время последнего выполняет сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="48644-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="48644-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="48644-146">errorCode</span></span>|<span data-ttu-id="48644-147">Int32</span><span class="sxs-lookup"><span data-stu-id="48644-147">Int32</span></span>|<span data-ttu-id="48644-148">Код ошибки, соответствующий ошибочный выполнение сценария управления устройства.</span><span class="sxs-lookup"><span data-stu-id="48644-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="48644-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="48644-149">errorDescription</span></span>|<span data-ttu-id="48644-150">String</span><span class="sxs-lookup"><span data-stu-id="48644-150">String</span></span>|<span data-ttu-id="48644-151">Описание ошибки, соответствующий ошибочный выполнение сценария управления устройства.</span><span class="sxs-lookup"><span data-stu-id="48644-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="48644-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="48644-152">Response</span></span>
<span data-ttu-id="48644-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48644-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48644-154">Пример</span><span class="sxs-lookup"><span data-stu-id="48644-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="48644-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="48644-155">Request</span></span>
<span data-ttu-id="48644-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48644-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
Content-type: application/json
Content-length: 209

{
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```

### <a name="response"></a><span data-ttu-id="48644-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="48644-157">Response</span></span>
<span data-ttu-id="48644-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="48644-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





