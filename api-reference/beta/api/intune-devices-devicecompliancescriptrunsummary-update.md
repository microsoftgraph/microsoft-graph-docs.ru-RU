---
title: Обновление Девицекомплианцескриптрунсуммари
description: Обновление свойств объекта Девицекомплианцескриптрунсуммари.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 906f98b2d6bc3603c750e38d8583ba37dc937a72
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792431"
---
# <a name="update-devicecompliancescriptrunsummary"></a><span data-ttu-id="607c3-103">Обновление Девицекомплианцескриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="607c3-103">Update deviceComplianceScriptRunSummary</span></span>

<span data-ttu-id="607c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="607c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="607c3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="607c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="607c3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="607c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="607c3-107">Обновление свойств объекта [девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="607c3-107">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="607c3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="607c3-108">Prerequisites</span></span>
<span data-ttu-id="607c3-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="607c3-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="607c3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="607c3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="607c3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="607c3-111">Permission type</span></span>|<span data-ttu-id="607c3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="607c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="607c3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="607c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="607c3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607c3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="607c3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="607c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="607c3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="607c3-116">Not supported.</span></span>|
|<span data-ttu-id="607c3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="607c3-117">Application</span></span>|<span data-ttu-id="607c3-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607c3-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="607c3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="607c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="607c3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="607c3-120">Request headers</span></span>
|<span data-ttu-id="607c3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="607c3-121">Header</span></span>|<span data-ttu-id="607c3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="607c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="607c3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="607c3-123">Authorization</span></span>|<span data-ttu-id="607c3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="607c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="607c3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="607c3-125">Accept</span></span>|<span data-ttu-id="607c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="607c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="607c3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="607c3-127">Request body</span></span>
<span data-ttu-id="607c3-128">В тексте запроса добавьте представление объекта [девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="607c3-128">In the request body, supply a JSON representation for the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

<span data-ttu-id="607c3-129">В следующей таблице приведены свойства, необходимые при создании [девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="607c3-129">The following table shows the properties that are required when you create the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md).</span></span>

|<span data-ttu-id="607c3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="607c3-130">Property</span></span>|<span data-ttu-id="607c3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="607c3-131">Type</span></span>|<span data-ttu-id="607c3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="607c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="607c3-133">id</span><span class="sxs-lookup"><span data-stu-id="607c3-133">id</span></span>|<span data-ttu-id="607c3-134">String</span><span class="sxs-lookup"><span data-stu-id="607c3-134">String</span></span>|<span data-ttu-id="607c3-135">Ключевой объект сводки запуска сценария соответствия устройства.</span><span class="sxs-lookup"><span data-stu-id="607c3-135">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="607c3-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="607c3-136">This property is read-only.</span></span>|
|<span data-ttu-id="607c3-137">ноиссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="607c3-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="607c3-138">Int32</span><span class="sxs-lookup"><span data-stu-id="607c3-138">Int32</span></span>|<span data-ttu-id="607c3-139">Количество устройств, для которых сценарий обнаружения не обнаружил проблему, и устройство находится в работоспособном состоянии.</span><span class="sxs-lookup"><span data-stu-id="607c3-139">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="607c3-140">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="607c3-140">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="607c3-141">иссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="607c3-141">issueDetectedDeviceCount</span></span>|<span data-ttu-id="607c3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="607c3-142">Int32</span></span>|<span data-ttu-id="607c3-143">Количество устройств, для которых сценарий обнаружения обнаружил неполадку.</span><span class="sxs-lookup"><span data-stu-id="607c3-143">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="607c3-144">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="607c3-144">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="607c3-145">детектионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="607c3-145">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="607c3-146">Int32</span><span class="sxs-lookup"><span data-stu-id="607c3-146">Int32</span></span>|<span data-ttu-id="607c3-147">Количество устройств, на которых возникла ошибка при выполнении сценария обнаружения и который не был выполнен.</span><span class="sxs-lookup"><span data-stu-id="607c3-147">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="607c3-148">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="607c3-148">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="607c3-149">детектионскриптпендингдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="607c3-149">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="607c3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="607c3-150">Int32</span></span>|<span data-ttu-id="607c3-151">Количество устройств, на которых еще не выполнялась последняя версия сценария соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="607c3-151">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="607c3-152">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="607c3-152">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="607c3-153">ластскриптрундатетиме</span><span class="sxs-lookup"><span data-stu-id="607c3-153">lastScriptRunDateTime</span></span>|<span data-ttu-id="607c3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="607c3-154">DateTimeOffset</span></span>|<span data-ttu-id="607c3-155">Время последнего запуска сценария на всех устройствах</span><span class="sxs-lookup"><span data-stu-id="607c3-155">Last run time for the script across all devices</span></span>|



## <a name="response"></a><span data-ttu-id="607c3-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="607c3-156">Response</span></span>
<span data-ttu-id="607c3-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="607c3-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="607c3-158">Пример</span><span class="sxs-lookup"><span data-stu-id="607c3-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="607c3-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="607c3-159">Request</span></span>
<span data-ttu-id="607c3-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="607c3-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```

### <a name="response"></a><span data-ttu-id="607c3-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="607c3-161">Response</span></span>
<span data-ttu-id="607c3-162">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="607c3-162">Here is an example of the response.</span></span> <span data-ttu-id="607c3-163">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="607c3-163">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="607c3-164">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="607c3-164">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "dad42f14-2f14-dad4-142f-d4da142fd4da",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```



