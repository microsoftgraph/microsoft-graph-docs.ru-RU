---
title: Обновление windowsProtectionState
description: Обновление свойства объекта windowsProtectionState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ce3c4fcd46e2d627f94e1728d38e9a8f0f91ad30
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939877"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="a931c-103">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="a931c-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="a931c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a931c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a931c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a931c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a931c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a931c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a931c-107">Обновление свойства объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a931c-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a931c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a931c-108">Prerequisites</span></span>
<span data-ttu-id="a931c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a931c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a931c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a931c-111">Permission type</span></span>|<span data-ttu-id="a931c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a931c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a931c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a931c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a931c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a931c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a931c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a931c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a931c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a931c-116">Not supported.</span></span>|
|<span data-ttu-id="a931c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a931c-117">Application</span></span>|<span data-ttu-id="a931c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a931c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a931c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a931c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="a931c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a931c-120">Request headers</span></span>
|<span data-ttu-id="a931c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a931c-121">Header</span></span>|<span data-ttu-id="a931c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a931c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a931c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a931c-123">Authorization</span></span>|<span data-ttu-id="a931c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a931c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a931c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a931c-125">Accept</span></span>|<span data-ttu-id="a931c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a931c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a931c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a931c-127">Request body</span></span>
<span data-ttu-id="a931c-128">В тексте запроса укажите представление JSON для объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a931c-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="a931c-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="a931c-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="a931c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a931c-130">Property</span></span>|<span data-ttu-id="a931c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a931c-131">Type</span></span>|<span data-ttu-id="a931c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a931c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a931c-133">id</span><span class="sxs-lookup"><span data-stu-id="a931c-133">id</span></span>|<span data-ttu-id="a931c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a931c-134">String</span></span>|<span data-ttu-id="a931c-135">Уникальный идентификатор для объекта состояния защиты устройств.</span><span class="sxs-lookup"><span data-stu-id="a931c-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="a931c-136">— Идентификатор устройства, устройства</span><span class="sxs-lookup"><span data-stu-id="a931c-136">This is device id of the device</span></span>|
|<span data-ttu-id="a931c-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a931c-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="a931c-138">Логический</span><span class="sxs-lookup"><span data-stu-id="a931c-138">Boolean</span></span>|<span data-ttu-id="a931c-139">Защита от вредоносных программ включен или не</span><span class="sxs-lookup"><span data-stu-id="a931c-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="a931c-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="a931c-140">deviceState</span></span>|[<span data-ttu-id="a931c-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="a931c-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="a931c-142">Состояние компьютера (например, очистить или Ожидание полного сканирования или помещенных в очередь перезагрузки и т.).</span><span class="sxs-lookup"><span data-stu-id="a931c-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="a931c-143">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="a931c-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="a931c-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a931c-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="a931c-145">Логический</span><span class="sxs-lookup"><span data-stu-id="a931c-145">Boolean</span></span>|<span data-ttu-id="a931c-146">Защита в режиме реального времени включено или нет?</span><span class="sxs-lookup"><span data-stu-id="a931c-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="a931c-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="a931c-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="a931c-148">Логический</span><span class="sxs-lookup"><span data-stu-id="a931c-148">Boolean</span></span>|<span data-ttu-id="a931c-149">Система проверки сети включено или нет?</span><span class="sxs-lookup"><span data-stu-id="a931c-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="a931c-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a931c-150">quickScanOverdue</span></span>|<span data-ttu-id="a931c-151">Логический</span><span class="sxs-lookup"><span data-stu-id="a931c-151">Boolean</span></span>|<span data-ttu-id="a931c-152">Быстрое сканирование просроченные или не?</span><span class="sxs-lookup"><span data-stu-id="a931c-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="a931c-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a931c-153">fullScanOverdue</span></span>|<span data-ttu-id="a931c-154">Логический</span><span class="sxs-lookup"><span data-stu-id="a931c-154">Boolean</span></span>|<span data-ttu-id="a931c-155">Полное сканирование просроченные или нет?</span><span class="sxs-lookup"><span data-stu-id="a931c-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="a931c-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="a931c-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="a931c-157">Логический</span><span class="sxs-lookup"><span data-stu-id="a931c-157">Boolean</span></span>|<span data-ttu-id="a931c-158">Устаревший подписи или нет?</span><span class="sxs-lookup"><span data-stu-id="a931c-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="a931c-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="a931c-159">rebootRequired</span></span>|<span data-ttu-id="a931c-160">Логический</span><span class="sxs-lookup"><span data-stu-id="a931c-160">Boolean</span></span>|<span data-ttu-id="a931c-161">Требуется ли перезагрузка?</span><span class="sxs-lookup"><span data-stu-id="a931c-161">Reboot required or not?</span></span>|
|<span data-ttu-id="a931c-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="a931c-162">fullScanRequired</span></span>|<span data-ttu-id="a931c-163">Логический</span><span class="sxs-lookup"><span data-stu-id="a931c-163">Boolean</span></span>|<span data-ttu-id="a931c-164">Полная проверка, требуется или нет?</span><span class="sxs-lookup"><span data-stu-id="a931c-164">Full scan required or not?</span></span>|
|<span data-ttu-id="a931c-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="a931c-165">engineVersion</span></span>|<span data-ttu-id="a931c-166">Строка</span><span class="sxs-lookup"><span data-stu-id="a931c-166">String</span></span>|<span data-ttu-id="a931c-167">Версия текущей конечной точки защиты ядра</span><span class="sxs-lookup"><span data-stu-id="a931c-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="a931c-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="a931c-168">signatureVersion</span></span>|<span data-ttu-id="a931c-169">Строка</span><span class="sxs-lookup"><span data-stu-id="a931c-169">String</span></span>|<span data-ttu-id="a931c-170">Текущая версия определения вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="a931c-170">Current malware definitions version</span></span>|
|<span data-ttu-id="a931c-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="a931c-171">antiMalwareVersion</span></span>|<span data-ttu-id="a931c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="a931c-172">String</span></span>|<span data-ttu-id="a931c-173">Текущая платформа защита от вредоносных программ версии</span><span class="sxs-lookup"><span data-stu-id="a931c-173">Current anti malware version</span></span>|
|<span data-ttu-id="a931c-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a931c-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="a931c-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a931c-175">DateTimeOffset</span></span>|<span data-ttu-id="a931c-176">Даты и времени последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="a931c-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="a931c-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a931c-177">lastFullScanDateTime</span></span>|<span data-ttu-id="a931c-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a931c-178">DateTimeOffset</span></span>|<span data-ttu-id="a931c-179">Даты и времени последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="a931c-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="a931c-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a931c-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="a931c-181">Строка</span><span class="sxs-lookup"><span data-stu-id="a931c-181">String</span></span>|<span data-ttu-id="a931c-182">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="a931c-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="a931c-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a931c-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="a931c-184">Строка</span><span class="sxs-lookup"><span data-stu-id="a931c-184">String</span></span>|<span data-ttu-id="a931c-185">Последняя версия полная проверка подписи</span><span class="sxs-lookup"><span data-stu-id="a931c-185">Last full scan signature version</span></span>|
|<span data-ttu-id="a931c-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a931c-186">lastReportedDateTime</span></span>|<span data-ttu-id="a931c-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a931c-187">DateTimeOffset</span></span>|<span data-ttu-id="a931c-188">Последнее состояние работоспособности устройства, обнаруженных времени</span><span class="sxs-lookup"><span data-stu-id="a931c-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="a931c-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="a931c-189">Response</span></span>
<span data-ttu-id="a931c-190">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a931c-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a931c-191">Пример</span><span class="sxs-lookup"><span data-stu-id="a931c-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="a931c-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="a931c-192">Request</span></span>
<span data-ttu-id="a931c-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a931c-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 804

{
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="a931c-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="a931c-194">Response</span></span>
<span data-ttu-id="a931c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a931c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```





