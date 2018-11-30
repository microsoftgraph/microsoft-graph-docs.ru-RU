---
title: Создание deviceManagementScriptDeviceState
description: Создание нового объекта deviceManagementScriptDeviceState.
ms.openlocfilehash: 64594aee75d398fb92a0b7150a07409aa4362126
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079477"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="af365-103">Создание deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="af365-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="af365-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="af365-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af365-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af365-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af365-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="af365-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af365-107">Создание нового объекта [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="af365-107">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af365-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="af365-108">Prerequisites</span></span>
<span data-ttu-id="af365-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af365-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af365-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af365-111">Permission type</span></span>|<span data-ttu-id="af365-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af365-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af365-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af365-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af365-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af365-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="af365-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af365-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af365-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af365-116">Not supported.</span></span>|
|<span data-ttu-id="af365-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af365-117">Application</span></span>|<span data-ttu-id="af365-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af365-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af365-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af365-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="af365-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af365-120">Request headers</span></span>
|<span data-ttu-id="af365-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af365-121">Header</span></span>|<span data-ttu-id="af365-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af365-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af365-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af365-123">Authorization</span></span>|<span data-ttu-id="af365-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="af365-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af365-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af365-125">Accept</span></span>|<span data-ttu-id="af365-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af365-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af365-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af365-127">Request body</span></span>
<span data-ttu-id="af365-128">В тексте запроса укажите представление JSON для объекта deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="af365-128">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="af365-129">В следующей таблице показаны свойства, которые необходимы для создания deviceManagementScriptDeviceState.</span><span class="sxs-lookup"><span data-stu-id="af365-129">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="af365-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="af365-130">Property</span></span>|<span data-ttu-id="af365-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af365-131">Type</span></span>|<span data-ttu-id="af365-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af365-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af365-133">id</span><span class="sxs-lookup"><span data-stu-id="af365-133">id</span></span>|<span data-ttu-id="af365-134">String</span><span class="sxs-lookup"><span data-stu-id="af365-134">String</span></span>|<span data-ttu-id="af365-135">Ключ сущности состояния устройства устройства управления скрипта.</span><span class="sxs-lookup"><span data-stu-id="af365-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="af365-136">runState</span><span class="sxs-lookup"><span data-stu-id="af365-136">runState</span></span>|[<span data-ttu-id="af365-137">runState</span><span class="sxs-lookup"><span data-stu-id="af365-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="af365-138">Состояние последнего выполнения сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="af365-138">State of latest run of the device management script.</span></span> <span data-ttu-id="af365-139">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="af365-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="af365-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="af365-140">resultMessage</span></span>|<span data-ttu-id="af365-141">String</span><span class="sxs-lookup"><span data-stu-id="af365-141">String</span></span>|<span data-ttu-id="af365-142">Подробные сведения о результатов выполнения.</span><span class="sxs-lookup"><span data-stu-id="af365-142">Details of execution output.</span></span>|
|<span data-ttu-id="af365-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="af365-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="af365-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af365-144">DateTimeOffset</span></span>|<span data-ttu-id="af365-145">Время последнего выполняет сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="af365-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="af365-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="af365-146">errorCode</span></span>|<span data-ttu-id="af365-147">Int32</span><span class="sxs-lookup"><span data-stu-id="af365-147">Int32</span></span>|<span data-ttu-id="af365-148">Код ошибки, соответствующий ошибочный выполнение сценария управления устройства.</span><span class="sxs-lookup"><span data-stu-id="af365-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="af365-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="af365-149">errorDescription</span></span>|<span data-ttu-id="af365-150">String</span><span class="sxs-lookup"><span data-stu-id="af365-150">String</span></span>|<span data-ttu-id="af365-151">Описание ошибки, соответствующий ошибочный выполнение сценария управления устройства.</span><span class="sxs-lookup"><span data-stu-id="af365-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="af365-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="af365-152">Response</span></span>
<span data-ttu-id="af365-153">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="af365-153">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af365-154">Пример</span><span class="sxs-lookup"><span data-stu-id="af365-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="af365-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="af365-155">Request</span></span>
<span data-ttu-id="af365-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af365-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af365-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="af365-157">Response</span></span>
<span data-ttu-id="af365-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="af365-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





